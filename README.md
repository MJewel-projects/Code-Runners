# Credit Card Customer Churn Analysis

# Overview

This project involves data exploration, cleaning, analysis, and visualisation using the Credit Card Customer dataset. It aims to understand customer churn behaviour, identify key factors influencing churn, and extract insights that can inform customer retention strategies and improve business decision-making.

## Business Map for Visualisation

**1. Pie Chart: Customer Attrition Rates**
 
  * Shows the proportion of attrited (16.07%) vs. existing (83.93%) customers.
  * Business Value: Highlights the scale of churn ((1,627 attrited out of 10,127 total users), aiding decisions on resource allocation for retention strategies.

**2. Histogram: Age Distribution with Churn Rates**

  * Displays age group distribution (e.g., 25–70) with attrited vs. existing customers overlaid.
  * Business Value: Identifies high-churn age segments to target with tailored marketing campaigns.

**3. Stacked Bar Chart: Churn by Income Category**

  * Compares churn rates across income brackets (e.g., <$40K to >$120K) with attrited vs. existing customers.
  * Business Value: Guides gender-specific marketing adjustments based on churn trends.

**4. Bar Charts: Churn Rate by Gender and Age**

   * Compares churn rates for females and males across age groups (e.g., 25–70), with side-by-side bars.
   * Business Value: Highlights gender-specific trends (e.g., females at 40–55 with 18% churn vs. males at 11%), enabling gender-targeted marketing  adjustments.

**5. KPI Cards: Key Metrics**

   * Displays total users (10,127), churn rate (16%), average tenure (36 months), median age (46), and average user balance ($1,163).
   * Business Value: Provides a quick executive summary to assess overall customer health, tenure trends, and financial engagement, supporting strategic planning.

## Dataset Content

This project uses the Credit Card Customer Churn dataset from Kaggle:
https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers

The dataset contains information about 10,000+ bank customers, including demographic, account, and credit card usage data. It is primarily used for predicting customer churn — whether a customer will leave the bank.

Key columns include:
 - `CLIENTNUM`: Unique customer identifier
 - `Attrition_Flag`: Churn status (e.g., Existing Customer, Attrited Customer)
 - `Customer_Age`, `Gender`, `Dependent_count`: Demographic information
 - `Education_Level`, `Marital_Status`, `Income_Category`, `Credit_Limit`, `Total_Trans_Ct`, `Total_Revolving_Bal`: Account usage
 - `Months_on_book`, `Avg_Utilization_Ratio`: Customer tenure and credit behaviour

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
   Help the business prioritise customer outreach efforts and design loyalty programs based on churn risk.

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

1. **Extract**

    * Import the Data into VS code.
    * Import required libraries (pandas & numpy)
 
 2. **Transform:  Data Cleaning:**

    * Drop irrelevant or identifier columns.
    * Handle missing values.
    * Rename columns for readability.
    
3. **Exploratory Data Analysis (EDA):**

   * Visualise churn distribution, correlations, demographics.
   * Use plots like bar chart, Pie Chart and Histogram.

4. **Load(for Analysis)**

   * After transformation, the cleaned DataFrame is saved to be pushed to Github.
   * From local machine import the Data to Tableau. 
   * Use Tableau analytical feature to create Pie Chart, Bar Chart and histogram to exmaine relationship between churned customers and their education, income, sex, and age.

5. **Interpretation**
   
    * Interpret the Data Charts. 
    * Explain  the attrition distribution among genders.
    * Explain  the attrition rate by age,income and age.
    * Demonstrate the methodology used to interpret the cleaned data set. 

## Analysis techniques used

  * Extract Transform load pipeline with data cleaning in Jupyter notebooks.
  * Used appropriate function to fill missing values, remove duplication  and outliners. 

## Main Data Analysis Libraries
  * Pandas
  * Numpy

## Visualisations:
  * Tableau is used to visualised the data.
  * pie chart, histogram,  and bar chart is used to describe the data. 

## Dashboard Design

This project involves the creation of a data-driven, interactive dashboard using Tableau. The goal is to analyze customer churn behavior in the credit card industry. This project helps identify key patterns and metrics associated with churn, providing insights for business decision-making and retention strategies.
You can view the Dashboard [HERE](https://public.tableau.com/app/profile/ivy.kepiro/viz/CreditCardCustomerChurnAnalysis_17502543802840/Dashboard1)

## Ethical considerations

Financial data is highly sensitive and requires compliance to GDPR and other regulations, in order to protect sensitive infomation I have anonymised the data by removing client numbers

## Credits

The Code Institute Learning Management System modules on pandas and data visualisations with Jupyter notebook and Tableau.
Different AI tolls and Visual Studio Code were used to help with code generation and debugging. Team efforts from Ivy Kepiro, Mohammad Jewel and Chris Agyemang

