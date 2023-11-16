# Credit Analysis Report

## Overview of the Analysis

From the above analysis, the goal is to evaluate the credit risk model's accuracy by performing 2 different sets of logistic regression learning methods, in order to properly classify and categorize the issuance of loans as either 'Healthy' or 'High Risk'. The following attributes which include the loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt were used as the dependent variables;  while the main objective to predict the level of accuracy for estimating a loan status as either 'Healhty' or 'High Risk'. 

In order to perform this analysis, the original data was split where 25% of the data was kept as the testing set; while 75% of the data was kept as the training set.

The following stages of the machine learning process are listed below

1. The data was split as (75% for training and 25% for testing).
2. Developed a logistic regression model to analyze the testing set.
3. Performed a confusion matrix to analyze how the results were split
4. Analyzed the overall accuracy of the precision, recall & F1 scores.
5. Peformed a Resampling operation by using the 'RandomOverSampler' function to create a more balanced distribution.
6. Utilized another regression model with the resampled data set.
7. Performed another confusion matrix to analyze how the results were split again
8. Re-evaluated the new performance of the resampled model by using the same metrics of precision, recall & F1 scores.


## Results

### Machine Learning Model 1: Logistic Regression with Original Data

#### Description of Model 1 with respect to the accuracy of Precision and Recall scores.

The Original Data Set score after the data set was split had the following results

1) Training Date Score: 0.9914878250103177
2) Testing Date Score: 0.9924164259182832

> The initial accuracy score was 99.24% but using the 'Balanced Score' calculation had judged the split of data to be around 94.43% accurate.

Precision:
 - For Healthy loans: The model precision was 100% accurate in determining the true level of healthy loans, with some false positives.
 - For High-risk loans: The model precision was only 87% accurate in determining the issuance of high-risk loans with some false positives.
Recall:
 - For Healthy loans: The model precision was 100% accurate in determining the true level of healthy loans fewer false negatives.
 - For High-risk loans: The model precision was only 89% accurate in determining the issuance of high-risk loans fewer false negatives.


### Machine Learning Model 2: Logistic Regression with Resampled Data 

#### Description of Model 2 with respect to the accuracy of Precision and Recall scores.

> The initial accuracy score and the 'Balanced Score' calculation were now both equal to 99.42%

Precision:
 - For Healthy loans: The model precision was now 99% accurate in determining the true level of healthy loans, with more false positives.
 - For High-risk loans: The model precision had increased to 99% accuracy in determining the issuance of high-risk loans with more false positives.
Recall:
 - For Healthy loans: The model precision was now 99% accurate in determining the true level of healthy loans with more false negatives.
 - For High-risk loans: The model precision had increased to 99% accuracy in determining the issuance of high-risk loans with more false negatives.


## Summary 

The logistic regression performed with the resampled data (Machine Learning Model 2), performs significantly better than the trained data set from (Machine Learning Model 1), more importantly when it comes to analyzing the performance of high-risk loans. The 2nd machine learning model can create better precision and recall scores when it comes to predicting the issuance of high-risk loans, which can help this particular financial institution from suffering massive losses.

Needless to say, the logistic regression model trained with the resampled data helps to provide a more balanced and accurate prediction when it comes to identifying both 'Healthy' & 'High Risk' loans as compared to the original credit risk analysis model. This in turn can help maintain the financial integrity of these institutions by optimizing the loan application and approval process, and in turn, can help mitigate the negative impacts of managing credit risk.

