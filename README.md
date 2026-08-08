Brazilian E-Commerce Sales & Operations Analytics | Power BI

📌 Project Overview

📚 Data Source & Provenance

Source: Brazilian E-Commerce Public Dataset by OlistObtained from: KaggleDataset page: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerceOriginal 
data provider: Olist, a Brazilian e-commerce marketplace/companyGeographic coverage: BrazilData period: 2016–2018

The dataset is a publicly available e-commerce dataset published on Kaggle and contains related transactional data covering customers, orders, order items, payments, reviews, products, sellers, and product categories. The Kaggle ecosystem identifies this dataset as the “Brazilian E-Commerce Public Dataset by Olist.” 

Important: The dataset was not collected by me. I used the publicly available Olist dataset from Kaggle as the source data and performed the Power BI data preparation, modeling, calculations, and visualization for this project.

Dataset Tables Used :
olist_customers_dataset.csv
olist_orders_dataset.csv
olist_order_items_dataset.csv
olist_order_payments_dataset.csv
olist_order_reviews_dataset.csv
olist_products_dataset.csv
olist_sellers_dataset.csv
product_category_name_translation.csv

Data Journey :
Olist
  ↓
Public Brazilian E-Commerce Dataset
  ↓
Kaggle
  ↓
CSV Tables
  ↓
Power Query
  ↓
Data Model + DAX
  ↓
Interactive Power BI Dashboard

For portfolio transparency, the README clearly distinguishes the original data source from the analysis and dashboard work performed in this project.
This project analyzes an e-commerce business across sales, customer behavior, product performance, delivery operations, and seller performance.

The Power BI report converts transactional data into an interactive management dashboard that helps answer questions such as:
How much revenue is the business generating?
How are sales changing month by month?
Which product categories and products contribute the most revenue?
Which states generate the most customers and revenue?
What is the on-time vs. late delivery performance?
Which sellers generate the highest revenue?
How do orders, revenue, ratings, and delivery performance vary across the business?
The final report contains 6 analytical pages designed for both executive-level review and detailed business analysis.

🎯 Business Objective:
The primary objective is to create a single analytical view of e-commerce performance and identify opportunities to improve:
Revenue growth
Product/category performance
Customer engagement
Delivery efficiency
Seller performance
Regional performance

🗂️ Dashboard Pages

1. Executive Overview
Provides a high-level snapshot of the business.

Key KPIs:
Total Revenue: 16.01M
Total Orders: 99K
Total Customers: 96K
Total Products Sold: 135K
Average Order Value: 160.99
Average Rating: 4.09
Total Sellers: 3K
Average Delivery Days: 12.50

Visuals:
Monthly Revenue Trend
Revenue by Customer State
Revenue by Payment Type
Top 10 Products
Top 10 Sellers

Business use: Quickly understand overall business health and identify major revenue contributors.

2. Sales Analysis
Focuses on revenue trends and category performance.

Key KPIs:
YTD Product Sales: 7.39M
SPLY Sales: 7.31M
YoY Growth %
MTD Product Sales
QTD Product Sales
Average Quantity: 1.36

Visuals:
Total Sales by Month
Top 10 Product Categories
Monthly Revenue Change
Category Ranking

Business use: Analyze sales trends, identify high-performing categories, and understand changes in monthly revenue.

3. Customer Analysis
Focuses on customer distribution, spending, ratings, and order behavior.

Key KPIs:
Total Customers: 96K
Repeat Customers
Repeat Customer Rate %
Revenue per Customer: 166.59
Orders per Customer: 1.03

Visuals:
Customers by State
Revenue by Customer State
Reviews by Customer Rating
Orders by Order Value Range
Customers by Month-Year

Business use: Understand regional customer concentration, order value distribution, and customer satisfaction.

4. Product Analysis
Evaluates product and category performance.

Key KPIs:
Total Products Sold: 125K
Best Selling Product
Lowest Selling Product
Best Category: health_beauty
Worst Category: security_and_services
Average Product Rating: 4.22

Visuals:
Top 10 Products
Bottom 10 Products
Quantity Sold by Category
Price vs. Rating
Revenue by Category

Business use: Identify high- and low-performing categories, understand product demand, and evaluate the relationship between price and rating.

5. Delivery Analysis
Measures operational and logistics performance.

Key KPIs:
Average Delivery Days: 12.50
On-Time Orders: 92K
Late Orders: 8K
Late Delivery %: 0.08
Total Freight: 2.25M
Average Freight: 19.99
On-Time Delivery %: 0.95

Visuals:
On-Time Delivery %
Average Delivery Days by State
Average Delivery Days by Month-Year
Delivery Status
Delivery Days by Month & State

Business use: Identify regions and periods with slower delivery performance and monitor logistics efficiency.

6. Seller Performance
Evaluates seller contribution and operational performance.

Key KPIs:
Total Sellers: 3K
Seller Revenue: 13.59M
Seller Orders: 99K
Average Seller Revenue: 4.39K
Average Rating: 4.09
Total Freight: 2.25M

Visuals:
Seller Rating Distribution
Top 10 Sellers
Orders vs. Revenue
Sales by Seller State
Monthly Seller Revenue
Seller Performance Matrix

Business use: Identify high-value sellers, compare seller revenue and order volume, and evaluate seller performance by region.

📊 Key Business Findings
Based on the completed dashboard
Revenue & Sales:
The dashboard reports 16.01M total revenue across approximately 99K orders.
Monthly revenue shows significant variation, with stronger performance in several months and a noticeable decline around September in the displayed trend.
The Sales Analysis page reports 7.39M YTD sales versus 7.31M SPLY sales, indicating positive year-over-year movement in the displayed KPI.

Customer Performance:
The business has approximately 96K customers.
Average revenue per customer is 166.59, while average orders per customer is 1.03.
São Paulo (SP) is the strongest customer-revenue state in the dashboard, contributing approximately 5.8M.

Product Performance:
health_beauty is the leading category in the dashboard.
The Top 10 Products visual shows health_beauty, watches_gifts, and bed_bath_table among the strongest revenue contributors.
The Product Analysis page reports an average product rating of 4.22.

Delivery Operations:
Approximately 92K orders are on time, while 8K are late.
The dashboard reports an On-Time Delivery % of 0.95 and an average delivery time of 12.50 days.
Delivery performance varies considerably by state, making regional logistics analysis important.

Seller Performance:
Approximately 3K sellers are represented.
Seller revenue is approximately 13.59M.
São Paulo (SP) is the dominant seller state in the displayed seller-revenue analysis.
The Orders vs. Revenue scatter plot can be used to identify high-volume/high-revenue sellers and potential outliers.

🧮 Key Analytical Measures
The report uses Power BI measures for business KPIs and time-based analysis, including:
Total Revenue
Total Orders
Total Customers
Total Products Sold
Average Order Value
Average Rating
Average Delivery Days
YTD Sales
SPLY Sales
YoY Growth %
MTD Sales
QTD Sales
Average Quantity
Repeat Customers
Repeat Customer Rate
Revenue per Customer
Orders per Customer
Total Freight
Average Freight
Late Orders
On-Time Orders
Late Delivery %
Seller Revenue
Seller Orders
Average Seller Revenue

🔄 Data Preparation & Transformation
The project uses Power BI's data preparation capabilities to transform raw e-commerce data into an analysis-ready model.
Typical transformation steps include:
Data type correction
Null and blank value handling
Duplicate checking
Date transformation
Category translation
Delivery-day calculation
Delivery status classification
Order value categorization
Rating categorization
Calendar table creation
Relationship creation between transactional and dimension tables

🏗️ Data Modeling

The report is designed around a relational e-commerce model connecting areas such as:

                 Calendar
                    │
                    ▼
Customers ─────── Orders ─────── Order Items ─────── Products
                    │
                    ├────────── Payments
                    │
                    └────────── Reviews

Sellers ───────── Order Items

🎛️ Interactive Features
The dashboard includes interactive filters/slicers such as:
Month
Year
Quarter
Customer City
Customer State
Seller State
Payment Type
Delivery Status
Users can filter the report and analyze how the KPIs and visuals change according to the selected business segment.

🛠️ Tools & Technologies :
Power BI Desktop
Dashboard development and visualization
Power Query
Data cleaning and transformation
DAX
KPI calculations and analytical measures
Data Modeling
Relationships and analytical structure
Kaggle
Source/distribution platform for the public Olist e-commerce dataset

📈 Skills Demonstrated:
Power BI
Interactive dashboard development
KPI cards
Line charts
Bar charts
Donut charts
Treemap
Scatter plot
Maps
Matrix
Waterfall chart
Slicers
Conditional analysis
DAX
Aggregation measures
CALCULATE
DIVIDE
DISTINCTCOUNT
Time intelligence
YTD / SPLY / YoY analysis
KPI calculations
Business logic
Data Analytics
Sales analysis
Customer analysis
Product analysis
Seller analysis
Delivery performance
Regional analysis
Trend analysis
Business storytelling

💡 Business Recommendations
The dashboard can support decisions such as:
Improve regional logistics by investigating states with consistently high delivery times.
Prioritize high-performing product categories such as health_beauty and other leading categories.
Investigate low-performing categories to determine whether pricing, demand, availability, or product mix is responsible.
Focus seller management on high-impact sellers using revenue, order volume, rating, and delivery metrics together.
Strengthen customer retention initiatives, particularly because average orders per customer are close to one.
Monitor monthly sales fluctuations and investigate periods with sharp declines or unusually strong performance.

📸 Dashboard Preview

Executive Overview : 





Sales Analysis



Customer Analysis



Product Analysis



Delivery Analysis



Seller Performance



Add the six exported Power BI page screenshots to a screenshots folder using the filenames above.

📁 Recommended Repository Structure

E-Commerce-PowerBI-Analytics/
│
├── README.md
│
├── Power BI/
│   └── E-Commerce Dashboard.pbix
│
├── Dataset/
│   └── dataset_files.csv
│
├── Screenshots/
│   ├── executive-overview.png
│   ├── sales-analysis.png
│   ├── customer-analysis.png
│   ├── product-analysis.png
│   ├── delivery-analysis.png
│   └── seller-performance.png
│
└── Documentation/
    └── Business-Insights.pdf

🚀 How to Use

Download or clone this repository.

Open the .pbix file using Power BI Desktop.

If Power BI requests the data source, update the dataset path.

Refresh the model.

Use the slicers to explore different business segments.

Navigate through the six dashboard pages.
