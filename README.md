# **credit-risk-classification**
identifying the creditworthiness of borrowers
___________________________________________________________________________________

This analysis is to identify the creditworthiness of the loan borrowers, to lower the risk for the lending services.

## **Overview**
___________________________________________________________________________________

**The factors of the data are:**

. The loan size
. Interest rate
. Borrower income
. Debt to income ratio
. Number of the borrower's accounts
. Borrower's derogatory marks
. Total debts of the borrower

In this analysis we are predicting the loan status of the borrower. The entire dataset was split into training and testing sets using train_test_split function that has been imported from  the sklearn.model_selection. The training set of the data is used for the logistic regression model building. Then the model was applied to the testing set. The model is to determine if the loan in the testing set would be low or high risk. 
In the second part of the analysis, the RandomOverSampler imported from the imblearn.over_sampling has been used to reshape the data for a new model. This has been done to resample the data and ensure that the new logistic regression model has an equal number of data points. 

## **Results**
____________________________________________________________________________________

**. For the model 1:**

The logistic regression model predicts the healthy loan ('0') with 100% precision, and the high-risk loan ('1') with 87% precision. The accuracy score is 94%.

**. For the model 2:**

The logistic regression model predicts the healthy loan ('0') with 100% precision, and the high-risk loan ('1') with 87% precision. The accuracy score is 99.6%. 

# **Summary**
____________________________________________________________________________________

Model 2 is less likely to predict false negative results. Model 1 and model 2 have the same precision for the low risk and high risk loans. But Model 2 is showing higher accuracy score (99.6% vs 94%). Also recall shows higher number fo the model 2, meaning that the model 2 identifies true positives better, than model 1. So, if the purpose of the model is to better identify the true positives, then model 2 gives better results.
