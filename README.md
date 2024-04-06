# Movie Recommendation Engine

This Python project is a movie recommendation engine that utilizes collaborative filtering techniques to suggest movies to users based on their past ratings.

## Installation

To run the recommendation engine, you need to install the required libraries. You can do this using pip:


pip3 install numpy
pip3 install scikit-surprise

## Usage

Import Required Libraries: Import the necessary libraries for data manipulation, visualization, and modeling. Ensure you have pandas, scikit-surprise, matplotlib, and seaborn installed.

Import Data: Import the movie ratings data. The code provided utilizes a sample dataset (ratings_small.csv) containing user ratings for various movies.

![Screenshot 2024-04-04 232954](https://github.com/vaishsinghds/Movies-recommendation-engine/assets/161769968/529538be-0318-40b4-9a33-02f1649eae4a)


Exploratory Data Analysis (EDA): Explore the dataset to understand its structure and distribution of ratings. Visualizations such as histograms are used to analyze the distribution of ratings by users and items (movies).

![output_11_1](https://github.com/vaishsinghds/Movies-recommendation-engine/assets/161769968/e1afbf87-f76b-4bbe-934f-641398dc0637)


Data Preprocessing: Filter out rarely rated movies and rarely rating users to reduce the dimensionality of the dataset.

![Screenshot 2024-04-06 004103](https://github.com/vaishsinghds/Movies-recommendation-engine/assets/161769968/b5d29214-df26-435d-b449-863146a6fdf8)

![output_23_0](https://github.com/vaishsinghds/Movies-recommendation-engine/assets/161769968/4c435d25-89c7-4614-96a4-4b70f3167ef7)



Model Training: Train different collaborative filtering models using the Surprise library. Models include SVD, SVD++, SlopeOne, NMF, NormalPredictor, KNNBaseline, KNNBasic, KNNWithMeans, KNNWithZScore, BaselineOnly, and CoClustering.

![Screenshot 2024-04-05 235818](https://github.com/vaishsinghds/Movies-recommendation-engine/assets/161769968/8455f2b8-1da1-486d-aac7-4f24bea61c7f)


Hyperparameter Tuning (Optional): Optionally, perform hyperparameter tuning using GridSearchCV to find the best parameters for the chosen model.

Generate Recommendations: Once the model is trained, it can generate personalized movie recommendations for users based on their past ratings.

## About Surprise

Surprise is a Python scikit for building and analyzing recommender systems. It provides various collaborative filtering algorithms, evaluation metrics, and tools for dataset handling.

Acknowledgments
This project was created as part of a learning exercise and utilizes the Surprise library for collaborative filtering.
