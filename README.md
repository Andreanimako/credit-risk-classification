# Credit Risk Analysis Report 
Module 20 challenge

## Overview

The goal of this analysis was to use machine learning to make predictions about whether a loan is likely to be "healthy" (ie not defaulted), or is likely to be a "high risk loan", given certain information about the loan characteristics, such as loan size and interest rate, and information about the borrower, such as borrower income, debt to income, number of accounts, total debt and derogatory remarks. The loan status was marked as being healthy or high risk based on these features.
The dataset used can be found [here](https://github.com/Andreanimako/credit-risk-classification/blob/main/Credit_Risk/lending_data.csv).

A preview of the dataset used is shown below.
![image](https://github.com/user-attachments/assets/bb82eecc-47d6-4a26-b01f-94c9aee7f81d)

The logistic regression model was used to train and test the machine, and the accuracy of its prediction determined by generating a confusion matrix and classification report.

## Results

The classification report generated was as follows:

![image](https://github.com/user-attachments/assets/2055bbb9-b563-4446-b6a5-691583e57241)

- **Accuracy:**

The overall accuracy of the model in predicing whether a loan was healthy or high risk was 0.99(99%). This means that 99% of the predictions were accurate and suggests that there is only a 1% chance that the model will generate a false prediction about the loan status.

- **Precision:**

The precision for predicting healthy loans was 0.99 and for high risk loans was 0.91. This means that 99% of the predicted healthy loans were truly healthy and 91% of predicted high risk loans were truly high risk.

- **Recall:**

The recall value for predicting healthy loans was 1.00 and for high risk loans was 0.85. Precision is the proportion of true positive predictions to the total positive predictions made by the model. This means that 100% of the predicted healthy loans were correctly identified as being healthy and 85% of predicted high risk loans were truly high risk. This implies that there is a 15% chance that this machine learning model will wrongly predict a loan as being healthy when it is actually unhealthy(false negative).


## Summary
Given the overall accuracy score of 99%, this logistic regression model appears to be highly effective for predicting whether a loan will be paid on schedule or will be high risk. However, while the precision and recall for healthy loans are very high, the recall for high-risk loans is 0.85, indicating that 15% of actual high-risk loans may be misclassified as healthy. To further reduce the risk of false predictions, particularly for high-risk loans, it may be beneficial to consider using this model in conjunction with another model that has a higher recall for high-risk loans. This combined approach could help the company minimize potential losses from granting loans that may end up being high risk.






