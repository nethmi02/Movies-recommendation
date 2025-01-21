# Movie Recommendation System

## Description
This project is a content-based movie recommendation system. It uses natural language processing and machine learning techniques to suggest movies similar to a user's favorite. The system analyzes movie data such as genres, keywords, tagline, cast, and director to calculate similarity scores between movies.

## Features
- **User Input**: Accepts the user's favorite movie name.
- **Recommendation**: Suggests the top 10 movies similar to the input movie.
- **Data Preprocessing**: Handles missing values by replacing them with empty strings.
- **Similarity Measurement**: Uses cosine similarity to compare movies based on combined features.

## Dependencies
The project requires the following Python libraries:
- `numpy`
- `pandas`
- `difflib`
- `scikit-learn`

## Usage
1. Load the dataset
2. Process the data:
   - Select relevant features: `genres`, `keywords`, `tagline`, `cast`, `director`.
   - Fill missing values with empty strings.
   - Combine features into a single text column.
3. Convert the text data into numerical feature vectors using `TfidfVectorizer`.
4. Compute cosine similarity
5. Get user input for a movie name and find the closest match using `difflib`.
6. Retrieve the top 10 most similar movies and display them.

