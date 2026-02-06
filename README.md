# Banking Data analysis methodology and key findings 
I used the linked dataset for studying the trend of long term deposit commitment from a given customer based on various features. 
Jupiter Notebook with analysis is linked here https://github.com/ruchika1/BankingDataAnalysis/blob/main/prompt_III.ipynb

As a first step I dropped null columns and modified 2 boolean columns - target Y and contact into numerical 0,1.
I then encoding the categorical columns using Pandas get_dummies method.
Followed by splitting the data into train and test sets.
To get started with a basic model I used dummy classifier to get baseline accuracy.
I then used the following models to train and compare the accuracies
1. LogisticRegression
2. KNN 
3. DecisionTree
4. SVN

After fitting and predicting the values I compare the models using side  by side confusion matrix as well as a table of train and test accuracy along with fit duration.

My main conclusions are as follows
1. Model with best performance in terms of test accuracy was SVM. However the time taken for training is prohibitively high. Next best is DecisionTree. KNN had the best train accurace but a significantly lower test accuracy
2. In terms of most important features Logistic Regression and KNN both models indicated duration as the most important feature.
