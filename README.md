# credit_risk_classification

## Overview of the Analysis

* The purpose of this analysis is to predict whether or not a loan is at high risk or is healthy.
* The information we are given to determine this is	loan size, interest rate, borrower income, debt to income,num of accounts, derogatory marks, total debt, and loan status. Loan status is what we are looking to predict.
* Loan status is a boolean value. Our dataset contains 77536 total loan status. 
* Stages of the machine learning process for this analysis:
    * The loan_status column will be assigned to the variable 'y' and the rest of the data to an 'X' variable
    * These X and y variables will then be split into test and train variables. 75% of the data train and 25% test.
        * This is done using train_test_split from sklearn.model_selection  
    * Fit the X and y training variables to a LogisticRegression model from skleran.model_selection.
    * Fit the X and y test variables to the trained LogisticRegression model for predictions
    * Generate a confusion_matrix and a classification_report from sklearn.model_selection to see model accuarcy.
* Methods used for this analysis are, LogisticRegression, confusion_matrix, and classification_report

## Results

Accuracy, precision, and recall scores of all machine learning models.

* Machine Learning Model 1:
    * LogisticRegression model
        * Accuracy: Healthy loan 100%, High-risk loan 89%, Overal 99%
        * Precision: Healthy loan 100%, High-risk loan 84%
        * Recall: Healthy loan 99%, High-risk loan 94%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* The LogisticRegression model performs well for predicting a healthy loan status
* It is important for us to be able to predict if a loan is at a high risk (1)

This model does a fantastic job at predicting healthy loans at 100% but its ability to find high-risk could use some work. At an f1 score of 89% this is good but means 11% of high risk loans are missed. 

I worked on this challenge with Conner Dekok.