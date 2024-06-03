This project implements a movie recommendation system using collaborative filtering. It leverages user ratings to provide personalized movie recommendations. The recommendation engine is built using a K-Nearest Neighbors (KNN) model with cosine similarity as the metric.
Introduction
The movie recommendation system is designed to suggest movies to users based on their past ratings. The system uses collaborative filtering to identify similar users or items and predict ratings for unseen items. In this project, we use a KNN model to find the nearest neighbors for a given movie and generate recommendations.

Dataset
The project uses two datasets:

ratings.csv: Contains user ratings for movies.

Columns: userId, movieId, rating, timestamp

movies.csv: Contains metadata for movies.

Columns: movieId, title, genres


Installation
To run this project, you'll need to have Python installed along with the following libraries:
1.	pandas
2.	numpy
3.	scikit-learn
4.	matplotlib


Usage

Prepare the Data:

Load and preprocess the data from CSV files.

Train the KNN Model:

Define and fit the KNN model using cosine similarity.

Recommendation Engine:

Implement the recommendation engine function.

Generate Recommendations:

Use the recommendation engine to generate movie recommendations.

Code Explanation

Data Loading and Preprocessing:

Load user ratings and movie metadata, merge them, and create a user-item matrix where rows represent users, columns represent movies, and cells contain ratings.

Model Definition and Training:

Define a KNN model using cosine similarity and fit it to the user-item matrix.

Recommendation Engine:

Implement a function that takes a movie name as input, finds its nearest neighbors using the trained KNN model, and returns a list of recommended movies.


License

This project is licensed under the MIT License.
