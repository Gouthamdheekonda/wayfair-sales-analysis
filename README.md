# Wayfair Sales Analysis

## Project Overview

This project analyzes Wayfair sales data to understand revenue trends, product category performance, seasonality, and order outcomes. The goal is to identify useful business insights and recommend actions to improve sales performance.

## Objectives

* Clean and prepare the provided sales datasets.
* Calculate net merchandise revenue for completed orders.
* Analyze monthly sales trends and compare 2025 with 2024.
* Identify seasonal sales patterns.
* Evaluate product category performance.
* Examine returned and canceled orders.
* Calculate average order value (AOV).
* Present findings and actionable recommendations.

## Tools and Technologies

* Python
* Pandas
* Matplotlib
* Jupyter Notebook

## Datasets

The project uses four datasets:

* `orders.csv`
* `order_items.csv`
* `products.csv`
* `customers.csv`

## Data Cleaning and Preparation

* Removed duplicate order records.
* Standardized product category values.
* Checked missing values and data consistency.
* Combined the datasets using appropriate joins.
* Calculated gross item amounts, net item revenue, and estimated item profit.

## Key Findings

1. **Revenue growth:** Completed-order net item revenue increased from $841,136.33 in 2024 to $1,016,984.67 in 2025, representing approximately 20.91% growth.
2. **Category performance:** Furniture generated the highest net item revenue at $318,593.13, while Kitchen had the highest quantity sold at 3,630 units.
3. **Seasonality:** November had the highest average monthly revenue across the analyzed years, at approximately $113,479.07.

## Recommendations

1. Investigate the performance of the Bath category to identify opportunities to improve revenue.
2. Prepare inventory and operational capacity for the potential increase in demand during November.

## Visualizations

The following charts illustrate the key findings from the sales analysis:

* **Monthly Revenue Trends:** `monthly_revenue_trend.png`
* **Monthly Seasonality:** `monthly_seasonality.png`
* **Revenue by Product Category:** `category_revenue.png`


## Important Notes

* Revenue calculations include completed-order items with valid unit prices.
* Completed-order items with missing unit prices are excluded from the revenue calculation.
* Estimated item profit is calculated using item revenue and item costs; it does not include operating expenses.

## Project Structure

```text
Wayfair Sales Analysis/
├── data/
│   └── raw/
├── notebooks/
│   └── 01_Data_Inspection_and_Cleaning.ipynb
├── charts/
│   ├── monthly_seasonality.png
│   ├── monthly_revenue_trend.png
│   └── category_revenue.png
└── README.md
```

## Conclusion

This analysis highlights revenue growth, differences in product category performance, and a potential seasonal sales peak. These findings can help guide further investigation into category performance and seasonal planning.
