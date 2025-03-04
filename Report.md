# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to use a logistic regression model to predict the creditowrthiness of borrowers based on their loan information. 

The data used included interest rate and size of the loan, the borrowers income including their debt to income ratio, the number of accounts the borrower owns, any derogatory marks that borrower has recieved, and the borrower's total debt. Using this data, the regression model predicts whether a loan is high-risk, or in good health. 

Data was stored as a csv and loaded into a pandas DataFrame before isolating the target variable for prediction (loan_status) and the features (loan/borrower information). The data was then seperated into two different sets, one to train the model and the other to test it's predictions. The model was fit to the training data before predicting the testing set's target variables. 

Sklearn's LogisticRegression model was used for the predictions. A confusion matrix and classifcation report (both are available through Sklearn) were generated based on those predictions. 

## Results

* Sklearn's Logistic Regression Model:
    * Accuracy: Total accuracy of 99%.
    * Precision: Healthy loans = 100%, High-Risk loans = 87%
    * Recall: Healthy loans = 100%, High-Risk loans = 95%

## Summary

The regression model used showed high accuracy rates in predicting healthy loans, while it struggled a little with accurately predicting high-risk loans. The model wasn't 100% accurate in all aspects, but it's still useable by staff to screen incoming loans. The tool would ideally be able to 100% accurately predict high-risk loans over healthy loans, so it shouldn't have the final say in loan approval. 

* This model would be a valuable tool for evaluatiing incoming loan applications and screen them for deeper non-numerical analysis by loan officers. 
* It is more important to screen loan applications for high-risk conditions. Although this model isn't perfectly accurate in predicting high-risk loans, it still properly identifies high-risk loans in the provided data with 95% accuracy. 

This model should be used to give loan officers another tool in their arsenal involving loan applications, but it shouldn't be completely relied upon to identify high-risk loans, given the model doesn't show 100% accuracy predicting high-risk. A bad loan would cost the company a lot of money, so professional judgement is still necessary. Loan approval should not be automated in a way that can give out loans. This model may find better usage as a tool to educate/guide future borrowers who are seeking a loan on how appealing/unappealing their loan application might be to the bank. 