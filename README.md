# Capstone Evaluation
Michael Shepherd

**Summary**

Overview and Goal: The goal of this project is to analyze the relationship between a bank customers account information and whether or not they exited their account. I intend to answer the question on what factors drive customers to leave versus stay with their current financial institution. 4 classification models are trained to clasify churn or no-churn The Sklearn library is used to create the models which are then fitted to the data and evaluated based on recall score. When the model's hyperparameters are tuned for the optimal recall score, the best scoring models are interpreted to look at how they function. The opservations taken from the models are then validated by looking at the data. Conclusions are made based on the work in both notnooks and then Future work is then discussed. 
Data can be found here:  https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn?resource=download
**Findings**

The best models for recall of the bank churn data are the Naive bayes, Logistic regression, and Decision tree classifier models. 
<img width="303" alt="image" src="https://github.com/miclshprd11/BankChurnCapstone/assets/80053362/b53e7d2f-1578-4311-93ce-b73ba47d15ec">
The Scores of these models are similar. 
<img width="545" alt="image" src="https://github.com/miclshprd11/BankChurnCapstone/assets/80053362/ee62c112-a342-4990-856a-8285927e674b">
With the Logistic Regression model having a satisfactory recall score, we can extract the weights of each feature the model
Uses to make its classification. The features weights are shown side by side to visualize the magnitude of thier importance. 
Observations and insights can be made from looking at what is a high or low importnace feature, as well as the realative 
difference in magnitude between features.
<img width="477" alt="image" src="https://github.com/miclshprd11/BankChurnCapstone/assets/80053362/e802cad7-1cd0-4b24-9928-c8543c1af543">
With the decision tree classifier having a satisfactory score, we can look at the branches and make observations about
the groups of customers it came up with. The classifier in a way is grouping the samples based on values of thier features. 
Looking towards the root node we see that the classifier immediatly seperated clients based on thier month to month status.

**Conclusions**
This study shows how client information may be used to gain insight into whether they will churn. Certain combinations
of account information serve as trends and customers can be grouped into high risk of churn and low risk of churn. 

Some insights/conclusions we can make from the charts above: 
    
1. Tenure, Monthly charges, and total charges are the top indicators of churn. 
2. Things like gender, senior citizen status, and dependents are not good indicators of churn. 
3. Clients using the fiber optic and electronic check services are churning at a higher rate, we may want to imporve those 
services. 
4. Month to month clients are churning at a high rate. Offer discounts/promotions to returning clients
5. If a customers tenure reaches 6.5 years they are much less likely to churn. Make the experience tailored to newer customers.

**Future Work**
Banks have much more data than shown in this project, a higher recall model with more interesting insights could be done 
with info such as credit score, debt, list of purchases, names, physical location, etc. Graphs can be made to represent the 
churn over time as well as any identify thresholds with features like charges. Data from multiple banks could be compared to
see what kinds of customers prefer which bank, and how marketing strategies can be devised to capture lacking demographics. 
