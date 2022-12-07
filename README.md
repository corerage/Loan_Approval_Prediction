# Loan Approval Prediction

*“where there is data smoke, there is business fire” - Thomas Redman (a data expert)*

![pexels-monstera-5849563](https://user-images.githubusercontent.com/99101608/206177331-a3a5c0c3-176d-45e0-b6ed-4d31e977e5fc.jpg)
Photo Credit: Photo by Monstera from Pexels

This repository contains a project carried out on Loan Approval Prediction.

## Table of Contents:

1. Problem Statement
2. About the Dataset
3. Conclusion


## 1. Business Problem Description

Dream Housing Finance company deals in all kinds of home loans. They have presence across all urban, semi urban and rural areas. Customer first applies for home loan and after that company validates the customer eligibility for loan.

Company wants to automate the loan eligibility process (real time) based on customer detail provided while filling online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. To automate this process, they have provided a dataset to identify the customers segments that are eligible for loan amount so that they can specifically target these customers. 

## 2. About the dataset

The dataset was gotten from the [analytics vidya hackathon platform](https://datahack.analyticsvidhya.com/contest/practice-problem-loan-prediction-iii/#ProblemStatement).There is the train, val, and test file available to download. For the purpose of this project I have used only the train.csv file to train and validate a machine learning model.

The dataset has 614 observations and 13 features.

The description of data attributes is as follows:

|Attributes|Description|
|-|-|
|loan id | Applicant's unqiue loan id|
|gender|  Applicant's gender male/female|
|married | Whether applicant is married or not (Y/N)|
|dependents | Number of dependents on applicant|
|education |  Education level of applicant(graduate/under graduate)|
|self-employed | self employed (y/n)|
|applicant-income | Applicant income|
|co-applicant income | Coapplicant's income, who is apply with applicant as money borrowers.|
|loan amount | Loan amount in thousands|
|loan amount term | Amount of time the lender gives you to repay your loan.|
|credit history | Credit history meets guidlines|
|property area | urban/semi urban / rural|
|loan status | loan approved(y/n)|

## 3. Conclusions

- 4 models: logistic regression, decision tree, random forest and XGboost were trained on the dataset
- parameter tuning was done for each model
- XGboost model is found to be the best performing model with an ROC AUC score of 0.794
- Best model was saved and will be loaded into a webservice using Flask. 
