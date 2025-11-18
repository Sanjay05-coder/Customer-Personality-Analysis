Customer Personality Analysis


📌 Project Overview


This project analyzes customer personality data to predict their likelihood of responding to marketing campaigns. The main objective is to classify customers into two categories:

0 → Did not accept the last campaign


1 → Accepted the last campaign

The analysis helps businesses understand customer behavior and improve targeted marketing strategies.

✅ Dataset Details

Source: Marketing Campaign Dataset
Key Features:

Demographics: Age, Education, Marital Status, Income, Kids at home, Teens at home
Spending Behavior: Amount spent on wines, meat, fish, sweets, fruits, gold products
Engagement: Recency, Number of web visits, Number of deals purchased
Past Campaigns: AcceptedCmp1–AcceptedCmp5


Target Variable: Response (Binary: 0 or 1)


🛠 Project Workflow

Data Cleaning

Handle missing values
Remove unecessary column
Remove duplicates


Feature Engineering

Create TotalSpend to reduce multicollinearity
Convert birth year to age
Encode categorical variables


Feature Scaling

Applied scaling for models that require it (Logistic Regression, SVM, K-NN)


Model Training

Logistic Regression
Support Vector Machine (SVM)
K-Nearest Neighbors (K-NN)
Decision Tree
XGBoost


Evaluation

Confusion Matrix
Accuracy, Precision, Recall, F1-score
Model comparison visualization




📊 Results

Model Accuracy Comparison:

Logistic Regression, XGBoost, SVM, K-NN, Decision Tree compared visually


Confusion Matrix:

Shows performance for predicting buyers vs non-buyers


Key Insight:

High accuracy overall, but recall for buyers is lower due to class imbalance
Suggested improvements: SMOTE, class weights, threshold tuning


✅ Model Evaluation
To evaluate performance beyond accuracy, we used:


Confusion Matrix:
Shows how well the model predicts buyers (1) vs non-buyers (0).
Example:

True Negatives (TN): Correctly predicted non-buyers
True Positives (TP): Correctly predicted buyers
False Negatives (FN): Missed buyers
False Positives (FP): Incorrectly predicted buyers



Metrics:

Precision: How many predicted buyers were actually buyers.
Recall: How many actual buyers were correctly predicted.
F1-score: Balance between precision and recall.
