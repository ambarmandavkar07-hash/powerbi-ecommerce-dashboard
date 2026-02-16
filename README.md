# 📊 Power BI E-Commerce Performance Dashboard

## 📌 Project Overview

This project presents an end-to-end Power BI dashboard built to analyze operational and sales performance for an e-commerce grocery platform (Swiggy Instamart).

The dashboard transforms raw transactional data into actionable business insights covering:

- Revenue performance
- Order trends
- Delivery efficiency
- Discount impact
- Product category analysis

The objective was to demonstrate real-world data analysis using Power BI, DAX, and business KPI design.

---

## 🧾 Dataset Description

The original dataset contained multiple companies and a large volume of records.

For focused analysis and performance optimization:

- Only **Swiggy Instamart** data was used
- Final dataset size: ~11,000 rows
- Total columns: 15
- Data structure: Single fact table (flat model)

### Key Columns

| Column Name | Description |
|-------------|------------|
| Order ID | Unique order identifier |
| Company | Service provider |
| City | Customer location |
| Customer Age | Age of customer |
| Order Value | Gross order amount |
| Net Revenue | Revenue after discount (calculated) |
| Product Category | Product classification |
| Items Count | Number of items in order |
| Delivery Time (min) | Delivery duration |
| Delivery Status | On Time / Late (calculated) |
| Payment Method | Mode of payment |
| Discount Applied | Yes/No flag |
| Customer Rating | Rating given by customer |

---

## 🔗 Data Model

- Single fact table structure
- No separate dimension tables
- Designed for simplicity and fast performance
- Can be converted to star schema in future

---

## 🧮 DAX Calculations Implemented

### Calculated Columns

**Net Revenue**
*Delivery Status*

### Measures Created

- Total Revenue
- Net Revenue
- Total Orders
- Average Order Value
- On-Time Orders
- Late Orders
- Discounted Orders
- Average Delivery Time

---

## 📊 Dashboard Structure

### 🏠 Home Page
High-level KPIs and navigation overview.

### 📈 Sales Overview
- Total Revenue
- Net Revenue
- Revenue by City
- Revenue by Product Category
- Orders by Payment Method

### 🚚 Delivery Performance Dashboard
- On-Time vs Late Orders
- Average Delivery Time by City
- Map Visualization (City-wise performance)
- Delivery Status Distribution

### 📦 Product & Discount Insights
- Orders by Product Category
- Average Order Value by Category
- Discount Impact Analysis
- Category Summary Table

---

## 📸 Dashboard Screenshots

Screenshots are available in the `/screenshots` folder:

- Home Page
- <img width="1308" height="733" alt="Screenshot 2026-02-16 143012" src="https://github.com/user-attachments/assets/cae7e8b7-0537-4429-bf7c-bf80578ef856" />

-Sales Overview
-<img width="1306" height="733" alt="Screenshot 2026-02-16 143057" src="https://github.com/user-attachments/assets/f740929a-fa73-4573-956f-13933ecb4e24" />

-  Delivery Performance
-<img width="1308" height="738" alt="Screenshot 2026-02-16 143125" src="https://github.com/user-attachments/assets/e6c83138-7ab3-43bc-8a78-df34a97872dd" />

-  Product & Discount Insights
<img width="1310" height="741" alt="Screenshot 2026-02-16 143158" src="https://github.com/user-attachments/assets/13b94eb3-88e5-4f8c-a4f8-70c8e20a0c6c" />

---

## 📌 Key Business Insights

- Major cities contribute the highest revenue
- Grocery and household categories dominate sales
- Discounts increase order volume but reduce net revenue
- Longer delivery distances increase late deliveries
- Faster delivery correlates with better customer ratings

---

## 🛠 Tools & Technologies

- Power BI Desktop
- DAX
- Excel (Data Cleaning)
- GitHub (Project Documentation)

---

## 🎯 Project Outcomes

This project demonstrates:

- Data cleaning and preparation
- Business KPI development using DAX
- Dashboard design and visualization
- Operational and financial performance analysis
- Business insight generation

---

## 🚀 How to Use

1. Download the `.pbix` file from the repository.
2. Open using Power BI Desktop.
3. Explore interactive dashboards using slicers and filters.

---

## 👤 Author Ambar Mandavkar
