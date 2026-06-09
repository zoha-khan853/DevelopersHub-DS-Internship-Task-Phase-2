# DevelopersHub-DS-Internship-Task-Phase-2

Task 1: Term Deposit Subscription Prediction
Task Objective:
Predict whether a bank customer will subscribe to a term deposit using machine learning. This is a binary classification problem — Yes (1) or No (0).

My Approach:
Loaded the Bank Marketing Dataset from UCI (45,211 rows, 17 columns)
Cleaned data by removing unknown values and encoding text columns into numbers
Split data into 80% training and 20% testing
Trained two models — Logistic Regression and Random Forest
Evaluated models using Confusion Matrix, F1-Score, and ROC Curve
Used SHAP to explain 5 individual predictions

Results and Findings:
Model                     F1-Score         ROC-AUC
Logistic Regression       0.41             0.89
Random Forest             0.50             0.93

Random Forest performed better than Logistic Regression
Most important features were: call duration, account balance, age
Longer phone calls strongly predict subscription
Customers contacted too many times are less likely to subscribe
