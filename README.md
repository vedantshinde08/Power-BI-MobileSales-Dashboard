# 📊 Mobile Sales Analysis Dashboard

## 📌 Project Overview

This project presents an interactive **Power BI dashboard** developed to analyze mobile sales performance.

The dashboard provides a consolidated view of key business metrics including **Total Sales, Total Profit, Total Transactions, Total Quantity, and Average Selling Price**.

It also allows users to explore sales performance by **brand, month, city, payment method, and other dimensions**.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Analyze overall mobile sales performance
- Track total sales and profit
- Monitor transaction volume
- Analyze quantity sold
- Compare sales across mobile brands
- Analyze monthly sales trends
- Analyze sales across different locations
- Analyze payment methods
- Provide interactive filtering for business analysis

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **Power Query**
- **DAX**
- **Data Modeling**
- **Data Visualization**

---

## 📊 Key Performance Indicators

The dashboard contains the following KPI cards:

| KPI | Purpose |
|---|---|
| Total Profit | Measures overall profit generated |
| Total Sales | Measures overall sales value |
| Total Transactions | Measures transaction volume |
| Total Quantity | Measures units sold |
| Average Selling Price | Measures average selling price |

---

## 🎛️ Dashboard Filters

Interactive slicers are provided for dimensions such as:

- Brand
- Month
- City
- Payment Method

These filters allow users to dynamically explore the dashboard.

---

## 📈 Dashboard Visualizations

### Monthly Sales Trend

A time-based visualization is used to analyze how mobile sales change across months.

### Geographic Analysis

A map visualization is used to analyze sales across different locations.

### Brand Analysis

Sales performance is compared across different mobile brands.

### Payment Method Analysis

The dashboard provides a breakdown of sales based on payment methods.

---

## 🧹 Data Preparation

The dataset was prepared using **Power Query** before creating the dashboard.

The data preparation process includes data cleaning, transformation, data type handling, and creation of fields required for analysis.

Detailed transformation steps will be documented as part of this project.

---

## 🧮 DAX Measures

DAX measures were created to calculate the key business metrics used in the dashboard.

The actual DAX formulas and explanations will be documented separately based on the measures created in the Power BI project.

---

## 🖼️ Dashboard Preview

![Mobile Sales Dashboard](Mobile_sales_dashboard.png.png)

---

## 🔄 Project Workflow

```text
Raw Sales Data
↓
Power Query
↓
Data Cleaning & Transformation
↓
Data Model
↓
DAX Measures
↓
Power BI Visualizations
↓
Interactive Dashboard
↓
Business Insights

## 🧮 DAX Measures

DAX (Data Analysis Expressions) was used to create measures for the key business metrics displayed in the dashboard.

### 1. Total Sales

```DAX
TOTAL SALES =
SUMX(
Sales,
Sales[Quantity] * Sales[Selling Price]
)

### 2. Total Profit

Total Profit =
SUMX(
Sales,
(Sales[Selling Price ] - Sales[Cost Price] * Sales[Quantity]

### 3. Total Transactions

Total Transactions =
COUNTROWS(Sales)

### 4. Total Quantity

Total Quantity =
SUM(Sales[Quantity]}

### 5. Average Selling Price

Average Selling Price =
DIVIDE(
[TOTAL SALES],
[TOTAL QUANTITY]
)
---

## 📊 Dashboard Visualizations

The dashboard contains interactive KPI cards, filters, and visualizations to analyze mobile sales performance from different perspectives.

### 1. KPI Cards

Five KPI cards are used to provide a quick summary of the overall sales performance:

- **Total Profit** – Shows the total profit generated from mobile sales.
- **Total Sales** – Shows the total sales revenue generated.
- **Total Transactions** – Shows the total number of sales transactions.
- **Total Quantity** – Shows the total number of mobile units sold.
- **Average Selling Price** – Shows the average selling price per mobile unit.

### 2. Sales by Month

A **Line Chart** is used to display total sales across different months.

**Purpose:**
To identify changes and trends in sales performance over time.

### 3. Sales by City

A **Map Visualization** is used to display total sales across different cities.

**Purpose:**
To understand the geographical distribution of mobile sales.

### 4. Sales by Brand

A **Bar Chart** is used to compare total sales across different mobile brands.

**Purpose:**
To identify differences in sales performance among brands.

### 5. Sales by Payment Method

A **Donut Chart** is used to show the distribution of sales across different payment methods.

**Purpose:**
To understand customer payment preferences.

### 6. Sales by Mobile Model

A **Bar Chart** is used to compare sales performance across different mobile models.

**Purpose:**
To identify which mobile models contribute to overall sales.

---

## 🎛️ Interactive Filters

The dashboard includes interactive slicers that allow users to filter the analysis dynamically.

- **Brand** – Filter the dashboard by mobile brand.
- **Month** – Analyze sales for a selected month.
- **City** – Analyze sales for a specific city.
- **Payment Method** – Analyze sales based on the selected payment method.

The KPI cards and visualizations update dynamically when filters are applied.

