Customer Churn Prediction & Retention Strategy
1. Business Problem
Objective

The objective of this project is to identify customers who are likely to leave the company (churn) and understand the main factors contributing to customer loss.

By combining data analysis, machine learning, and Power BI visualization, this project aims to help businesses:

Understand customer churn patterns.
Identify the main factors associated with customer churn.
Predict customers who are at risk of leaving.
Prioritize retention actions for high-risk and high-value customers.

The ultimate goal is to support proactive customer retention and reduce customer loss.



2. Data Overview
Dataset Description

The dataset used in this project contains 7,043 customer records and provides information about customer demographics, subscribed services, contracts, payment methods, and financial details.

Dataset Features

The dataset includes:

Customer demographics
Internet and phone services
Contract information
Payment methods
Monthly charges
Total charges
Customer Lifetime Value (CLTV)
Target Variable

The target variable is Churn Value.

0 = Customer stayed with the company.
1 = Customer churned.
Project Objective

The dataset is used to analyze customer behavior, identify churn patterns, and develop a machine learning model to predict customer churn probability.



3. Data Preparation

Data preparation was performed to improve data quality and ensure the dataset was suitable for exploratory data analysis and machine learning.

Data Cleaning

The following steps were performed:

Removed unnecessary customer location identifiers.
Removed churn explanation fields that could cause data leakage.
Checked for duplicate records.
Handled missing values.
Converted columns to appropriate data types.
Feature Engineering

Two additional features were created:

1. Tenure Group

Customers were divided into three categories:

New Customer
Established Customer
Loyal Customer

This feature helps identify how customer loyalty and subscription duration relate to churn.

2. Number of Services

A new feature was created to count the number of services subscribed to by each customer.

This helps analyze whether the number of services is associated with customer retention.

Final Dataset

The cleaned and transformed dataset was prepared for exploratory data analysis and machine learning modeling.




4. Exploratory Data Analysis (EDA) Findings

Exploratory Data Analysis was performed to identify customer behavior patterns and understand the factors associated with churn.

1. Contract Type
Month-to-month customers have the highest churn rate.
One-year and two-year contract customers show better retention.
2. Internet Service
Fiber optic customers show higher churn levels.
Customers using other internet services generally demonstrate lower churn.
3. Payment Method
Electronic check users have higher churn rates.
Customers using automatic payment methods generally show better retention.
4. Tech Support
Customers without Tech Support are more likely to churn.
Providing technical assistance may help improve customer satisfaction.
5. Customer Tenure
New customers are more vulnerable to churn.
Customers with longer subscription periods tend to be more loyal.
Overall Finding

The analysis indicates that contract type, internet service, payment method, technical support, and customer tenure are important factors associated with customer churn.



5. Machine Learning Model
Model Selection: Logistic Regression

Logistic Regression was selected to predict customer churn.

This model was chosen because:

It is easy to interpret.
It estimates the probability of customer churn.
It helps identify factors associated with customer churn.
It supports business decision-making through probability-based predictions.
Model Performance

The Logistic Regression model achieved the following approximate results:

Evaluation Metric	Score
Accuracy	75%
Precision	52%
Recall	80%
F1 Score	63%
ROC-AUC	0.85
Model Evaluation
Accuracy measures the overall proportion of correct predictions.
Precision measures how many predicted churn cases were actually churn cases.
Recall measures how many actual churn cases were correctly identified.
F1 Score balances precision and recall.
ROC-AUC measures the model's ability to distinguish between customers who churn and those who stay.
Conclusion

The model achieved approximately 80% recall and a ROC-AUC of 0.85, demonstrating its ability to identify a substantial proportion of customers at risk of leaving.



6. Model Insights

The Logistic Regression model helped identify factors associated with an increased or decreased probability of customer churn.

Factors Increasing Churn Probability
Fiber optic internet service.
Electronic check payment method.
New customer status.
Higher service complexity.
Factors Reducing Churn Probability
Two-year contracts.
One-year contracts.
Longer customer tenure.
Availability of Tech Support.
Online Security services.
Key Insight

The model suggests that customers with short-term contracts, shorter tenure, and certain service or payment characteristics may require additional attention.

These insights can help businesses understand customer behavior and develop more targeted retention strategies.



7. Retention Strategy

Based on the machine learning predictions, customers were segmented into three risk categories to support targeted retention actions.

Customer Risk Segmentation
Risk Level	Recommended Action
High Risk	Immediate retention campaign
Medium Risk	Preventive engagement
Low Risk	Maintain customer relationship
Model Outputs

The model generates the following information:

Churn Probability: Estimated probability that a customer will leave.
Risk Level: Customer classification into High, Medium, or Low Risk.
Retention Priority: A score used to help prioritize retention efforts.
Retention Prioritization

High-risk customers with high Customer Lifetime Value (CLTV) should receive priority attention.

This approach helps businesses allocate retention resources more effectively and focus on customers who represent greater potential business value.




8. Final Recommendations

Based on the exploratory data analysis and machine learning results, the following business recommendations are proposed to reduce customer churn and improve retention.

1. New Customers
Improve the customer onboarding experience.
Provide support during the first months of subscription.
Introduce early loyalty incentives.
2. Month-to-Month Customers
Encourage customers to move to one-year or two-year contracts.
Offer attractive long-term contract benefits.
Improve engagement with customers on flexible contracts.
3. Fiber Optic Customers
Review pricing and service quality.
Improve technical support.
Monitor customer satisfaction.
4. Electronic Check Users
Encourage customers to adopt automatic payment methods.
Make payment processes easier and more convenient.
5. High-Value Customers
Prioritize customers with high churn probability and high CLTV.
Provide personalized retention offers.
Monitor high-value customer satisfaction.
Final Conclusion

This project demonstrates how data analysis and machine learning can support customer retention strategies.

By identifying churn patterns, predicting customer risk, and prioritizing valuable customers, businesses can take proactive actions to reduce customer loss and improve long-term customer relationships.

DATASET is not mine.
Dataset used for this project was obtained from a publicly available dataset.
The dataset is used for educational and portfolio purposes. All dataset rights belong to the original provider.