# Rating Products

This repository contains a Python script for calculating weighted ratings for course reviews. The script implements different rating methodologies to provide a more accurate representation of course quality based on both time and user engagement.

Features
Average Rating: Computes the simple mean of all ratings.
Time-Based Weighted Average: Gives higher importance to more recent ratings while reducing the impact of older ones.
User-Based Weighted Average: Weights ratings based on user progress in the course, prioritizing feedback from those who completed more content.
Final Weighted Rating: Combines both time and user-based weightings to calculate a more representative score.
Dependencies
pandas
math
scipy.stats
sklearn.preprocessing.MinMaxScaler
Usage
Ensure you have the necessary dependencies installed and a dataset containing course reviews. The script reads from a CSV file (datasets/course_reviews.csv) and calculates various weighted ratings.

You can adjust the weighting parameters for both time and user engagement to customize the rating calculation.

Example Usage

course_weighted_rating(df, time_w=40, user_w=60)

This repository is useful for anyone analyzing course reviews, ratings, and trying to improve the reliability of rating systems by considering time decay and user engagement.

