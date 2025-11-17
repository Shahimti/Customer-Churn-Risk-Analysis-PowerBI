**Customer Churn Analysis (Power BI)**

**Project Overview**

- This project focuses on analyzing customer churn to identify key factors that influence how many customers stay or leave by different segmentations. Using Power BI, the goal was to create an interactive dashboard that highlights patterns in customer behavior and helps explain which customer segments have the highest churn.

**Project Description**

- The purpose of this project is to explore churn behavior within a telecom dataset that was sourced from Kaggle and develop insights that can support retention strategies. The dashboard allows users to slice the data by contract type, payment method, gender, tenure, and internet service.

The visuals were designed to answer questions such as:

- Which customer segments churn the most?

- How do contract type and payment method influence churn?

- What combinations of features lead to higher churn?

- How does tenure affect customer behavior?

This one-page dashboard brings together multiple perspectives of the data and is fully interactive to support dynamic analysis.

**Dataset Information**

Dataset Source: Kaggle Open Data Set

**Columns Used**

- Customer ID

- Gender

- Senior Citizen

- Partner

- Dependents

- Tenure

- Tenure Group

- Phone Service

- Multiple Lines

- Internet Type

- Has Internet

- Online Security

- Online Backup

- Device Protection

- Tech Support

- Streaming TV

- Streaming Movies

- Contract

- Contract Type

- Paperless Billing

- Payment Group

- Monthly Charges

- Total Charges

- Churn

**Data Cleaning Steps**

Several cleaning steps were performed in Power Query before building the visuals:

- Removed duplicate and empty Customer ID rows

- Standardized all Yes/No fields

- Replaced “No Internet Service” and “No Phone Service” with “No” for consistency

- Created Tenure Group buckets (0–1, 1–2, 2–4, 4–6 years)

- Categorized Contract Type into Short Term and Long Term

- Grouped Payment Method into Automatic, Mailed Check, Electronic Check

- Ensured Monthly Charges and Total Charges were converted to numeric formats

- Removed blank Total Charges rows

- Created additional helper columns for modeling and visualization

**Key DAX Measures**

These measures were created to support the dashboard:

Total Customers =
DISTINCTCOUNT('Teleco Raw Data'[Customer ID])

Churn Customers =
CALCULATE(
    DISTINCTCOUNT('Teleco Raw Data'[Customer ID]),
    'Teleco Raw Data'[Churn] = "Yes"
)

NonChurn Customers =
[Total Customers] - [Churn Customers]

Churn Rate (%) =
DIVIDE([Churn Customers], [Total Customers], 0)

Retention Rate =
1 - [Churn Rate (%)]

Avg Monthly Charges =
AVERAGE('Teleco Raw Data'[Monthly Charges])

Avg Total Charges =
AVERAGE('Teleco Raw Data'[Total Charges])

**Dashboard Overview**

The dashboard includes the following key visuals:

**Slicers:**

- Contract Type

- Payment Group

- Gender

- Paperless Billing

- Tenure Group

- Internet Type

**Charts**

- Clustered Bar Chart: Churn Customers by Tenure Group -** Displays churn counts by tenure segments and reveals which tenure ranges have the highest churn**

- Clustered Column Chart: Churn Rate (%) by Payment Group - **Compares churn rates across payment methods**

- Stacked Column Chart: Churn Customers by Contract Type - **Highlights churn distribution across short-term and long-term contracts**

- Decomposition Tree: Analyzes churn customers and identifies the strongest contributing factors (Contract Type, Payment Group, Internet Type, Monthly Charges, etc.).

- Matrix: Churn Rate by Contract Type and Internet Type - **Provides a cross-segmentation view to understand how internet service type interacts with contract type in explaining churn**

**KPI Cards**:

- Total Customers

- Churn Rate (%)

- Churn Customers

- Avg Monthly Charges

**Files in Repository**

This repository contains the following files:
- README.md — Project documentation

- Dashboard.pdf — A PDF export of the Power BI dashboard

- Telecom_Churn.pbix — The Power BI file for interactive exploration

**Interactivity**

The dashboard is fully interactive. All slicers dynamically update the visuals, allowing users to analyze customer churn across different segments.

Examples of interactions include:

- Filtering churn behavior by gender or payment group

- Observing how churn changes for specific internet types

- Exploring high-churn customer segments using the decomposition tree

- Comparing churn between long-term and short-term contracts

**Findings From the Project**

Below are the types of insights observed from the dashboard. 

- Customers with short-term contracts had a higher churn rate of **0.27%** compared to long-term contract customers.

- Payment method played a major role. Customers using Electronic Check showed a churn rate of **0.45%**, significantly higher than the other groups.

- Tenure was strongly related to churn. Customers in the first 0–1 year tenure group churned at **0.47%**, while long-tenure customers had much lower churn.

- Fiber internet users showed higher churn in specific segments, especially when combined with **short-term contracts & electronic payment**.

- The decomposition tree identified the top churn segment as **Short Term - Contract Type + Electronic - Payment Group + Fiber - Internet Type**.

- Average monthly charges for churned customers were approximately **$80** compared to **$61.50** for retained customers.

These findings help identify which customer groups should be targeted for retention strategies.

**Tools and Skills**

- Power BI Desktop

- Power Query for data cleaning

- DAX for calculated measures

- Data modeling

- Dashboard design

- Exploratory data analysis

**Author Details**

Project created by:Shah Imtiaz
Mail: Shahimti12@gmail.com


