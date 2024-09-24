# Car Sales Dashboard - Power BI Project

## Overview
This project focuses on building an interactive and dynamic **Car Sales Dashboard** in **Power BI** for a car dealership. The aim is to enhance sales tracking and analysis by visualizing key performance indicators (KPIs) and gaining insights into sales trends, all contributing to informed decision-making.

## Project Objective
The goal of this project is to design and develop a user-friendly dashboard that tracks critical sales metrics such as total sales, cars sold, and average pricing, helping the company optimize its sales strategies and performance across different metrics.

## Key Features
The dashboard provides a comprehensive view of car sales with the following key metrics:

1. **Total Sales** – Analyze YTD, MTD, and YoY growth.
2. **Cars Sold** – Track the number of cars sold, compared to previous periods.
3. **Average Price** – Monitor trends in the average price of cars sold.

---

## Problem Statement 1: KPI Requirements
### Sales Metrics:
- **YTD (Year-to-Date) Total Sales**
- **MTD (Month-to-Date) Total Sales**
- **YoY (Year-over-Year) Growth in Total Sales**
- **Comparison of YTD vs. Previous Year YTD (PTYD) Sales**

### Average Price Metrics:
- **YTD Average Price**
- **MTD Average Price**
- **YoY Growth in Average Price**
- **Comparison of YTD Average Price vs. PTYD Average Price**

### Cars Sold Metrics:
- **YTD Cars Sold**
- **MTD Cars Sold**
- **YoY Growth in Cars Sold**
- **Comparison of YTD Cars Sold vs. PTYD Cars Sold**

---

## Problem Statement 2: Visualization Requirements
The dashboard requires several visualizations to help monitor the metrics mentioned above:

1. **Weekly YTD Sales Trend:** Display a line chart showing the YTD sales trend on a weekly basis.
2. **Sales by Body Style:** A pie chart illustrating sales distribution based on car body styles.
3. **Sales by Color:** Another pie chart visualizing sales breakdown by car colors.
4. **Cars Sold by Region:** Use a map chart to display car sales distributed across different regions.
5. **Company-Wise Sales Table:** A tabular view showcasing the sales trend of different car manufacturers.
6. **Detailed Sales Grid:** A data grid listing each sale's information, including car model, body style, color, sales amount, dealer region, and date.

---

## Data Sources
### Car Sales Data:
- **Car ID**
- **Date**
- **Customer Details** (Name, Gender, Annual Income)
- **Dealer Info** (Dealer Name, Number, Region)
- **Car Specs** (Company, Model, Engine, Transmission, Color, Body Style)
- **Price** in dollars

### Calendar Data:
- **Date** (linked to the sales data)
- **Month**
- **Week**
- **Year**

---

## Dashboard Features
1. **Sales Overview:**
   - **YTD Total Sales:** $371.2M
     - Formula: `SUM('Car Data'[Total Sales])`
   - **MTD Total Sales:** $54.28M
     - Formula: `CALCULATE(SUM('Car Data'[Total Sales]), DATESMTD('Calendar'[Date]))`
   - **YoY Growth in Sales:** 23.6%
     - Formula: `[Sales Difference]/[PTYD Total Sales]`
   - **Difference between YTD and PTYD Sales:** $70.8M

2. **Average Price Overview:**
   - **YTD Average Price:** $28.0k
     - Formula: `TOTALYTD([Avg Price],'Calendar'[Date])`
   - **MTD Average Price:** $28.26k
     - Formula: `TOTALMTD([Avg Price],'Calendar'[Date])`
   - **YoY Growth in Average Price:** -0.79%
     - Formula: `[Avg Price Difference]/[PTYD Avg Price]`
   - **Difference between YTD and PTYD Average Price:** $0.22k loss

3. **Cars Sold Metrics:**
   - **YTD Cars Sold:** 13.3K
     - Formula: `SUM('Car Data'[Cars Sold])`
   - **MTD Cars Sold:** 1.92k
     - Formula: `CALCULATE(SUM('Car Data'[Cars Sold]), DATESMTD('Calendar'[Date]))`
   - **YoY Growth in Cars Sold:** 19.73%
     - Formula: `[Cars Sold Difference]/[PTYD Cars Sold]`
   - **Difference between YTD and PTYD Cars Sold:** 3K

---

## Dashboard Visualization

![Car Sales Dashboard](https://github.com/GirishChowdary0208/Powerbi/assets/92716279/a39d22f2-eff5-400d-b99d-7c5f2efcc165)

This interactive dashboard empowers stakeholders to drill into the data, identify patterns, and optimize sales strategies accordingly.

--- 

Feel free to reach out for additional insights or further dashboard customization.
