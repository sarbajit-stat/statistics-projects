# statistics-projects
My project using Statistics and Python
<br>
Author:Sarbajit Roy

Customer Churn Prediction for a Streaming ServiceProject OverviewThis project provides an in-depth analysis of customer churn for a subscription-based streaming service. Using three distinct datasets—customer activity, demographic data, and subscription history—we perform exploratory data analysis, extensive feature engineering, and build several machine learning models to predict which customers are most likely to churn. The primary goal is to identify the key drivers of churn and provide actionable, data-driven recommendations to improve customer retention.

Key Findings: Engagement is the Dominating FactorThe analysis conclusively shows that the most significant predictor of churn is a customer's level of engagement with the platform.Primary Driver: Login activity was identified as the single most important feature. Customers who log in infrequently are at a very high risk of churning.

Supporting Metrics: Low Total Watch Time and short Customer Tenure were also strong indicators of churn.This suggests that churn is primarily driven by a customer's perceived lack of value in the service, with inactivity being the most reliable warning sign before they decide to cancel.

Data Sources:The analysis was performed using the following three datasets:(customer_churn_data.csv: Daily records of customer activity, including logins and watch time.)(demographic_data.csv: Static demographic information for each customer.)(subscription_payment_history.csv: Details about each customer's subscription plan and billing cycle.)

Methodology:The project follows a standard data science workflow- 

1.Data Cleaning & Merging: The three data sources were merged into a single, unified dataset for each customer.

2.Feature Engineering: New, powerful features were created to capture customer behavior, including:Total Watch Time: The cumulative minutes a customer has spent watching content.TotalLogins: The total number of times a customer has logged in. 

3.Exploratory Data Analysis (EDA): Visualizations were used to uncover patterns and relationships between various features and customer churn.

4.Data Preprocessing: The data was prepared for modeling through:Ordinal Encoding: For features with a natural order (e.g., Subscription Plan).One-Hot Encoding: For nominal features (e.g., Location, Primary Device, Content Preference).Standard Scaling: To normalize the scale of numerical features. 

5.Model Implementation: Two different classification models were trained and evaluated:Random ForestXGBoostModel Evaluation: The models were compared using a classification report, with a focus on Recall and F1-Score for the churn class to ensure which model works best in predicting whether a customer will get churned or not and to analysis which factor dominate the Churn.

Actionable RecommendationsBased on the model's findings, the following business strategies are recommended to reduce churn:Implement an Inactivity Alert: Create an automated system to flag customers who have not logged in for a set period (e.g., 14 days).Launch Proactive Re-engagement Campaigns: Target these flagged, at-risk customers with personalized emails or promotions to encourage them to return to the platform.Incentivize Longer-Term Plans: Since monthly billing cycles correlate with higher churn, offer discounts to encourage customers to switch to quarterly or annual plans.
