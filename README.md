# DevelopersHub-DS-Internship-Task-Phase-2

# Task 1: Term Deposit Subscription Prediction
# Task Objective:
Predict whether a bank customer will subscribe to a term deposit using machine learning. This is a binary classification problem — Yes (1) or No (0).

# My Approach:
Loaded the Bank Marketing Dataset from UCI (45,211 rows, 17 columns)
Cleaned data by removing unknown values and encoding text columns into numbers
Split data into 80% training and 20% testing
Trained two models — Logistic Regression and Random Forest
Evaluated models using Confusion Matrix, F1-Score, and ROC Curve
Used SHAP to explain 5 individual predictions

# Results and Findings:
Random Forest got F1-Score of 0.50 and ROC-AUC of 0.93
Logistic Regression got F1-Score of 0.41 and ROC-AUC of 0.89

Random Forest performed better than Logistic Regression
Most important features were: call duration, account balance, age
Longer phone calls strongly predict subscription
Customers contacted too many times are less likely to subscribe

# Task 2: Customer Segmentation Using Unsupervised Learning
# Objective:
Segment mall customers into distinct groups based on Annual Income and Spending Score using KMeans clustering. These segments help businesses create targeted marketing strategies for each customer group.

# My Approach:
Loaded Mall Customers Dataset — 200 records and 5 columns
Performed EDA by plotting age, income and spending score distributions
Scaled features using StandardScaler for better KMeans performance
Used Elbow Method to find the best number of clusters which was 5
Applied KMeans Clustering and assigned each customer to a cluster
Measured cluster quality using Silhouette Score
Visualized clusters using PCA and t-SNE
Proposed marketing strategy for each segment

# Results and Findings:
Successfully divided 200 customers into 5 distinct segments
Cluster 0 — Low Income Low Spenders — offer discounts and budget deals
Cluster 1 — High Income Low Spenders — target with premium campaigns
Cluster 2 — Medium Income Medium Spenders — offer membership programs
Cluster 3 — Low Income High Spenders — offer installment payment options
Cluster 4 — High Income High Spenders — treat as VIP with exclusive offers
PCA and t-SNE both clearly showed 5 well separated customer groups
Annual Income and Spending Score were the most important features

# Task 4: Loan Default Risk with Business Cost Optimization

# Objective:
Predict loan default likelihood and optimize the decision threshold to minimize financial risk for the bank.

# My Approach:
Loaded and explored Loan Default dataset
Cleaned data by dropping high missing columns and filling rest with median
Encoded all categorical columns using LabelEncoder
Trained Logistic Regression and XGBoost models
Evaluated models using Confusion Matrix, F1 Score and ROC Curve
Defined business costs and adjusted threshold to minimize total cost

# Results and Findings
XGBoost outperformed Logistic Regression with higher F1 Score and ROC AUC
Loan amount, income and interest rate were the most important features
Lower income and higher loan amount customers have higher default risk
Best threshold reduced total business cost significantly
XGBoost with optimized threshold is recommended for loan default prediction
