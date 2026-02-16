📊 Power BI E-Commerce Performance Dashboard
📌 Project Overview
This project presents an end-to-end Power BI dashboard built to analyze operational and sales performance for an e-commerce grocery platform (Swiggy Instamart).
The dashboard converts raw transactional data into business insights covering:
• Revenue growth
• Order behavior
• Delivery efficiency
• Discount impact
• Product performance
The goal is to demonstrate real-world data analysis using Power BI, DAX, and data modeling.
🧾 Dataset Description
The original dataset contained multiple companies and a very large volume of records.
For performance optimization and focused analysis:
✅ Only Swiggy Instamart data was used
✅ Final working dataset contains ~11,000 rows
✅ Single fact table structure
Main Columns Used:
Column Name
Description
Order ID
Unique order identifier
Company
Service provider
City
Customer city
Customer Age
Age of customer
Order Value
Order amount
Net Revenue
Revenue after discount (calculated)
Product Category
Product group
Items Count
Number of items
Delivery Time (min)
Delivery duration
Delivery Status
On Time / Late (calculated)
Payment Method
Payment type
Discount Applied
Yes/No
Customer Rating
Order rating
🔗 Data Model
• Single-table star structure (fact table only)
• Optimized for beginner-friendly and fast performance
• Calculated columns and measures created using DAX
🧮 DAX Calculations Implemented
Net Revenue (Calculated Column)
DAX
Copy code
Net Revenue = 
IF(
    'dataset'[Discount Applied] = 1,
    'dataset'[Order Value] * 0.9,
    'dataset'[Order Value]
)
Delivery Status (Calculated Column)
DAX
Copy code
Delivery Status = 
IF(
    'dataset'[Delivery Time (min)] <= 20,
    "On Time",
    "Late"
)
KPI Measures
Total Revenue
Net Revenue
Total Orders
Average Order Value
On-Time Orders
Late Orders
Discounted Orders
📊 Dashboard Structure
🏠 Home Page
High-level KPIs and navigation
📈 Sales Overview
Revenue by city
Revenue by product category
Payment method distribution
🚚 Delivery Performance
On-time vs late deliveries
Delivery time trend
City-wise delivery performance
Geographic revenue map
📦 Product & Discount Insights
Orders by category
Average order value by category
Discount impact on revenue
📸 Visuals Included
All dashboard screenshots are available in the /screenshots folder:
Home Page
<img width="1308" height="733" alt="Screenshot 2026-02-16 143012" src="https://github.com/user-attachments/assets/67c8efa3-d623-43d6-a97a-cab8e50181a9" />
Sales Overview
<img width="1306" height="733" alt="Screenshot 2026-02-16 143057" src="https://github.com/user-attachments/assets/a39070b1-ac71-43e6-9a7a-b728d67dcbfd" />
Delivery Performance
<img width="1308" height="738" alt="Screenshot 2026-02-16 143125" src="https://github.com/user-attachments/assets/0b386ab9-5506-4362-aecc-0d31c9c7f823" />
Product Insights
<img width="1310" height="741" alt="Screenshot 2026-02-16 143158" src="https://github.com/user-attachments/assets/097e533a-1d52-4a38-acb9-3a2d2b0ec7bf" />
