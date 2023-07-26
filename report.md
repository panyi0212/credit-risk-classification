# Module 12 Report Template

## Overview of the Analysis

The aim of this analysis is to assess the credit risk of loan applicants by predicting whether they are classified as high-risk or low-risk borrowers.

The financial information used in the analysis includes loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. These factors are utilized to determine whether an applicant is likely to be a healthy loan applicant or a high-risk one.

In the original database, the loan status variables consist of 75,036 data points for healthy loans and 2,500 data points for high-risk loans. After resampling the database, both categories had 56,271 data points.

The data was then separated and split into training and testing datasets using the train_test_split method. Two Logistic Regression Models were created - one using the original dataset and the other using the resampled dataset. Subsequently, predictions were made using both models, and a classification report was generated to compare their performance.

By conducting this analysis, we aim to gain insights into the effectiveness of the Logistic Regression Model with and without the resampling technique for predicting credit risk in loan applicants.


## Results

* Model 1: precision recall f1-score support

              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384


* Model 2: precision recall f1-score support


              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384


## Summary

he model using the resampled data show high accuracy in all aspects of the test proving itself useful and reliable when make a prediction for loan applicants.