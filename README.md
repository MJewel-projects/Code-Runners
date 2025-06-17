# Credit Card Customer Churn Analysis

## Overview

This project involves data exploration, cleaning, analysis, and visualization using the Credit Card Customer dataset. It aims to understand customer churn behavior, identify key factors influencing churn, and extract insights that can inform customer retention strategies and improve business decision-making.

## Dataset Content

This project uses the Credit Card Customer Churn dataset from Kaggle:
https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers

The dataset contains information about 10,000+ bank customers, including demographic, account, and credit card usage data. It is primarily used for predicting customer churn — whether a customer will leave the bank.

Key columns include:
 - `CLIENTNUM`: Unique customer identifier
 - `Attrition_Flag`: Churn status (e.g., Existing Customer, Attrited Customer)
 - `Customer_Age`, `Gender`, `Dependent_count`: Demographic information
 - `Education_Level`, `Marital_Status`, `Income_Category`, `Credit_Limit`, `Total_Trans_Ct`, `Total_Revolving_Bal`: Account usage
 - `Months_on_book`, `Avg_Utilization_Ratio`: Customer tenure and credit behavior

## Business Requirements
The primary business goal is to identify factors that influence customer churn and use those insights to support customer retention strategies. Reducing churn can lead to increased customer lifetime value and lower acquisition costs.

### Specific business objectives:
1. **Understand key drivers of customer attrition**  
   Analyse customer demographics and account activity to determine what patterns are associated with churn.

2. **Segment high-risk customers**  
   Develop a profile of customers who are more likely to leave, so that targeted retention strategies can be applied.

3. **Support data-driven decision-making**  
   Provide actionable insights that can inform marketing campaigns, product offers, and personalized communication.

4. **Improve resource allocation**  
   Help the business prioritize customer outreach efforts and design loyalty programs based on churn risk.

## Hypothesis and and Validation
To guide the analysis, the following hypotheses were formed based on domain knowledge and assumptions. Each will be validated through visual analysis using Tableau:

1. **Customers with low transaction activity are more likely to churn**  
   **Rationale:** Infrequent usage may indicate disengagement.  
   **Validation:** Compare average `Total_Trans_Ct` (transaction count) between churned and active customers using boxplots and t-tests.

2. **Older customers are less likely to churn than younger ones**  
   **Rationale:** Older customers may have longer, more stable banking relationships.  
   **Validation:** Analyse churn rate across age groups using histograms and correlation analysis.

3. **Education and income levels influence churn behavior**  
   **Rationale:** Financial knowledge and income may impact engagement with credit products.  
   **Validation:** Use bar plots and group-wise churn percentages to visually compare churn across different `Education_Level` and `Income_Category` values.

## Project Plan
Outline the high-level steps taken for the analysis.
How was the data managed throughout the collection, processing, analysis and interpretation steps?
Why did you choose the research methodologies you used? 

£££££
## The rationale to map the business requirements to the Data Visualisations
List your business requirements and a rationale to map them to the Data Visualisations £££


