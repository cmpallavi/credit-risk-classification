# Module 12 Report Template

## Overview of the Analysis

The analysis is done to create a model that will be able to predict whether a loan offered will be a high-risk or healthy loan.

The analysis was done based on the following factors present in the data:
* size of the loan
* interest rate
* borrower's income
* debt to income ratio
* number of accounts the borrower held
* derogatory marks against the borrower
* total debt

The dataset (77,536 data points) was split into training and testing sets. The training set was used to build an initial logistic regression model (Logistic Regression Model) using the LogisticRegression module from scikit-learn. Logistic Regression Model was then applied to the testing dataset. The purpose of the model was to determine whether a loan to the borrower in the testing set would be low- or high-risk and results are summarized below. This intial model was drawing from a dataset that had 75,036 low-risk loan data points and 2,500 high-risk data points. 

## Results


* Logistic Regression Model
Precision: 92% (low-risk loans predicition, the model was 100% precise, though the model was only 87% precise in predicting high-risk loans)
Accuracy: 94%
Recall: 96.5% (on average--the model had 100% recall in predicting low-risk loans, but 94% recall in predicting high-risk loans)


## Summary

The Logistic Regression model was 100% precise at predicting healthy loans. However, it was only 87% precise while predicting high-risk loans. The purpose of the study is to predict high-risk loans and avoid them. Since the precision and accuracy of predicting the high-risk loans is low resulting in more false negatives, I would not recommend the model to use.
