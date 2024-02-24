Module 20 Challenge: Credit-Risk-Classification

Credit Risk Analysis Report

1. An overview of the analysis: Explain the purpose of this analysis.

The purpose of this analysis is to train and evaluate a model using historical data from a peer-to-peer lending services company to identify the creditworthiness of borrowers. 

We started by reading the data from the CSV file "lending_data.csv" into a Pandas DataFrame. After, we create the labels set (y) from the "loan_status" column. The values in the "loan_status" column are either 0, which mean that the loan is healthy, and 1, which means that the loan is high-risk. Next, we created the features (X) DataFrame by dropping the "loan_status" column and keeping the remaining columns. Then, we split the data into training and testing datasets using "train_test_split. Then, we created a logistic regreesion model, calculated the accuracy, generated a confusion matrix and printed the classification report with the data. 

In the next part of the assignment, we used the RandomOverSampler module to create a random oversampler model. Then, we used the resampled data to create a logistic regression model, calculate the accuracy score, generate a confusion matrix, and print the classification report. 


2. The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

Results Using Original Data:

- Accuracy Score: 0.9672620331306306

Classification Report

- Precision for healthy loans: 1.00
- Recall for healthy loans: 0.99
- f1-score for healthy loans: 1.00
- Precision for high-risk loans: 0.84
- Recall for high-risk loans: 0.94
- f1-score for high-risk loans: 0.89

Results Using Resampled Data: 

- Accuracy Score: 0.9946686570347071

Classification Report

- Precision for healthy loans: 0.99
- Recall for healthy loans: 0.99
- f1-score for healthy loans: 0.99
- Precision for high-risk loans: 0.99
- Recall for high-risk loans: 0.99
- f1-score for high-risk loans: 0.99


3. A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

Based on the accuracy scores of the model with the original data (97%) and the resampled data (99%), I would recommend the model, since the accuracy score is near-perfect. 