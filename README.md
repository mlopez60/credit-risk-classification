# Credit Risk Classification Report 

## Overview of the Analysis


This analysis consisted of using historical lending actvitiy from a peer-to-peer lengind services company to build a model that can identify the crediworthiness of borrowers.

The data consisted of loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, and loan status. The data has roughly 77,000 data points to work the model with. 

The key variable I was looking at was loan satus. Loan status is either 0 or 1, with 0 meaning a loan is healthy and 1 meaning a loan is at a high risk of defaulting. 

Process:
* Read in the lending data
* Split the data into Training and Testing Sets using train_test_split
* Using the training data, fit a logistic regression model.
* Make predictions using the logistic regression model with testing feature data
* Evaluate the model's preformance using confusion matrix and a classification report



## Results

* Machine Learning Model 1:
    * Accuracy: 99%
    
    Loan Status 0 (Healthy):
    * Precision: 100%
    * Recall: 100%
    
    Loan Status 1 (High Risk):
    * Precision: 87%
    * Recall: 89%

## Summary

The model appears to predict the healthy loan at a higher precision, recall, and f1-score than the high-risk loan at 100% and 87%, 100% and 89%, 100% and 88% respectively. The overall weighted average was 99% across the model.

While the model appears to predict the healthly loans at a higher precision, it seems to me that it would be more important for it to identify the high-risk loans at a higher rate. 

It is good to see what loans will be healthy, but I imagine it would be better to know which will be high-risk and better to avoid or watch out for. 

I recommend using the logistic regression model as it gives decent results for the data we were looking for. 
