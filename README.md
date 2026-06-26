# Project Overview

Businesses use coupons to attract customers, but not every customer redeems them. Predicting coupon acceptance helps companies target the right customers, improve marketing efficiency, and reduce promotional costs

# Predicting-Coupon-Acceptance-on-E-commerce-Platforms
In this project, I built an end-to-end Machine Learning pipeline to predict whether a customer will accept a coupon based on demographic information, driving conditions, customer behavior, and coupon attributes.

## Dataset Information
- Rows: 12,684
- Columns: 25
- Target Variable: Accept (Y/N)

## Important Features
- Coupon Type
- Occupation
- Income
- Age
- Passenger
- Destination
- Weather
- Temperature
- CoffeeHouse Visits
- Restaurant Visits
- Bar Visits
- Marital Status
- Education
- Gender
- Coupon Expiration
- Driving Direction
- Distance to Coupon Location

## Data Preprocessing
### The following preprocessing techniques were applied:
- Missing Value Imputation
  - Median for numerical columns
  - Mode for categorical columns
- Outlier Treatment
  - IQR-based capping
- Feature Encoding
- Feature Scaling using StandardScaler
- Data Cleaning & Validation

## Exploratory Data Analysis
Performed detailed EDA including:
- Distribution Analysis
- Correlation Heatmap
- Scatter Plots
- Feature Importance
- Customer Behaviour Analysis

## Machine Learning Models
The following classification algorithms were compared:
- Logistic Regression
- Random Forest
- XGBoost
- Gradient Boosting
- AdaBoost
- Decision Tree
- KNN
- SVC
- Linear SVC
- Ridge Classifier
- Gaussian Naive Bayes
- Bernoulli Naive Bayes
- Perceptron

## Model Evaluation
Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- 10-Fold Cross Validation

## Best Model
Model	Accuracy
✅ XGBoost	74.25%
Random Forest	72.95%

XGBoost achieved the highest prediction accuracy and provided meaningful feature importance scores.

🔥 Top Important Features

According to XGBoost:

1. Coupon Type
2. Occupation
3. Income
4. Age
5. Bar Visits
6. Passenger Type
7. CoffeeHouse Visits
8. Destination
9. Restaurant Visits
10. CarryAway

## Key Insights
- Coupon type is the strongest predictor of coupon acceptance.
- Occupation and income significantly influence customer decisions.
- Younger customer groups appear more frequently in the dataset.
- Most variables have weak linear correlations, indicating that tree-based models capture complex interactions better.
- XGBoost performed best among all tested models.
