## Overview of the Analysis

## Purpose of the Analysis
The analysis aimed to develop machine learning models for predicting loan status using financial data. The dataset included information such as loan size, interest rate, borrower income, and more. The goal was to predict whether a loan is healthy or high-risk.

## Data Overview
The target variable, loan_status, had two classes: 0 for healthy loans and 1 for high-risk loans. The data exhibited an imbalance, with a higher number of healthy loans compared to high-risk loans.

## Machine Learning Process
## Data Preprocessing:

Separation of data into features (x) and the target variable (y).
Train-test split while maintaining stratification of the target variable.

## Model 1: Logistic Regression (Unbalanced Data):

Training a Logistic Regression model on the original, unbalanced training data.
Evaluation using balanced accuracy, confusion matrix, and classification report.

## Model 2: Logistic Regression with Random Oversampling:

Application of Random Oversampling to address class imbalance.
Training a Logistic Regression model on the oversampled data.
Evaluation of performance using the same metrics.

## Results

## Machine Learning Model 1: Logistic Regression (Unbalanced Data)
Balanced Accuracy: 98.93%
Precision and Recall Scores:
Healthy Loan (Class 1):
Precision: 0.99
Recall: 0.99
High-Risk Loan (Class 0):
Precision: 0.87
Recall: 0.89

## Machine Learning Model 2: Logistic Regression with Random Oversampling
Balanced Accuracy: 99.44%
Precision and Recall Scores:
Healthy Loan (Class 1):
Precision: 0.99
Recall: 0.99
High-Risk Loan (Class 0):
Precision: 0.99
Recall: 0.99

## Summary
Both models performed well, but Model 2, incorporating random oversampling, showed slightly better results.

## Recommendation:

Model 2 (Logistic Regression with Random Oversampling) is Recommended.
Improved balanced accuracy and precision-recall scores.
Addresses the imbalanced nature of the data for a more robust model.
Considerations:

Model choice depends on the problem; here, correctly identifying high-risk loans is crucial.
Model 2 provides a good balance for both classes.
Conclusion:

Model 2, with random oversampling, is the preferred choice for predicting loan status in this financial dataset. It provides a well-balanced approach to identifying both healthy and high-risk loans, crucial for effective risk management in lending.