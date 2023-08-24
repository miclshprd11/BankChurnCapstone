# BankChurnEDA
Exploratory Data Analysis on Bank Churn Data

In this Jupyter Notebook I analize churn data from European banks. 
I see that the data is unalanced and thereofre recall is the best way of scoring any ML clissification models. 

After preping the data, I train classification models that have been gridsearched for the best hyperparameters to the data. 
I trained Logsitic Regression, Support Vector Machine, K-Nearest Naighbors, Naive Bayes, and Decision Tree models. 
SVC was taking way too long so the results of theat model are left out. 

The best scoring models were naive bayes, which achiveved a score of .768 by guessing not churn every time. 
The 2nd best score is Logistic regression, with a score of .573. 

I extracted the feature coefficients from the model and plotted them based on weight. From this I can make several conclsuions about the bank churn. 

1. Tenure is the best indiccator whether a client will stay.
2. Clients who use the more modern technologies of banking tend to not churn, these include electronic checking, paperaless billing, and online security.
3. Client's gender, dpenedent status, and whether they are on a contract are not good inicators on whether they will churn. 
