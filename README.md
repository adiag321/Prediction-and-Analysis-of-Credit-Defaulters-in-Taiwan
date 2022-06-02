# <p align = 'center'> Prediction of Credit Card Defaulters In Taiwan</p>

## OVERVIEW:
The main scope for this project is to predict the occurence of credit card defaulter based on a customers previous history.
The data provided in the csv file are in huge dimensions and the data used here is a PCA of multidimensions data reducing the dimensions so that we can handle with limited computational resources.

This Python prject describes the implementation and data visualization of 6 supervised machine learning techniques implemented on the kaggle dataset of credit card defaulters. As the data is huge in terms of calculations i have used google colab and so first few steps are dedicated for setting up cloud environment.

The dataset is collected from UCI Machine Learning Repository - 
https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)

## DATA DESCRIPTION:

1. ID: ID of each client
2. LIMIT_BAL: Amount of given credit in NT dollars (includes individual and family/supplementary credit
3. SEX: Gender (1=male, 2=female)
4. EDUCATION: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)
5. MARRIAGE: Marital status (1=married, 2=single, 3=others)
6. AGE: Age in years
7. PAY_0: Repayment status in September, 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months,8=payment delay for eight months, 9=payment delay for nine months and above)
8. PAY_2: Repayment status in August, 2005 (scale same as above)
9. PAY_3: Repayment status in July, 2005 (scale same as above)
10. PAY_4: Repayment status in June, 2005 (scale same as above)
11. PAY_5: Repayment status in May, 2005 (scale same as above)
12. PAY_6: Repayment status in April, 2005 (scale same as above)
13. BILL_AMT1: Amount of bill statement in September, 2005 (NT dollar)
14. BILL_AMT2: Amount of bill statement in August, 2005 (NT dollar)
15. BILL_AMT3: Amount of bill statement in July, 2005 (NT dollar)
16. BILL_AMT4: Amount of bill statement in June, 2005 (NT dollar)
17. BILL_AMT5: Amount of bill statement in May, 2005 (NT dollar)
18. BILL_AMT6: Amount of bill statement in April, 2005 (NT dollar)
19. PAY_AMT1: Amount of previous payment in September, 2005 (NT dollar)
20. PAY_AMT2: Amount of previous payment in August, 2005 (NT dollar)
21. PAY_AMT3: Amount of previous payment in July, 2005 (NT dollar)
22. PAY_AMT4: Amount of previous payment in June, 2005 (NT dollar)
23. PAY_AMT5: Amount of previous payment in May, 2005 (NT dollar)
24. PAY_AMT6: Amount of previous payment in April, 2005 (NT dollar)
25. default.payment.next.month: Default payment (1=yes, 0=no)

## METHODS:

1. Importing Libraries and other dependencies
2. Performing Data Visualisation and Analysis
3. Observing Correlation between features of the dataset
4. Cleaning and Preprocessing the data
5. Performing Feature Scaling of Numerical Attributes
6. Applying Machine Learning Algorithm for Classification Problem 
7. Applying Grid-Search CV and check if the accuracy is increased or not
8. Evaluate the performance of the model

<br>
Machine Learning Techniques used:

1) SVM
2) Decision Tree
3) Random Forest
4) Logistic Regression
5) K nearest neighbours
6) Ensemble classifier using decision trees

## CONCLUSION:
1. Using a Logistic Regression classifier, we can predict with 82.5% accuracy, whether a customer is likely to default next month.
2. Using a Stochastic Gradient Descent classifier, we can predict with 83.33% accuracy, whether a customer is likely to default next month.
3. Using a Support Vector Machine classifier, we can predict with 80.83% accuracy, whether a customer is likely to default next month.
4. Using a K-Nearest Neighbour classifier, we can predict with 80.83% accuracy, whether a customer is likely to default next month.
5. Using a Decision Tree classifier, we can predict with 82.83% accuracy, whether a customer is likely to default next month.
6. Using a Random Forest classifier, we can predict with 81% accuracy, whether a customer is likely to default next month.
7. Using a XGBOOST classifier, we can predict with 82.16% accuracy, whether a customer is likely to default next month.
8. The strongest predictors of default are the PAY_X (ie the repayment status in previous months), the LIMIT_BAL & the PAY_AMTX (amount paid in previous months).
9. We found that using Stochastic Gradient Descent and Decision Tree are better.


