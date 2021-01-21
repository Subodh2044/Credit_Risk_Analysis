# Credit_Risk_Analysis

## Overview

Loans are vital to run modern day economy and presents banks with enormous opportunities and challenges. Banks charge interest on loans which is the main source of income for banks. Also, banks take huge risk while lending money and if the burrower cannot make a payment, which will result in loan defult creatingn loss for banks. So, in order for banks to make smarter decisions while lending, machine learning can be implemented for risk analysis and make decision on wheather to approve or deny the loan applications.

Typically, banks rely of vriables like income, credit score etc to make decision which poses risk of leaving out other variables that will contribute in decision making. For this project, I am using credit card dataset from LendingCLub.

Using Python and libraries like Scikit-larn libraries, I am building algorithms to predict risk. Following machine learning models are evaluated, comparing it;s strengths and weeknesses to examine the efficacy of the models in classifying and predicting risks:

1. naive Random Oversampling
2. SMOTE Oversampling
3. Undersampling
4. SMOTEENN
5. Balanced Random Forest Classifier
6. Easy Ensemble AdaBoost Classifier

## Results

### 1. Naive Random Oversampling models:
![image](https://user-images.githubusercontent.com/67131400/105268267-806f6b00-5b57-11eb-8292-9dda02e8cfd3.png)

* 0.65 is the balanced accuracy score.

![image](https://user-images.githubusercontent.com/67131400/105269010-c678fe80-5b58-11eb-8ec5-b3c9ff72b361.png)

* Precision score for high risk and low risk is 0.01 and 1.0 respectively and recall score for high risk and low risk is 0.64 amd 0.66 respectively.

### 2. SMOTE Oversampling Model
