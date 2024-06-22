# Movie Recommendation System Using SVD Algorithm

**Overview**

This repository contains code to build a movie recommendation system using the Singular Value Decomposition (SVD) algorithm implemented with the Surprise library. The system predicts user ratings for movies based on historical data.

**Installation**

To run the code, ensure you have the necessary libraries installed:

!pip install scikit-surprise

**Some Guiding steps**

1. Import Necessary Libraries
  - import pandas as pd
  - from surprise import Dataset, Reader, SVD, accuracy
  - from surprise.model_selection import KFold
  - from sklearn.metrics import mean_squared_error
  - from math import sqrt

2. Load and Sample the Data
  - Load training and test datasets from CSV files.
  - Sample 10% of the training data for quicker iterations.

3. Create Surprise Dataset
  - Use Surprise's Dataset class to create a dataset from the sampled training data.

4. Define and Cross-Validate the SVD Algorithm
  - Use the SVD algorithm and perform 5-fold cross-validation to optimize parameters.

5. Train the Algorithm and Predict Ratings
  - Train the SVD algorithm on the full sampled dataset and predict ratings for the test set.

6. Create Submission File
  - Create a submission file in CSV format with user-movie predictions.

7. Download Submission File
  - Download the CSV file containing predictions.

**RMSE** is a metric used to evaluate the accuracy of the predicted ratings compared to actual ratings. Lower RMSE values indicate better model performance, reflecting smaller differences between expected/predicted and actual ratings.

**Conclusion**

  - Following the steps outlined above, you can replicate the process, adjust parameters, and evaluate the system's performance using RMSE.











