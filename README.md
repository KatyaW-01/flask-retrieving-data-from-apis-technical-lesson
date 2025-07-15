# Book Search App with Open Library API
This project introduces the fundamentals of working with APIs by building a simple book search tool that fetches data from the Open Library API. The app allows users to search for books by title and view basic information such as the book's title and author.
## Purpose
This lesson focused on retrieving (GET) data from external APIs. Skills demonstrated:
* Identify an API endpoint
* Format query parameters
* Send HTTP requests
* parse JSON responses
* Display structured data to users
## Features
* Uses the requests library to interact with a RESTful API.
* Allows users to input any book title and returns the first matching result.
* Formats and displays the title and author of the book.

## How It Works
1. Input: User enters a book title.
2. Formatting: The app prepares the API URL by formatting the search term and defining the fields and limit.
3. API Request: A GET request is sent to the Open Library Search API.
4. Response: The app receives and parses the JSON response.
5. Output: The title and author of the first result are printed to the console.

### Example Code
search_term = input("Enter a book title: ") <br>
result = Search().get_user_search_results(search_term) <br>
print("Search Result:\n") <br>
print(result) <br>
### Sample Output
Enter a book title: the lord of the rings<br>
Search Result:<br> <br>
Title: The Lord of the Rings<br>
Author: J.R.R. Tolkien <br>

## Requirements
* Python 3
* requests library <br>
install dependencies with pip install requests

## API Used
Open Library Search API <br>
Base URL: https://openlibrary.org/search.json <br>
Example Endpoint: https://openlibrary.org/search.json?title=the+lord+of+the+rings&fields=title,author_name&limit=1



