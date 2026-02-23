# Customer Churn Analysis 

## Northbridge Communications | Power BI - Case Study

Live Interactive Dashboard 

[**Click Here**](https://app.powerbi.com/view?r=eyJrIjoiMjQ0YjNmNGQtNTg2MS00NjExLWJkNzAtNmQwMjYzZWU2NzUyIiwidCI6IjljYTMxODVjLTIzYzEtNDg5Yy1iOTk1LTFlNGVjYWM2MWM3YiIsImMiOjEwfQ%3D%3D)

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

![image alt](https://github.com/Shahimti/Customer-Churn-Analysis-/blob/main/images/Data_Model.png)

The dataset represents customer-level subscription data enriched with segmentation logic and financial measures.

To better simulate real enterprise-level data conditions, the dataset was refined and restructured to introduce transformation and categorization challenges. These were resolved through Power Query transformations and DAX-based modeling techniques, reflecting real-world data preparation workflows.

## Executive Summary

![image alt](https://github.com/Shahimti/Customer-Churn-Analysis-/blob/main/images/KPI's.png)

Northbridge Communications currently serves 5,074 active customers, generating 11.53M in total lifetime revenue.

Churn has reached 26.1%, resulting in 2.05M in lost revenue and exposing 17.8% of total revenue to risk.

This concentration of churn within specific contractual and behavioral segments creates measurable financial volatility rather than uniform customer attrition.

The analysis reveals that churn is concentrated within specific contractual and behavioral segments rather than evenly distributed across the customer base.

Additionally, a scenario-based churn reduction model demonstrates that even modest retention improvements could recover over 100K in revenue, highlighting the measurable financial value of targeted intervention.

## Insights Deep Dive

**Contract Risk Analysis**

![image alt](https://github.com/Shahimti/Customer-Churn-Analysis-/blob/main/images/Churned%20Revenue%20by%20Contract%20.png)

Short-term contracts represent the primary revenue volatility driver, accounting for 1.37M in churned revenue - more than double long-term contract exposure.

Long-term contracts demonstrate significantly stronger retention stability.

**Payment Behavior Risk**

![image alt](https://github.com/Shahimti/Customer-Churn-Analysis-/blob/main/images/Churned%20Risk%20by%20Payment%20.png)

Electronic check customers show the highest churn rate (44.5%), materially higher than automatic payment users.

Billing behavior strongly correlates with retention stability.

**Tenure Lifecycle Impact**

![image alt](https://github.com/Shahimti/Customer-Churn-Analysis-/blob/main/images/Churn%20Rate%20by%20Customer%20Tenure%20.png)

Churn risk decreases as tenure increases:

0–1 year: 46.5%

1–2 years: 29.1%

2–4 years: 18.8%

4–6 years: 10.0%

Churn is heavily front-loaded within early customer lifecycle stages.

**Revenue–Risk Positioning Matrix**

![image alt](https://github.com/Shahimti/Customer-Churn-Analysis-/blob/main/images/Revenue%20Risk%20Positioning%20Matrix.png)

The Revenue - Risk Positioning Matrix highlights segments combining elevated churn probability with significant revenue contribution, enabling capital allocation toward the highest financial return retention opportunities

**Revenue Drivers of Customer Churn**

![image alt](https://github.com/Shahimti/Customer-Churn-Analysis-/blob/main/images/Decompostion%20Tree.png)

The decomposition analysis isolates the highest revenue-loss pathway:

Short Term → Electronic Check → Fiber → Early Tenure

This multi-factor intersection represents Northbridge’s most financially exposed churn cluster.

## Financial Impact Simulation

![image alt](https://github.com/Shahimti/Customer-Churn-Risk-Analysis-PowerBI/blob/main/images/Projected%20Revenue%20Saved%20.png)

A dynamic what-if churn reduction parameter was implemented to estimate potential revenue recovery.

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





