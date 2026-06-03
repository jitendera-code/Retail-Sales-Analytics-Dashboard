# Retail Sales Analytics Dashboard

## Project Overview

Retail businesses generate large volumes of transactional data across products, customers, promotions, and locations. However, raw sales data alone does not provide meaningful insights for decision-making.

This project develops an end-to-end Retail Sales Analytics Dashboard in Power BI to analyze sales performance, product profitability, promotion effectiveness, and geographical revenue distribution. The dashboard enables business users to identify revenue-driving products, evaluate promotional campaigns, monitor sales trends, and support data-driven decision-making.

---

# Business Problem

Management wants answers to the following questions:

* Which products generate the highest and lowest revenue?
* Which products contribute the most profit?
* How do sales trends change over time?
* Which promotional campaigns are most effective?
* Which cities contribute the highest revenue?
* How many orders are being generated?
* How do discounts impact overall revenue performance?

Without a centralized reporting solution, answering these questions requires manual analysis and significant effort.

---

# Project Objectives

The objectives of this project were:

1. Analyze product performance using sales, profit, and quantity sold.
2. Monitor revenue trends across time periods.
3. Evaluate promotion effectiveness and discount impact.
4. Identify top revenue-contributing cities.
5. Build an interactive dashboard that allows users to filter and explore data dynamically.
6. Create a scalable data model using star schema principles.

---

# Project Scope

### In Scope

* Sales Analysis
* Product Performance Analysis
* Profit Analysis
* Promotion Analysis
* Geographic Revenue Analysis
* Interactive Reporting

### Out of Scope

* Inventory Management
* Customer Churn Prediction
* Forecasting Models
* Machine Learning

### Data Granularity

Transaction-Level Data

Each row represents an individual sales transaction.

### Date Range

2020 – 2024

---

# Tools & Technologies

| Tool                 | Purpose                         |
| -------------------- | ------------------------------- |
| Power BI             | Dashboard Development           |
| Power Query          | Data Cleaning & Transformation  |
| DAX                  | Business Metrics & Calculations |
| Excel                | Source Dataset                  |
| Star Schema Modeling | Data Model Design               |

---

# Data Workflow

Raw Excel Data
↓
Power Query Cleaning
↓
Data Transformation
↓
Star Schema Data Modeling
↓
DAX Calculations
↓
Dashboard Development
↓
Business Insights

---

# Data Model

The project follows a Star Schema design.

### Fact Table

Fact Sales

Contains transactional information:

* Order ID
* Customer ID
* Product ID
* Promotion ID
* Units Sold
* Total Sales
* Discount
* Net Sales
* Profit

### Dimension Tables

#### Dim Customer

* Customer ID
* Customer Name
* City
* State
* Email ID

#### Dim Product

* Product ID
* Product Name
* Product Line
* Price Per Unit

#### Dim Promotion

* Promotion ID
* Promotion Name
* Ad Type
* Coupon Code
* Discount Percentage

#### Date Dimension

Created using CALENDARAUTO() to support time intelligence and trend analysis.

---

# Data Preparation

The following transformations were performed using Power Query:

* Data type corrections
* Column renaming
* Removing unnecessary columns
* Creating conditional columns
* Handling missing values
* Data validation
* Table relationships setup

### Derived Columns

#### Total Sales

Total Sales = Units Sold × Price Per Unit

#### Discount

Calculated using promotion discount percentages.

#### Net Sales

Net Sales = Total Sales − Discount

#### Profit

Profit = Net Sales × 10%

(Note: Profit margin is assumed because product cost information was not available in the dataset.)

---

# Dashboard Pages

## 1. Executive Overview

Provides a high-level summary of business performance.

### KPIs

* Total Revenue
* Average Discount %
* Total Orders

### Analysis

* Monthly Revenue Trend
* Promotion Performance
* Revenue by City

---

## 2. Product & Category Analysis

Provides detailed product-level insights.

### Analysis

* Top Revenue Products
* Product Profitability
* Revenue by Product Category
* Profit by Product Category

---

## 3. Transaction Explorer

Provides transaction-level visibility.

### Interactive Filters

* Date
* Product Name
* Customer Name
* Promotion Name

### Metrics

* Sales
* Discount
* Net Sales
* Profit
* Units Sold

---

# Key Metrics

### Revenue

Represents actual revenue generated after discounts.

Revenue = Net Sales

### Profit

Estimated profitability of transactions.

### Units Sold

Measures sales volume.

### Average Discount %

Measures promotional intensity.

### Total Orders

Tracks overall transaction activity.

---

# Key Findings

### Product Performance

* Apple iPhone 14 generated the highest revenue.
* Apple MacBook Air and Sony Bravia TV were also major revenue contributors.
* Electronics dominated overall sales performance.

### Category Performance

* Electronics generated significantly more revenue than other categories.
* Personal Care and Kitchenware contributed the lowest revenue.

### Promotion Analysis

* Weekend Flash Sale offered the highest average discount.
* Clearance Sale was the second most aggressive promotion strategy.

### Geographic Insights

* Bhopal generated the highest revenue.
* Kanpur and Indore were also major contributors.
* Bangalore contributed the lowest revenue among analyzed cities.

### Revenue Trends

* Revenue recovered strongly after a weaker spring period.
* Sales peaked during October and November.

---

# Business Recommendations

### Product Strategy

Increase inventory availability for high-performing Electronics products.

### Promotion Strategy

Evaluate the ROI of highly discounted campaigns such as Weekend Flash Sale and Clearance Sale.

### Geographic Expansion

Investigate opportunities in top-performing cities such as Bhopal, Kanpur, and Indore.

### Category Improvement

Develop targeted campaigns for underperforming categories such as Personal Care and Kitchenware.

---

# Assumptions & Limitations

### Assumptions

* Profit margin assumed at 10%.
* Promotion discounts mapped through business rules.

### Limitations

* No product cost data available.
* No inventory information.
* No customer demographics.
* No forecasting included.

---

# Deliverables

* Power BI Dashboard (.pbix)
* Cleaned Data Model
* DAX Measures
* Business Insights Report
* GitHub Documentation

---

# Future Enhancements

* Profit Margin Analysis using actual cost data
* Customer Segmentation
* Sales Forecasting
* Customer Lifetime Value Analysis
* Geographic Mapping Dashboard

---

# Author

Jitender Yadav

Aspiring Data Analyst

Tools: Excel | SQL | Power BI | Statistics

---

# Last Updated

June 2026

