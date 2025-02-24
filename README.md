movies_in_theater = {
    "Dear Comrade": {"show-time": "9:00AM"},
    "Lucky Bhaskar": {"show-time": "12:00PM"},
    "Orange": {"show-time": "3:00PM"}
}

movie = input("Enter movie you want to watch: ")


if movie in movies_in_theater:

    print(f"Movie '{movie}' is available.")
else:
     print(f"Movie '{movie}' is not available.")


ticket_price = int(input("Enter Ticket Price: "))

if ticket_price > 200:
     print("Get ticket to watch movie")
else:
     print("Cannot provide ticket")


rating = float(input("Enter movie rating: "))

if rating >= 8.0 or rating >= 6.5:
     print("Movie is good")
else:
     print("Movie is below average")


if "Dear Comrade" in movies_in_theater:
    print("Yes")
else:
    print("No")


if movies_in_theater.get("Dear Comrade", {}).get("show-time") == "9:00AM":
    print("Dear Comrade")
else:
    print("Lucky Bhaskar")


movie_genre = input("Enter movie genre (Family Entertainment or Horror): ").strip().lower()

if movie_genre == "family entertainment":
    print("Watch with family")
elif movie_genre == "horror":
    print("Don't watch with children")
else:
    print("Invalid genre entered")


overall_rating = input("Give me overall rating to movie: ")
print(f"The overall rating given is: {overall_rating}")