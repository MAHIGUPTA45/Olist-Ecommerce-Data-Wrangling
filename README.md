**📊 Olist E-Commerce Data Immersion & Wrangling**

**📌 Project Overview**

This project focuses on data acquisition, cleaning, transformation, and preparation of the Olist Brazilian E-Commerce dataset.

The objective was to transform raw multi-table transactional data into an analysis-ready master dataset suitable for business intelligence and KPI development.

**🎯 Objectives**

Clean and standardize raw order data

Handle missing values logically

Convert timestamp columns to proper datetime format

Engineer time-based and logistics-related features

Merge multi-table dataset into a unified master dataset

Create revenue-ready dataset for future EDA and dashboarding

**📂 Dataset Used**

Olist Brazilian E-Commerce Public Dataset

Key tables used:

olist_orders_dataset

olist_order_items_dataset

**🛠 Data Cleaning & Preparation Steps**

1️⃣ Datetime Conversion

Converted all order-related timestamp columns from object to datetime64.

2️⃣ Missing Value Analysis

Identified missing delivery timestamps.

Verified missing values correspond to non-delivered orders.

Avoided incorrect row deletion.

3️⃣ Duplicate Check

Confirmed zero duplicate rows in orders table.

4️⃣ Feature Engineering

Created the following engineered features:

purchase_year

purchase_month

purchase_day

purchase_weekday

delivery_days

estimated_delivery_days

delivery_delay

total_revenue

5️⃣ Multi-Table Merge

Merged orders and order_items tables using order_id.

Removed inconsistent merged rows (<1% of data).

**📊 Engineered Business Metrics**

Actual delivery duration

Estimated delivery duration

Delivery delay metric

Total revenue per item

These metrics prepare the dataset for:

Logistics performance analysis

Sales trend analysis

Revenue reporting

Time-series exploration
