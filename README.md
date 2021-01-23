# Credit Risk Analysis

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

![image](https://user-images.githubusercontent.com/67131400/105269424-823a2e00-5b59-11eb-8d04-c248e2bb83a0.png)

* Balance accuracy score is 0.65.

![image](https://user-images.githubusercontent.com/67131400/105269441-8b2aff80-5b59-11eb-9db7-035cdd6d35d5.png)

* Precision score for high risk and low risk is 0.01 and 1.0 respectively and recall score for high risk and low risk is 0.64 amd 0.66 respectively.

### 3. Undersampling Model

![image](https://user-images.githubusercontent.com/67131400/105269821-4e133d00-5b5a-11eb-9f9b-92001cc0c7a2.png)

* Balance accuracy score is 0.52.

![image](https://user-images.githubusercontent.com/67131400/105269838-54a1b480-5b5a-11eb-8f30-15f0a8935dfe.png)

* Precision score for high risk and low risk is 0.01 and 1.0 respectively and recall score for high risk and low risk is 0.63 amd 0.41 respectively.

### 4. SMOTEENN

![image](https://user-images.githubusercontent.com/67131400/105270137-e27d9f80-5b5a-11eb-9d7a-4993c85184fb.png)

* Balance accuracy score is 0.64.

![image](https://user-images.githubusercontent.com/67131400/105270165-ef01f800-5b5a-11eb-8a0b-ae7db0a2ecca.png)

* Precision score for high risk and low risk is 0.01 and 1.0 respectively and recall score for high risk and low risk is 0.70 amd 0.57 respectively.

### 5. Balanced Random Forest Classifier

![image](https://user-images.githubusercontent.com/67131400/105270387-499b5400-5b5b-11eb-8825-54d0d47aae71.png)


* Balance accuracy score is 0.80.

![image](https://user-images.githubusercontent.com/67131400/105270396-4ef89e80-5b5b-11eb-961e-1b256d7596db.png)

* Precision score for high risk and low risk is 0.03 and 1.0 respectively and recall score for high risk and low risk is 0.71 amd 0.89 respectively.

### 6.  Easy Ensemble AdaBoost Classifier


![image](https://user-images.githubusercontent.com/67131400/105270581-9f6ffc00-5b5b-11eb-9e87-65a51d607d27.png)


* Balance accuracy score is 0.925.

![image](https://user-images.githubusercontent.com/67131400/105270590-a434b000-5b5b-11eb-8681-4ab81e422cba.png)

* Precision score for high risk and low risk is 0.08 and 1.0 respectively and recall score for high risk and low risk is 0.91 amd 0.94 respectively.

## Summary

* Similar results are produced by Naive Random and SMOTE sampling.
* Precision scores for low risk are produced under sampling and oversampling method but undersampling produced the balance accuracy score and F1 score that is lower.
* There was a very small improvement in balance accuracy score when oversampling and undersampling are combined but on high risk F1 score is low.
* Balance accuracy scoreis higher in Random classifier than resampling models but lower high risk F1 scores.
* Easy ensembler has higher balanced accuracy score bu tlower high risk F1 score.

So, while evaluating the models, undersmpling, oversampling and SMOTEENN will not be the best approach in predicting credit risk due to it's accuracy scores being below 0.66 and F1 scores are not ideal to state that the these models will best classify high risk loan application. Balanced random forest classifier and Ensembler are good in predicting the risk but not classifying. If these model is used in making decision it will be very risky.


