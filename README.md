# credit-risk-classification
The purpose of this analysis was to discover if there is a machine learning technique that can accurately predict if a loan borrower will be trustworthly. 

## Overview of the Analysis

The dataset was divided into two portions: training and testing sets. The initial task involved creating a logistic regression model using the training set. Then, this regression model was used on the testing dataset to determine whether loans extended to borrowers in that set carried low or high risk. 

The initial model was developed using a dataset that contained 75,036 reports of low-risk loans and 2,500 reports of high-risk loans. To ensure equitable representation, the training set data was rebalanced using the RandomOverSampler module from the imbalanced-learn library. This process resulted in an equal count of 56,277 data points for both low-risk (0) and high-risk (1) loans, preserving the original dataset's characteristics.

The rebalanced data served as the foundation for constructing a new logistic regression model, designated as Logistic Regression Model 2. Similar to its precursor, the primary objective of this subsequent model was to categorize loans as either low or high risk for borrowers within the testing set. The summarized outcomes of this endeavor are delineated below.

## Results
<strong>Logistic Regression Model 1:</strong>

* Precision: 100% for low-risk loans, 85% for high-risk loans, 93% on average
* Accuracy: 92%
* Recall: 99% for low-risk loans, 91% for high-risk loans, 95% on average

<strong>Logistic Regression Model 2:</strong>

* Precision: 100% for low-risk loans, 84% for high-risk loans, 92% on average
* Accuracy: 92%
* Recall: 99%

## Summary

Neither model scores above 90% precision for determining the likelihood of high-risk loans. However, Logistic Regression Model 2 had fewer false predictions than model 1, so I would be more likely to recommend Logistic Regression Model 2. Both are still highly accurate, but in a high stakes situation like a large loan, I'm not sure if I would recommend either of these models. If a client really wanted to accurately predict high-risk loan liability, I don't believe 84-85% would be high enough to risk losing a large amount of money. I would say that performance does depend on the problem we are trying to solve, because some problems have different levels of risks. 
