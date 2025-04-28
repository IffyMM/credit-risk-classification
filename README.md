# credit-risk-classification
# Credit Risk Analysis 

## Overview of the Analysis



* The purpose of the analysis.
-The purpose of this analysis is to create a supervised machine learning model that will predict if a loan is healthy (class 0) or high-risk (class 1).
 
* The financial information the data was on, and what you needed to predict.
-The analysis was conducted on financial data, specifically focusing on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

* Provide basic information about the variables you were trying to predict
-We will use logistic regression as a binary classifier for our model here.  The objective was to predict the loan status, either as a healthy loan (0) or a high-risk loan (1). The data used is a 77,500-line CSV file.

* The stages of the machine learning process through is:

-Splitting data into labels and features, with the loan status (healthy or high-risk) being the label and the remaining seven columns as features.
-The data was then split into training and testing data sets.
-A Logistic Regression model from sklearn was created.
-Logistic Regression as a binary classifier was chosen as we are classifying loans as healthy OR high-risk and only those two options.
-The model was then fit with the training data.
-Predictions were made with the test data.
-The model’s performance was evaluated using accuracy, precision, and recall score
- a classification report was generated


## Results

Accuracy: The overall accuracy of the model is 0.99, indicating that it correctly classifies 99% of the instances.

Precision

Healthy Loan (class 0): 1.00
High-Risk Loan (class 1): 0.85

Recall

Healthy Loan (class 0): 0.99
High-Risk Loan (class 1): 0.91

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

-The logistic regression model is doing a very good job predicting the healthy loans (class 0), with precision 1.00, recall 0.99. 
-When it comes to risky loans (class 1), the model is still doing a good prediction, precision 0.85 and recall 0.91.

There are very few high-risk loans for the model to learn from when compared to the number of healthy loans in the data set. If more of these types of loans could be added to the data to train from, there may be improvement to the model.

The lower percision and recall in predicting the risky loans (class 1) can be because of our imbalanced dataset as the support test data for class 1 is only 619 which is very low compared to 18765 for class 0. There is some room for improvement in predicting high risk loans. 


For trying to classify loans, trying to prevent high-risk loans is more important than giving out a loan as more money can be lost from a single loan that defaults than the interest earned from a loan.
