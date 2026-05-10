# 🍔 Swiggy Hyderabad Sales Dashboard — Power BI

> An end-to-end interactive Power BI dashboard analyzing Swiggy food delivery orders across Hyderabad for the year 2024 — covering sales trends, delivery patterns, cuisine preferences, and customer behavior.

---

## 📊 Dashboard Preview

![Dashboard Screenshot](screenshot.png)

---

## 🖥️ How to View This Dashboard

> 📥 **Download** [`dashboard.pbix`](./dashboard.pbix) from this repo
> 🔓 Open it with **[Power BI Desktop](https://powerbi.microsoft.com/desktop/)** ← Free to download
> 🎛️ Explore filters, slicers, and all interactive visuals locally

> **Note:** Power BI Service (online publishing) requires a Pro license. Use Power BI Desktop (free) to view this report.

---

## 🧾 About the Project

### Background

Swiggy is one of India's leading online food delivery platforms. Hyderabad, being one of the most active metro cities for food delivery, offers rich data insights into consumer ordering behavior, peak demand windows, and restaurant performance.

This project analyzes **100 real-world Swiggy orders** from Hyderabad spanning the year **2024**. The goal was to go beyond raw data — by building a clean, visually compelling Power BI report that helps identify sales patterns, high-performing areas, and customer trends.

---

### 🎯 Objectives

- Analyze **monthly and quarterly sales trends** to identify peak periods
- Understand **which areas in Hyderabad** generate the most order value
- Break down **payment mode preferences** among customers
- Study **meal period patterns** — when do people order the most?
- Track **key KPIs** like Total Orders, Total Revenue, and Average Delivery Time
- Build an interactive, filterable dashboard suitable for business storytelling

---

### 📐 Dashboard Pages

#### Page 1 — Sales Overview
The main dashboard page contains all high-level KPIs and visual breakdowns:

| Visual | Description |
|--------|-------------|
| **KPI Cards** | Total Orders (100), Total Revenue (₹132K), Avg Delivery Time (25.06 min) |
| **Monthly Sales Trend** | Line/area chart showing order volume across all 12 months |
| **Payment Mode Distribution** | Donut chart breaking down UPI, Debit Card, Swiggy Wallet, Cash on Delivery, Credit Card |
| **Order Value by Area** | Horizontal bar chart showing avg order value per delivery area, split by Quarter (Q1–Q4) |
| **Total Orders by Meal Period** | Bar chart showing volume across Morning, Afternoon, Evening, Night, Late Night |

#### Page 2 — Deep Dive Analysis
Detailed breakdown by cuisine type, restaurant performance, discount analysis, and customer ratings.

---

### 📌 Key Insights

| # | Insight |
|---|---------|
| 1 | **Biryani** dominates as the top cuisine — consistent across all delivery areas |
| 2 | **August** records the highest monthly order volume; orders decline steadily toward year-end |
| 3 | **Q4** shows strongest order value in premium areas like Jubilee Hills and Banjara Hills |
| 4 | **UPI (23%)** is the most preferred payment mode, followed by Debit Card (22%) and Cash on Delivery (20%) |
| 5 | **Jubilee Hills** leads in average order value across all quarters |
| 6 | **Late Night and Night** slots are the busiest meal periods for Swiggy orders |
| 7 | Orders with **20% discount** drive the highest quantity uplift — discounts significantly boost volume |
| 8 | **Average Delivery Time** is just ~25 minutes — indicating strong delivery efficiency in Hyderabad |
| 9 | **Gachibowli and KPHB** show consistently high Q2 order values, suggesting tech-worker demand |
| 10 | **Customer Ratings** are highest for Biryani and South Indian cuisine restaurants |

---

### 🗺️ Areas Covered

The dashboard covers **8 major delivery zones** in Hyderabad:

`Begumpet` · `Jubilee Hills` · `Banjara Hills` · `Ameerpet` · `KPHB` · `Gachibowli` · `Charminar` · `Secunderabad`

---

## 📁 Project Structure

```
swiggy-hyd-sales-dashboard/
│
├── README.md          ← Project overview, insights & documentation
├── dashboard.pbix     ← Power BI report file (open with Power BI Desktop)
├── screenshot.png     ← Dashboard preview image
└── data/
    └── sales_data.csv ← Dataset used (100 orders, Hyderabad 2024)
```

---

## 🗂️ Dataset Overview

- **File:** `data/sales_data.csv`
- **Source:** Swiggy Hyderabad order data (2024)
- **Records:** 100 orders
- **Time Period:** January 2024 – December 2024

| Column | Description |
|--------|-------------|
| `Order_ID` | Unique order identifier (SWG prefix) |
| `Order_Date` | Date of order placement |
| `Month / Quarter / Day_of_Week` | Time dimensions for trend analysis |
| `Time_Slot` | Order time bucket (Breakfast, Lunch, Dinner, Late Night) |
| `Restaurant_Name` | Name of the restaurant |
| `Cuisine_Type` | Food category (Biryani, Chinese, South Indian, etc.) |
| `Restaurant_Area` | Area where restaurant is located |
| `Delivery_Area` | Area where order was delivered |
| `Quantity` | Number of items ordered |
| `Unit_Price_INR` | Price per item in INR |
| `Gross_Amount_INR` | Total before discount |
| `Discount_Percent / Amount` | Discount applied on the order |
| `Delivery_Fee_INR` | Delivery charges |
| `Net_Amount_INR` | Final amount paid by customer |
| `Payment_Mode` | UPI / Debit Card / Swiggy Wallet / Cash on Delivery / Credit Card |
| `Order_Status` | Delivered / Cancelled |
| `Delivery_Time_Min` | Time taken to deliver (in minutes) |
| `Customer_Rating` | Rating given by customer (scale: 1–5) |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard design, DAX measures, data modeling |
| **Microsoft Excel** | Raw data cleaning and preparation |
| **Power Query** | Data transformation within Power BI |
| **DAX** | Custom KPI calculations (Revenue, Avg Delivery Time, etc.) |
| **PowerShell** | Data pipeline & file conversion |

---

## 👤 Author

**Prashanth Gajula**
[GitHub](https://github.com/prashanthgajula08-dot) | [LinkedIn](https://linkedin.com/in/prashanthgajula)

---

*Built as part of a Data Analytics portfolio — showcasing end-to-end Power BI dashboard development from raw data to business insights.*
