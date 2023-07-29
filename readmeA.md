## Movie Recommendation System

## Introduction
The Movie Recommendation System is a Python program designed to allow users to rate movies and receive recommendations based on their preferences. The system makes use of lists, dictionaries, loops, functions, and Lambda functions to achieve its functionality.

## Functionality

- Upon running the program, the user is presented with a list of available movies.
- The user is then prompted to rate each movie on a scale of 1 to 5 stars.
- The program stores the user's ratings in a dictionary (movie: rating).
- After the user has rated all the movies, the system recommends movies based on the user's preferences, excluding the top-rated movie.
- The recommendations are displayed to the user.


## Code Overview
- `display_movies()`: Displays the list of available movies to the user.
- `get_user_ratings()`: Collects user ratings for each movie and stores them in the `ratings` dictionary.
- `recommend_movies()`: Recommends movies to the user based on their ratings. It sorts the movies in descending order of ratings and excludes the top-rated movie from the recommendations.
- `main()`: The main function that orchestrates the execution of the program. It calls the other functions in the appropriate sequence.

## Usage
To use the Movie Recommendation System, simply run the Python script. The user will be prompted to rate each movie from the provided list. After all movies are rated, the system will generate recommendations and display them to the user.

## Example Output
