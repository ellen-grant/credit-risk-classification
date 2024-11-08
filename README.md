# credit-risk-classification

## Overview of the Analysis

In this analysis, I built a logistic regression model to predict the credit risk associated with loan applicants. The purpose was to assess the likelihood of loan default, identifying loans as either "healthy" (0) or "high-risk" (1) based on historical lending data from a peer-to-peer lending service.

The dataset contains financial information related to previous loans, including various borrower attributes that may impact their likelihood of repaying the loan. The key variable we aimed to predict was the loan_status, where:

* A value of `0` indicates a healthy loan.
* A value of `1` indicates a high-risk loan likely to default.

The machine learning process for this analysis involved the following stages:
1. Data Preparation: Splitting the data into features (X) and target (y), followed by a train-test split to prepare the data for model training and evaluation.
2. Model Selection: Using LogisticRegression as the chosen algorithm due to its suitability for binary classification problems.
3. Model Training and Evaluation: Training the model on the training data, generating predictions, and evaluating the model’s performance using accuracy, precision, and recall metrics.

## Results

Machine Learning Model 1: Logistic Regression
* Accuracy: 0.99 – The model achieved a high accuracy score, correctly classifying 99% of the loan statuses.
* Precision:
    * Healthy Loan (0): 1.00 – The model demonstrates perfect precision in identifying healthy loans, with no false positives.
    * High-Risk Loan (1): 0.86 – Reasonable precision, with some healthy loans misclassified as high-risk.
* Recall:
    * Healthy Loan (0): 0.99 – The model successfully identifies 99% of actual healthy loans.
    * High-Risk Loan (1): 0.94 – Good sensitivity, capturing 94% of high-risk loans, indicating effective identification of potential defaults.

## Summary

The logistic regression model performs very well, with high accuracy, precision, and recall scores for both healthy and high-risk loan classifications. It particularly excels in identifying healthy loans accurately, and it is also effective in predicting high-risk loans, with only a few misclassifications.

* Recommendation: Based on these results, we recommend this logistic regression model for the company's credit risk assessment purposes. Its high accuracy and strong metrics make it reliable for predicting both healthy and high-risk loans, which is crucial for minimizing potential loan defaults and managing lending risk.
* Performance Consideration: Given the context, accurately predicting high-risk loans (1) is slightly more critical, as it allows the company to proactively address potential defaults. The model’s recall of 0.94 for high-risk loans indicates it performs well in this aspect, making it suitable for the task.