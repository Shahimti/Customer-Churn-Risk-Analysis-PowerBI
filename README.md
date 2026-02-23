# Customer Churn Analysis - Northbridge Communications

## Power BI - Case Study

Live Interactive Dashboard 

**Click Here**

## Business Background & Problem Statement

Northbridge Communications is a subscription-based telecommunications provider operating under recurring revenue contracts.

The company began experiencing rising customer churn, leading to instability in recurring revenue and reduced customer lifetime value.

Leadership identified the following concerns:

- Increasing churn impacting revenue predictability

- High volatility among short-term contract customers

- Limited visibility into financially exposed customer segments

- No structured quantification of churn-driven revenue loss

- Lack of clear insight into behavioral churn drivers

Northbridge required a structured analytics solution to:

- Identify high-risk customer segments

- Quantify revenue exposure

- Understand behavioral drivers of churn

- Simulate financial impact from improved retention

This case study was developed to translate subscription data into measurable business risk and strategic insight.

## Data Structure & Model Overview

[https://github.com/Shahimti/Customer-Churn-Analysis-/blob/main/images/Data_Model.png]

The dataset represents customer-level subscription data enriched with segmentation logic and financial measures.

To better simulate real enterprise-level data conditions, the dataset was refined and restructured to introduce transformation and categorization challenges. These were resolved through Power Query transformations and DAX-based modeling techniques, reflecting real-world data preparation workflows.

## Executive Summary

[INSERT KPI CARDS SCREENSHOT – PAGE 1 KPI SECTION]

Northbridge Communications currently serves 5,074 active customers, generating 11.53M in total lifetime revenue.

However:

- 26.1% of customers have churned

- 2.05M in revenue has been lost

- 17.8% of total revenue is exposed to churn risk

The analysis reveals that churn is concentrated within specific contractual and behavioral segments rather than evenly distributed across the customer base.

Additionally, a scenario-based churn reduction model demonstrates that even modest retention improvements could recover over 100K in revenue, highlighting the measurable financial value of targeted intervention.

## Insights Deep Dive

**Contract Risk Analysis**

[INSERT SCREENSHOT – Churned Revenue by Contract Type]

Short-term contracts account for the largest share of churned revenue (1.37M), indicating elevated volatility among customers without long-term commitment.

Long-term contracts demonstrate significantly stronger retention stability.

**Payment Behavior Risk**

[INSERT SCREENSHOT – Churn Risk by Payment Type]

Electronic check customers show the highest churn rate (44.5%), materially higher than automatic payment users.

Billing behavior strongly correlates with retention stability.

**Tenure Lifecycle Impact**

[INSERT SCREENSHOT – Churn Rate by Customer Tenure]

Churn risk decreases as tenure increases:

0–1 year: 46.5%
1–2 years: 29.1%
2–4 years: 18.8%
4–6 years: 10.0%

Churn is heavily front-loaded within early customer lifecycle stages.

**Revenue–Risk Positioning Matrix**

[INSERT SCREENSHOT – Revenue–Risk Positioning Matrix]

This matrix identifies high-revenue and high-risk segments, enabling prioritization of retention strategies where financial exposure is greatest.

**Revenue Drivers of Customer Churn**

[INSERT SCREENSHOT – Decomposition Tree]

The decomposition analysis isolates the highest revenue-loss path:

Short Term → Electronic Check → Fiber → Early Tenure

Current exposure:

- Revenue Lost: 2.05M
- Revenue Lost %: 17.8%
- Projected Revenue Saved (sample scenario): 102.46K

## Strategic Recommendations

**Based on the findings, Northbridge Communications should:**

- Incentivize migration from short-term to long-term contracts.

- Encourage transition from electronic check to automatic payment methods.

- Implement early-tenure engagement programs within the first 12 months.

- Prioritize high-revenue fiber customers under short-term contracts for retention campaigns.

- Use churn segmentation to allocate retention budgets efficiently.

- These actions directly address identified revenue exposure segments.




