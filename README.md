# ds_mod_20_suprervised_ML
Homework for week 20 of the data analysis bootcamp 2024 - Supervised ML

### All deliverables are located in the 'Submission' folder.

The purpose of this analysis was to train and evaluate a logistic regression model based on loan risk.

The data was based on historical lending activity from a peer to peer lending company. It had several different features of the data like loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, and loan status. We needed to predict the creditworthiness of borrowers.

Based on the data We needed to know how many loans were in good status and how many were in a negative status, to do this I used .value_counts. By using .value_counts it made it easier to see how the data is balanced, in this case it was severely imbalanced. 

To begin the stages of the machine learning process I needed to make sure I had all of the imports required to run all my models. Next I needed to split the data into training and testing datasets. I did this by reading in the initial CSV file then creating the X and y labels, which were the features and loan_status respectively. Next, I did some data exploration and checked the data to make sure there were no nulls, check that all of the columns were numeric, and determine if I needed to scale the data. The data did end up needed a scaler, so I scaled the data then began splitting data for the train. After the data was done being prepped I ran the logistic regression and started to analyze the results.

I used a logistic regression because this data had a binary outcome, meaning that either the loans were in good standing or they were defaulted on. 

Some parts of the code came from in class activities, instructor lead office hours, and out AI learning assistant.

