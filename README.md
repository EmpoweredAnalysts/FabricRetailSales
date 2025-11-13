# Retail Sales Repository

This repository contains a synthetic retail dataset and supporting notebooks/scripts used to demonstrate an end-to-end data analytics and machine learning workflow involving data exploration, linear regression modelling, experiment tracking, and dashboard reporting. The supporting notebook is designed for use in Microsoft Fabric.

###  Background: The Retail Company

A mid-sized national retail chain, Northstar Retail, operates 40 stores across a variety of urban and suburban regions. Over the past two years, the company has increased its digital advertising investment and expanded its in-store promotional activity.

Leadership wants to understand which operational and marketing factors drive monthly store sales performance, and how these drivers vary across stores and seasons.

To support better decision-making, Northstar Retail is building a predictive model aimed at:

1. Optimising advertising spend allocation
2. Improving promotion planning
3. Supporting staffing and inventory decisions
4. Giving leadership teams clear visibility into the key drivers of sales performance

The dataset in this repository is designed for training, experimentation, and demonstration purposes.

###  Dataset Overview
The dataset contains 960 rows, representing 40 stores over 24 months (store-month grain).
It is fully synthetic and reflects realistic retail behaviour, including:

1. Seasonality
2. Promotion effects
3. Variability in store demographics and competition
4. Operational differences such as staffing and inventory availability


This dataset supports:

Linear regression modelling
Exploratory data analysis
Feature engineering
Experiment tracking
Dashboard visualisation
General data science education

#### Intended Use of the Data 

Northstar Retail aims to:

1. Predict monthly store sales using a regression model.
2. Identify the strongest drivers of revenue, including advertising spend, traffic, pricing, and promotions.
3. Iterate on different feature sets and modelling approaches to improve accuracy.
4. Visualise insights for business partners in dashboards or reports.
5. Build a foundation for future modelling work such as promotion optimisation and demand forecasting.

#### Data Dictionary (also available as a CSV file in the repository)

| Field Name                 | Description |
|----------------------------|-------------|
| `store_id`                 | Unique identifier for each store (1–40). |
| `year`                     | Calendar year of the record. |
| `month`                    | Calendar month of the record (1–12). |
| `month_index`             | Numeric month index used for capturing seasonality (1–12). |
| `is_holiday_month`        | Indicates whether the month is part of the holiday season (1 = November/December, 0 otherwise). |
| `ad_spend`                | Monthly advertising expenditure. |
| `foot_traffic`            | Estimated number of customer visits to the store during the month. |
| `avg_price`               | Average unit price of items sold. |
| `staff_count`             | Number of employees assigned to the store during the month. |
| `store_size_sqft`         | Total size of the store in square feet. |
| `promo_days`              | Number of promotional days held during the month. |
| `competitors_within_3km`  | Number of competing stores within a 3 km radius. |
| `inventory_fill_rate`     | Proportion of SKUs in stock (0 to 1). |
| `returns_rate`            | Proportion of sales returned by customers (0 to 1). |
| `local_income_index`      | Local income indicator where 100 represents the national average. |
| `parking_spaces`          | Number of customer parking spaces available. |
| `store_age_years`         | Age of the store in years. |
| `monthly_sales`           | Total sales revenue for the store in that month (dependent variable). |
