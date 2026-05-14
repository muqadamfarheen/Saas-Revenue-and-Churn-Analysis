<h3 align="center">⭐ End-to-End Data Analytics Project</h3>
<h1 align="center">📊 SAAS REVENUE AND CHURN ANALYSIS</h1>

<p align="center">
  
![Excel](https://img.shields.io/badge/Tool-Excel-green)
![SQL](https://img.shields.io/badge/Language-SQL-blue)
![Power BI](https://img.shields.io/badge/Tool-PowerBI-yellow)
![EDA](https://img.shields.io/badge/Analysis-EDA-orange)
![Data Analysis](https://img.shields.io/badge/Type-Data%20Analysis-purple)
![Churn Analysis](https://img.shields.io/badge/Focus-Churn%20Analysis-red)
![Revenue Analysis](https://img.shields.io/badge/Focus-Revenue%20Analysis-blueviolet)
![CLV:CAC](https://img.shields.io/badge/Metric-CLV%3ACAC-success)
</p>

**Project Title:** Saas Revenue and Churn Analysis Report

**Prepared by:** Farheen Muqadam

**Date:** 14-05-2026
 
---

## 1. Executive Summary  


- **Objective:** Analyze customer churn patterns across plans, acquisition channels, regions, and customer segments to identify key drivers and recommend retention strategies.
- **Overall Churn Rate:** The business is experiencing a high churn rate of 52.1%, indicating significant customer attrition and potential revenue loss.
- **Key Finding 1 (Plan-Based Risk):**
- Starter plan shows the highest churn (71%), followed by Professional (48%).
- Enterprise customers have the lowest churn (22.%). 
- **Key Finding 2 (Acquisition Channel Impact):**
-  Referral (61%) and Partner channels (58%) have the highest churn.
-  irect Sales has the lowest churn (39%).
- **Key Finding 3 (Regional Risk):**
-  Latin America (62%) and Europe (55%) show the highest churn rates.
-  North America has the lowest churn (49%).  
- **Business Impact:** High churn in low-tier and certain acquisition channels is likely eroding revenue stability and increasing customer acquisition pressure 
- **Recommendation:**
- Improve value proposition and onboarding for Starter & Professional plans
-	Optimize acquisition strategy—reduce reliance on high-churn channels (Referral, Partners)
 --- 
## 2. Problem Statement  
CloudTask Pro, a SaaS company, has rapidly scaled its customer base from 0 to 600 customers since 2022. Despite strong revenue growth, the company is experiencing a relatively high churn rate, raising concerns among senior leadership regarding long-term sustainability and customer retention.
The CFO has specifically highlighted the need to better understand:
- Monthly churn trends and whether churn is increasing over time
- Customer segments that are most at risk of churning
- The company’s unit economics, including revenue per customer and the relationship between customer acquisition cost (CAC) and customer lifetime value (CLV)
This analysis aims to:
- Identify key drivers of churn across customer segments
- Evaluate churn patterns over time
- Assess business profitability through core SaaS metrics (MRR, CLV, CAC)
- Provide actionable recommendations to improve retention and optimize growth strategy
--- 
## 3. Data Overview
- **Data Source(s):** internal database (subscription, Monthly Revenue)
- **Time Period:** [e.g., Feb 2022 – Dec 2025]
- **Dataset Size:** Subscription (600 rows -17 columns), Revenue(49 rows- 8 columns)

**Key Variables:**
- plan
- billing_cycle
- Company_size
- Acquisition channel
- Region
- Monthly_revenue
- Churned_date
- Churned(yes/No)
- Nps_score
- Feature_usage Pct
- New_customers
- Churned_customers
- Average_revenue_per_customer
- Customer_acquisition_cost
- Total_mrr

---
 
## 4. Data Preparation
- **Duplicates removed:** Yes
- **Feature engineering:**
- Churn flag(0,1)
- Customer lifetime
- CLV
- Feature_usage_segment (high risk, medium risk, low risk)
- CLV:CAC
- New_mrr
- Churned_mrr
- Net_customer_growth
  
- **Tools used:**
- Excel (Pivot tables, charts, calculated fields, formulas)

## 5. Exploratory Data Analysis (EDA)
### 5.1 Overall Trends
- Overall churn rate: 52.1%
- Churn rate show increasing trend overtime
- MRR shows increasing trend overtime despite the churn rate

### 5.2 Segment Analysis
- **By Plan Type:**
- Highest churn is observed in Starter plan (70.5%), followed by Professional (48%)
- Enterprise customers show the lowest churn (22%), indicating stronger retention among higher tier user
- **By Acquisition Channel:**
- Customers acquired via Referral (61.3%) and Partner channels (58%) exhibits highest churn rates
- Direct Sales customers have the lowest churn(39.3%) ,suggesting higher-quality acquisitions
- **By Region:**
- Latin America (61.7%) and Europe (54.9%) shows the highest churn rates
- North America (48.9%) has the lowest churn, indicating better retention performance in this region
- **By Company Size:**
- Customers with 500+ employees (63.2%) and 1-10 employees (56.7%) show elevated churn rates
- Mid segments (51-200 employees) demonstrate relatively lower churn (42.6%)


### 5.3 Distribution Analysis
- The customer base is distributed across multiple segments, with a significant concentration in medium-risk (254 customers) and high-risk (223 customers) categories.
- Churn distribution is skewed toward:
  - Lower-tier plans (Starter)
  - Certain acquisition channels (Referral, Partner)
  - Specific regions (Latin America, Europe)

→ This indicates that churn is not random but concentrated in identifiable high-risk segments.

---
 
## 6. Key Insights
### Insight 1: Churn is concentrated in lower-tier plans
- **Observation:**Starter plan has the highest churn rate (60.2%) compared to Enterprise (22.2%) and Business (27.4%)
- **Evidence:**as shown in chart below starter plan churn(70%) is significantly higher than enterprise(22%)
  
  ![churn by plan](Images/churn by plan.png)
  
- **Business Meaning:**
Insight 1: Churn is concentrated in lower-tier plans
•	Observation: Starter plan has the highest churn rate (60.2%) compared to Enterprise (22.2%) and Business (27.4%)
•	Evidence: as shown in chart below starter plan churn(70%) is significantly higher than enterprise(22%)
















