## Analysis Overview:
The study employs machine learning techniques to analyze a historical lending dataset from a peer-to-peer lending services company. The goal is to develop a model that can effectively identify the creditworthiness of borrowers. Key factors considered in the analysis include loan size, interest rate, borrower's income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

## Dataset Split:
The dataset, comprising 77,536 data points, was divided into training and testing sets. The initial logistic regression model (Logistic Regression Model 1) was constructed using scikit-learn's LogisticRegression module. Model 1 was then applied to the testing dataset.

## Data Resampling:
To address class imbalance, where there were 75,036 low-risk and 2,500 high-risk data points, the training set underwent resampling using the RandomOverSampler module from imbalanced-learn. This ensured an equal number of data points (56,277) for both low-risk (0) and high-risk (1) loans based on the original dataset.

## Logistic Regression Model 2:
The resampled data was utilized to build Logistic Regression Model 2, aimed at predicting whether a loan to a borrower in the testing set would be low- or high-risk.

## Results Summary:
Logistic Regression Model 1:

Precision: 93%
Accuracy: 94%
Recall: 95%
High precision for low-risk loans (100%), but slightly lower precision for high-risk loans (87%).
Logistic Regression Model 2:

Precision: 93%
Accuracy: 100%
Recall: 100%
Achieves perfect precision and recall for both low- and high-risk loans.

## Conclusion:
Logistic Regression Model 2 exhibits a reduced likelihood of false negative predictions. While it predicts slightly more false positives (low-risk when actual is high-risk), it maintains high accuracy and recall. Given the goal of identifying high-risk loans, neither model achieves above 90% precision. However, Logistic Regression Model 2 is recommended due to its overall superior performance in accuracy and recall on the testing data.
