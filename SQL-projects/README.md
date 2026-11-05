# REVENUE DECLINE ANALYSIS

## Overview
NordCart seeks to understand the factors behind a significant decline in revenue and identify opportunities to improve sales performance. This project analyzes e-commerce order and session data to compare Q2 and Q3 performance, with a focus on revenue trends, order volume, customer types, discounts, and sales channels. By examining changes across key business segments and identifying the main contributors to the revenue decline, the analysis provides actionable insights to help stakeholders understand the underlying performance issues and support data-driven decisions for Q4 planning.

# Business Problem
NordCart experienced a significant decline in revenue during Q3 despite an increase in order volume. Understanding the factors behind this decline is important for effective Q4 planning and decision-making.

The objective of this project is to analyze NordCart's sales and session data to identify the key factors contributing to the revenue decline, enabling the business to:

* Identify key drivers of the Q2-to-Q3 revenue decline
* Understand changes in customer purchasing behaviour
* Evaluate revenue performance across sales channels
* Assess the impact of discounts and customer types
* Support data-driven Q4 planning and decision-making

# Dataset Description

The analysis uses three datasets representing NordCart's products, customer sessions, and orders.

* **Products:** Contains product-level information, including product categories, launch dates, active status, and product weight.
* **Sessions:** Contains website session data, including session dates, customer information, traffic channels, countries, session activity, and conversion status.
* **Orders:** Contains transaction-level data, including order dates, customers, products, categories, quantities, prices, discounts, revenue, order status, sales channels, countries, and payment methods.

Together, these datasets provide a view of NordCart's sales performance, customer activity, and revenue trends, enabling comparison between Q2 and Q3 and investigation of the factors contributing to the revenue decline.

# Data Cleaning and Preparation

The datasets were cleaned and prepared to ensure consistency, accuracy, and reliability before analysis. Key preparation steps included:

* Identifying and assessing missing values across the datasets
* Standardising inconsistent categorical values, particularly customer type and order status fields
* Reviewing and handling invalid and negative revenue values
* Converting date fields into appropriate datetime formats
* Creating a quarterly field to enable Q2 and Q3 comparisons
* Reviewing duplicate and inconsistent records
* Preparing the cleaned data for SQL-based exploratory analysis and visualisation

The cleaned datasets were then used for further analysis of revenue, order volume, customer behaviour, discounts, and sales channels.

# Exploratory Data Analysis

The EDA focuses on key revenue trends and performance drivers to understand the factors behind NordCart's Q2-to-Q3 revenue decline.

## Monthly Revenue Trend
The monthly trend shows a sharp decline in revenue beginning in July, with Q3 revenue remaining significantly below the levels observed during the first half of the year.

<img width="884" height="439" alt="image" src="https://github.com/user-attachments/assets/fbb4a7bf-f445-42c7-8438-f18651c4ca19" />

Insight:

Revenue remained relatively stable from January to June, despite some month-to-month fluctuations. A sharp decline occurred in July, with revenue falling by approximately 41.2% from June. Revenue then remained at a significantly lower level through August and September, indicating that the decline began in July and persisted throughout Q3.

## Q2 vs Q3 Performance

<img width="888" height="528" alt="image" src="https://github.com/user-attachments/assets/450c6688-1470-4fbf-93e1-5c7ab0a92316" />

Insight:

The revenue decline was broad-based across all major channels rather than isolated to paid social or email. Paid search experienced the largest percentage decline, while email experienced the smallest, indicating that the problem is unlikely to be attributable to a single acquisition channel.

## Revenue Waterfall by Channel

<img width="869" height="505" alt="image" src="https://github.com/user-attachments/assets/72292987-7062-4212-833c-ba89efab1dd4" />

Insight:

Paid Social and Paid Search together account for about 60.4K of the 167.1K decline, making paid acquisition a particularly important contributor.
But because every channel declined, the evidence points toward a broader deterioration in revenue performance rather than a single-channel failure.

# Recommendations
1. Investigate the broad-based revenue decline across all channels to identify the underlying factor affecting overall customer spending.
2. Review paid acquisition performance, particularly Paid Social and Paid Search, since they contributed the largest individual revenue declines.
3. Assess customer purchasing behaviour to understand why revenue is falling despite order volume remaining relatively strong.
4. Review discounts and refunds to determine whether changes in these areas are reducing net revenue.
5. Monitor channel performance in Q4 with weekly revenue, order volume, AOV, and refund-rate tracking to identify whether the decline is reversing.

# Technologies Used

* Python — Data cleaning, preparation, analysis, and visualisation
* Pandas & NumPy — Data manipulation and numerical analysis
* SQL — Exploratory data analysis and business metric calculations
* Matplotlib — Data visualisation
* Jupyter Notebook — Analysis and documentation
* GitHub — Project version control and presentation

# Conclusion
NordCart experienced a significant 40.20% decline in revenue from Q2 to Q3, falling from 415,576.07 to 248,507.17. The decline occurred across all sales channels, with Paid Social and Paid Search contributing the largest individual revenue losses.

The analysis also shows that the decline was not simply caused by fewer orders, as order volume increased from 2,589 to 2,736. This indicates that the business needs to focus on understanding the factors affecting the value and profitability of those orders, particularly customer purchasing behaviour, discounts, and refunds.

