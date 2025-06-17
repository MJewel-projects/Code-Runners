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

--Outline the high-level steps taken for the analysis: 

1. Extract

 -Open VS Code and activate a virtual environment
 -Import required libraries (pandas, numpy, matplotlib, seaborn, sklearn)
 -Load the dataset using: 
 import pandas as pd
df = pd.read_csv('path/to/BankChurners.csv')

 2. Transform

-Clean the data:

Drop irrelevant or identifier columns (e.g., CLIENTNUM).

Handle missing values (though this dataset is usually clean).

Rename columns for readability if needed.

Feature Engineering:

Convert categorical variables using encoding (e.g., pd.get_dummies() or LabelEncoder).


Exploratory Data Analysis (EDA):

Visualize churn distribution, correlations, demographics.

Use plots like bar charts, boxplots, heatmaps, etc.

3. Load(for Analysis)

-After transformation, the cleaned DataFrame is saved to be pushed to Github

How was the data managed throughout the collection, processing, analysis and interpretation steps? 

Step___________|___________Description
Collection	               The data was pre-collected and provided in CSV format, avoiding collection biases.
Processing	               Handled in VS Code using pandas. Involved removing unused columns, dealing with types, coding  
                           categorical values, and normalizing.
Analysis	                  Exploratory Data Analysis to uncover patterns, trends, and relationships. Followed by building
                           models (e.g., logistic regression, decision trees) to predict churn.
Interpretation	            Model evaluation (accuracy, recall, precision) and graphical summaries helped interpret the 
                           effect of features on churn.

--Why did you choose the research methodologies you used? 

-Quantitative Analysis: The dataset is numeric-heavy and allows for statistical, measurable patterns.

-Descriptive Statistics & Visualization: Help understand the structure and spot outliers/trends before modeling.

-Reproducibility: Using Python in VS Code ensures the process is well-documented, modular, and repeatable.

-Efficiency: VS Code supports powerful extensions (e.g., Jupyter Notebooks, Linting, Git) that accelerate development and collaboration.


## The rationale to map the business requirements to the Data Visualisations

The first visualization uses a pie chart to represent customer attrition rates, providing a clear overview of the problem's scale. This helps the business assess whether allocating resources to address attrition is a worthwhile investment

The second visualization is a histogram displaying the age distribution alongside churn rates, enabling the bank to evaluate if specific age groups should be prioritized in future marketing strategies

The third chart is a stacked bar graph that compares attrition rates by gender. This insight can guide the bank in refining its marketing efforts toward either male or female customers, depending on observed trends

Lastly, a scatter plot illustrates the relationship between attrition and gender in relation to both "months on the books" and total transaction amounts. This type of analysis offers various strategic insights—for instance, understanding how customer tenure or spending habits relate to churn can inform the development of targeted perks or retention strategies for both new and long-standing clients

## Analysis techniques used

-Extract Transform load pipeline with data cleaning in Jupyter notebooks.
-Visualisations: pie chart, histogram, bar chart and scatter plot

## Ethical considerations

Financial data is highly sensitive and requires compliance to GDPR and other regulations, in order to protect sensitive infomation I have anonymised the data by removing client numbers

## Dashboard Design

## Development Roadmap
What challenges did you face, and what strategies were used to overcome these challenges?


## Main Data Analysis Libraries

-Pandas
-Numpy
-Plotly
-Seabon
-Matplotlib

## Credits

The Code Institute Learning Management System modules on pandas and data visualisations with Matplotlib,Seaborn and Plotly
Chat GPT and Microsoft Copilot integrated into Visual Studio Code was used to help with code generation and debugging
Team efforts from Ivy Kepiro, Mohammad Jewel and Chris Agyemang

