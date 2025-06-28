# Retail Sales and Customer Segmentation

## Project Overview
This project analyzes online retail sales transaction data from a UK-based e-commerce store, covering the period from December 2010 to December 2011. The goal is to generate actionable business insights by examining sales trends, product performance, return rates, and customer purchasing behavior using RFM segmentation. The project includes data cleaning and RFM analysis in Python, with all dashboard visualizations built in Tableau.

## Data Source
The dataset was obtained from the UCI Machine Learning Repository, specifically the Online Retail Dataset. 
[It](https://drive.google.com/file/d/1F0m075kYRABRz8sVb9bmA454r_HNw72P/view?usp=sharing) contains transactional sales data from a UK-based online retailer, covering the period from December 2010 to December 2011.

## Objective
To answer key business questions regarding sales performance, customer segmentation, and geographical revenue contribution, with the aim of supporting data-driven business decisions and targeted marketing strategies.

## Business Questions
1.	What are the monthly sales trends in terms of revenue and quantity?
2.	Which products are the top-selling items based on quantity sold?
3.	What is the rate and volume of returned transactions?
4.	Which countries contribute the highest sales revenue?
5.	How are customers segmented based on Recency, Frequency, and Monetary (RFM) analysis?
6.	What is the distribution of customers across RFM-based customer segments?

## Tools Used
### Python (Pandas, NumPy, Matplotlib, Seaborn):
- Data Cleaning
- Feature Engineering (e.g., TotalPrice, IsReturn flag)
- RFM Calculation and Segmentation

### Tableau:
- Interactive Dashboard Visualization
- Geographical Revenue Mapping
- Sales Trend Analysis
- Customer Segmentation Visualization

## Customer Segmentation (RFM Analysis)
RFM (Recency, Frequency, Monetary) is a widely used method for classifying customers based on their purchasing behavior.
### RFM Metrics Definition

| **Metric**   | **Definition**                                       |
|--------------|------------------------------------------------------|
| **Recency**  | Days since the customer’s last purchase (lower is better) |
| **Frequency**| Total number of purchase transactions               |
| **Monetary** | Total amount spent by the customer                  |

### RFM Scoring Method
Each customer receives a score from 1 (low) to 5 (high) for each RFM dimension:
- Recency (R_Score): Recent buyers get higher scores.
- Frequency (F_Score): Frequent buyers get higher scores.
- Monetary (M_Score): Higher spenders get higher scores.
  
The three scores are then combined into an RFM Segment Code (e.g., “555” = Best Customers).

### Customer Segment Profiles

| **Segment**      | **Profile**                                  |
|------------------|----------------------------------------------|
| Best Customers   | High Recency, Frequency, and Monetary        |
| At Risk          | Low Recency, previously valuable             |
| Big Spenders     | High Monetary, lower Frequency/Recency       |
| Loyal Customers  | High Frequency, moderate Recency and Monetary|
| Others           | Low across all RFM dimensions                |

## Key Insights
![alt text](https://github.com/deaanisaaulia/retail-sales-and-customer-segmentation/blob/main/Dashboard.png)

### 1. Monthly Sales Trends (Revenue and Quantity) 
Sales showed steady growth throughout 2011, with both revenue and quantity sold peaking in November 2011. This suggests a seasonal sales spike, likely due to year-end and holiday shopping behavior.

### 2. Top-Selling Products by Quantity 
Analysis revealed that products like "World War 2 Gliders ASSTD Designs" and "Jumbo Bag Red Retrospot" were among the top 5 best-selling items based on quantity sold.
These are affordable, novelty, and gift-type products, showing customer preference for unique and low-cost items.

### 3. Return Transaction Rate 
Approximately 2.2% of total transactions were identified as returns, based on invoice patterns and negative quantities. This indicates that the majority of customers were satisfied with their purchases, and product issues were minimal.

### 4. Revenue Contribution by Country 
The United Kingdom accounted for over 80% of total revenue, confirming that it is the dominant sales market. Other notable contributors included Germany, France, and the Netherlands, showing potential for regional expansion.

### 5. Customer Segmentation (RFM Analysis) 
Using Recency, Frequency, and Monetary value, customers were segmented into 5 key groups:
- Best Customers (22%): Recent, frequent, and high spenders.
- At Risk (24%): Long time since last purchase, low frequency.
- Loyal Customers (11%): High frequency but moderate recency.
- Big Spenders (6%): High spending customers with varying frequency.
- Others (37%): Low engagement across all metrics.
  
### 6. Customer Segment Distribution 
A significant portion of customers (about 24%) are at risk of churn, while Best Customers represent a smaller but highly valuable group. This shows clear opportunities for both customer retention and reactivation efforts.

## Strategic Recommendations
### 1. Maximize Sales During Seasonal Peaks
Focus inventory planning and promotional campaigns around high-demand months, especially November, to fully capitalize on peak buying behavior.

### 2. Promote Top-Selling Products
Leverage best-selling product categories for future promotions, cross-selling, or product bundling strategies to increase average order value.

### 3. Reduce Churn by Targeting At Risk Customers 
Implement reactivation campaigns (e.g., personalized discounts, reminder emails) aimed at the ‘At Risk’ customer segment to encourage repeat purchases.

### 4. Reward Best and Loyal Customers
Develop loyalty programs, exclusive deals, or early-access sales targeted at ‘Best Customers’ and ‘Loyal Customers’, to retain them and increase lifetime value.

### 5. Expand International Marketing Efforts
Given the revenue contribution from countries outside the UK, consider localized marketing campaigns and country-specific offers in regions like Germany and France.

### 6. Continue Monitoring Return Trends
Although the return rate is low, continue to track and analyze return transactions to identify any emerging quality or fulfillment issues.
