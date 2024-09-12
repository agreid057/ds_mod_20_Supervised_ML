# Module 12 Report 

## Overview of the Analysis

The purpose of this analysis was to train and evaluate a logistic regression model based on loan risk.

The data was based on historical lending activity from a peer to peer lending company. It had several different features of the data like loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, and loan status. We needed to predict the creditworthiness of borrowers.

Based on the data We needed to know how many loans were in good status and how many were in a negative status, to do this I used .value_counts. By using .value_counts it made it easier to see how the data is balanced, in this case it was severely imbalanced. 

To begin the stages of the machine learning process I needed to make sure I had all of the imports required to run all my models. Next I needed to split the data into training and testing datasets. I did this by reading in the initial CSV file then creating the X and y labels, which were the features and loan_status respectively. Next, I did some data exploration and checked the data to make sure there were no nulls, check that all of the columns were numeric, and determine if I needed to scale the data. The data did end up needed a scaler, so I scaled the data then began splitting data for the train. After the data was done being prepped I ran the logistic regression and started to analyze the results.

I used a logistic regression because this data had a binary outcome, meaning that either the loans were in good standing or they were defaulted on. 

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model- Logistic Regression:
-The model is pretty accurate, which is a little bit surprising based on the imbalance
-No signs of over fitting based on the train and test precision accuracy
-Recall scores are also very close signifying a pretty good fit
-The confusion matrix shows only 90 false positives and 12 false negatives, which again is pretty good for a larger data set like this
-The ROC curve is almost perfect, this shouldn't be the only variable that you evaluate your model on, this is because of the imbalance in the data

## Summary

There is severe imbalance in this data, which made me think that the models would not perform as expected. There were very few defaulted loan_status compared to the size of the data. The logistic regression model does a pretty accurate job at predicting both the healthy loans and the high risk loans. There are pretty comparable metrics of the train set (0 was 0.99, 1 was 0.98) and the test set (0 was 0.99, 1 was 0.99).This shows that there were no signs of over fitting even with the data being imbalanced. Looking at the Confusion Matrix you can also see that there were only 90 false positives and 12 false negatives. When looking at the ROC curve you can see an almost perfect model but that should not be the only part of the analysis you base the prediction on because of the sever imbalance. Several other models like SVC and KNN could further show the relationships in a better way in future work.

