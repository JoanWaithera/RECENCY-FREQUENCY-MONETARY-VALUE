# RECENCY-FREQUENCY-MONETARY-VALUE
RFM Analysis Project

Project Overview

This project conducts an RFM (Recency, Frequency, Monetary) analysis using a dataset stored in BigQuery. The dataset is located in the turing_data_analytics database under the table rfm. The analysis aims to segment customers based on their purchasing behavior to guide marketing strategies.

Objectives

Data Selection: Use one year of data from 2010-12-01 to 2011-12-01.

RFM Calculation: Compute Recency, Frequency, and Monetary values for each customer.

Quartile Segmentation: Assign R, F, and M scores using quartiles.

Customer Segmentation: Categorize customers into groups such as Best Customers, Loyal Customers, and Lost Customers.

Visualization: Present findings using Power BI.

Insights & Recommendations: Identify customer groups that should be targeted for marketing campaigns.

Methodology

1. Data Extraction & Cleaning

Filtered the dataset to include transactions within the given time frame.

Removed duplicate or irrelevant data entries.

2. RFM Calculation

Recency: Days since the customer's last purchase, calculated from 2011-12-01.

Frequency: Total number of purchases made by each customer within the period.

Monetary: Total spending amount per customer.

3. RFM Scoring

Used APPROX_QUANTILES function in BigQuery to compute quartile-based scores (1 to 4) for R, F, and M values.

Cross-validated results with the reference tables rfm_value and rfm_quantiles.

4. Customer Segmentation

Assigned common RFM scores to classify customers into meaningful segments such as:

Best Customers (High R, F, and M scores)

Loyal Customers (High Frequency and Monetary scores)

Big Spenders (High Monetary value)

Lost Customers (Low Recency score)

Other relevant segments based on RFM values.

5. Visualization & Insights

Created a Power BI dashboard to illustrate customer distribution across segments.

Analyzed key trends and provided actionable insights for marketing teams.

Deliverables

Dashboard: Interactive visualization displaying customer segmentation and RFM distribution.

Insights Report: Summary of findings and strategic recommendations for marketing efforts.

Key Insights

Identifying High-Value Customers: Helps prioritize customers who drive the most revenue.

Retention Strategies: Provides targeted approaches to re-engage lost or inactive customers.

Optimized Marketing Spend: Enables efficient allocation of resources towards high-impact customer groups.

Reference

For SQL queries used in this project, please refer to the uploaded file.

Next Steps

Conduct further segmentation based on customer demographics or product categories.

Implement marketing automation for targeted customer engagement.

Compare RFM trends across different time periods to track changes in customer behavior.
