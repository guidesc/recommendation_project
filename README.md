# Amazon Fine Food Recommendation

Author: Xiaoyu Tian, Tailai Zhang, Dongxue Shao, Shenghua Du

## Introduction
This is our final project for Machine Learning Class. We aim to build a recommendation system based on data from 
[Amazon Fine Food Reviews](https://www.kaggle.com/snap/amazon-fine-food-reviews). 

## Exploratory Data Analysis
Please refer to `Review.ipynb` for the data cleaning, feature engineering, and dashboard.

## Recommendation System
Please refer to `main.py`.

We mainly covers all the following methods:

- Collaborative Filtering (Matrix Factorization)
- PMF
- SVD
- Random Forest

## Performance

As for evaluation, we choose MSE (including train set and test set MSE) and Confusion Matrix (score > 4 as recommend, 
score < 4 as not recommend) to evaluate all the models above. 

Colloborative Filtering based on Matrix Factorization acheived the best performance.

## Time features

Finally, we creatively add "Time features" into the recommendation system and consider 
"Time model" as a threhold, say, the prediction from time model is below 3, we will drop 
the recommendation candidates. (Please refer `Review.ipynb` for our time model)



