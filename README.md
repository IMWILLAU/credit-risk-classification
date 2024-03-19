## Overview of the Analysis

**Explain the purpose of the analysis**
The purpose of the analysis is to develop machine learning models to predict the creditworthiness of borrowers based on lending activity data from a peer-to-peer lending services company. This analysis aims to assist in decision-making processes related to loan approvals and risk management.

**Explain what financial information the data was on, and what you needed to predict.**
The dataset contains contains financials information on borrowers, including attributes such as income, debt-to-income ratio, credit score, loan amount, and loan status. The prediction target is the loan status which indicates whether a borrower is likely to repay the loan or is at high risk.

**Provide basic information about the variables you were trying to predict (e.g., `value_counts`).**

Loan status (target variable):
- 0: Fully paid loans
- 1: Charged off loans
Value Counts:
- Class 0: 
- Class 1: 

**Describe the stages of the machine learning process you went through as part of this analysis.**
- Create label sets and feature Dataframe frozen the provided dataset.
- Split the data into training and testing data sets.
- Create a logistic regression model and fit our original data into the model.
- Making the prediction on testing data labels by using a testing feature data and the fitted model.


**Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithm).**
- Logistic Regression on the original fitted data
- Confusion Matrix for the model
- Classfication report

## Results
This section describes the accuracy and balanced accuracy scores, and the precisions and recall scores of the two machine learning models used for the challenge.

**Logistic Regression**

![image](https://github.com/IMWILLAU/credit-risk-classification/assets/61693472/545ab395-54fa-40a4-9966-c6ce663a4f7f)

- Precision (Class '0'): 1.00
- Precision (Class '1'): 0.87
- Recall (Class '0'): 1.00
- Recall (Class '1'): 0.89
- F1-Score (Class '1'): 1
- F1-Score (Class '0'): 0.88

**Confusion Matrix**

![image](https://github.com/IMWILLAU/credit-risk-classification/assets/61693472/8a1a682f-2165-4022-bdd8-7c4205f9f67f)

- True Negatives (TN): 18,679 instances were correctly predicted as negative (class 0).
- False Positives (FP): 80 instances were incorrectly predicted as positive (class 1) when they were actually negative (class 0).
- False Negatives (FN): 67 instances were incorrectly predicted as negative (class 0) when they were actually positive (class 1).
- True Positives (TP): 558 instances were correctly predicted as positive (class 1).


## Summary

Based on the evaluation results, the performance models may vary depending on the problem of what is being addressed and/or data set. Logistic regression model appears to predict both health and high risk loans quite accurately with high precision, recall and F1-scores for both classes. However, further validation and monitoring of the model's performance in real-world scenarios are advisable before deployment.

