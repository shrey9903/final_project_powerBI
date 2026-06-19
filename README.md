📊 Sales Performance Analytics Dashboard - Power BI
📌 Project Overview

The Sales Performance Analytics Dashboard is an end-to-end Power BI solution designed to analyze business performance across sales, customers, products, returns, and regions.

This project demonstrates advanced Power BI concepts including:

Data Modeling
DAX Measures & Calculated Columns
Time Intelligence
Interactive Dashboards
Drillthrough Analysis
Row Level Security (RLS)
Mobile Layout Optimization

The dashboard enables stakeholders to monitor KPIs, identify trends, evaluate customer behavior, and make data-driven business decisions.

🎯 Project Objectives
Analyze sales performance across different regions and categories.
Track customer activity and purchasing behavior.
Identify top-performing products and customers.
Monitor product returns.
Implement interactive filtering and drillthrough analysis.
Demonstrate advanced Power BI development techniques.
🗂 Dataset Structure
Fact Tables
Table	Description
Sales_Fact	Transactional sales data
Returns_Fact	Product return records
Dimension Tables
Table	Description
Customer_Dim	Customer information
Product_Dim	Product details
Date_Dim	Date hierarchy
Region_Dim	Regional segmentation
🏗 Data Model

The project follows a Star Schema Architecture.

                Customer_Dim
                       |
                       |
Product_Dim ---- Sales_Fact ---- Date_Dim
                       |
                       |
                 Returns_Fact
                       |
                       |
                 Region_Dim
Features
Primary & Foreign Key Relationships
Single Direction Filtering
Optimized Star Schema Design
Hidden Technical Columns
📈 DAX Measures Implemented
Core Measures
Total Sales
Total Units Sold
Total Returns
Average Sales
Customer Count
Revenue
Time Intelligence
Sales YTD
Previous Year Sales
YOY Growth %
Previous Month Sales
MOM Growth %
KPI Measures
Sales KPI Classification
Sales Percentage of Total
High Sales Orders
🧮 Calculated Columns
Customer Full Name
Full Name =
Customer_Dim[FirstName] &
" " &
Customer_Dim[LastName]
Year-Month
YearMonth =
FORMAT(Date_Dim[Date],"YYYY-MM")
Profit Margin Classification
Profit Margin Class =
SWITCH(
TRUE(),
Sales_Fact[TotalAmount] >= 1000,"High",
Sales_Fact[TotalAmount] >= 500,"Medium",
"Low"
)
📊 Dashboard Pages
1️⃣ Main Dashboard

Features:

Total Sales KPI
Total Units Sold KPI
Total Returns KPI
YOY Growth KPI
Sales Trend Analysis
Sales by Category
Sales by Region
Interactive Slicers
2️⃣ Customer Analysis

Features:

Customer Performance Analysis
Top 10 Customers
Customer Regional Distribution
Customer Detail Table
3️⃣ Product Analysis

Features:

Product Performance Analysis
Top 10 Products
Category-wise Sales
Product Trend Analysis
4️⃣ Drillthrough Page

Features:

Customer Level Drillthrough
Product Purchase Analysis
Customer Transaction Details
🔍 Interactive Features
Filtering
Product Slicer
Customer Slicer
Region Slicer
Date Slicer
Drill Functionality
Drill Up
Drill Down
Drillthrough Pages
User Experience
Navigation Bar
Custom Buttons
Bookmarks
Back Buttons
Collapsible Slicer Panel
Custom Tooltips
📱 Mobile Layout

A dedicated mobile layout was designed to:

Improve mobile usability
Highlight key KPIs
Optimize visual arrangement
🔐 Security
Row Level Security (RLS)

Implemented role-based access:

North Manager
South Manager
East Manager
West Manager

Users can only access data related to their assigned region.

🛠 Tools & Technologies
Power BI Desktop
DAX
Power Query
Data Modeling
Star Schema Design
Row Level Security
📸 Dashboard Preview

Add screenshots here:

/images/dashboard.png
/images/customer-analysis.png
/images/product-analysis.png
/images/drillthrough.png
🚀 Key Learning Outcomes
Building enterprise-level Power BI dashboards
Advanced DAX calculations
Time Intelligence functions
Interactive reporting techniques
Security implementation using RLS
Dashboard performance optimization
👨‍💻 Author

Shrey Patel

