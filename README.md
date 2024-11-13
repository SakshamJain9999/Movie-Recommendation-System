# Movie-Recommendation-System

This project implements a movie recommendation system that suggests movies based on user preferences and viewing behavior. The recommendation engine is built using the MovieLens dataset and offers personalized movie recommendations by analyzing user ratings and movie metadata.

## Project Overview
The objective of this project is to create a recommendation system that can:

Suggest movies based on user ratings and preferences.
Provide interactive search capabilities for specific movie titles.
Use machine learning techniques to improve recommendation accuracy.

## Dataset
Data files used:
movies.csv: Contains information about movies (e.g., movieId, title, genres).
ratings.csv: Contains user ratings with columns userId, movieId, rating, and timestamp.

## Project Structure
### Data Preprocessing: Cleans and prepares the dataset for analysis.
### Feature Extraction: Utilizes TF-IDF vectorization to process movie titles for search functionality.
### Recommendation Model: Generates personalized movie recommendations using similarity measures.
### Interactive Search: Provides a live search box that suggests movies as users type.
### User-based Collaborative Filtering: Recommends movies by finding similar users based on rating behavior.

## Key Components
### Data Cleaning:
Removed special characters from movie titles using regular expressions.
Cleaned data stored in a new column for efficient processing.

### TF-IDF Vectorization:
Implemented TF-IDF on movie titles for textual similarity.
Supports n-gram modeling for better search and recommendation accuracy.

### Similarity Search Function:
Calculates cosine similarity between user-inputted title and movie dataset.
Finds the top 5 most similar movies based on title similarity.

### User-based Recommendations:
Identifies similar users based on movie ratings.
Recommends movies frequently rated highly by similar users.

### Recommendation Scoring:
Calculates recommendation scores based on user ratings and similarity.
Combines similar user preferences with general user popularity for weighted recommendations.
