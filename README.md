# Atliq Hardware Sales Insights Data Analysis

## Project Overview
This project focuses on analyzing the sales data of AtliQ Hardware, a computer hardware manufacturing company facing declining sales performance. The goal was to build an interactive dashboard to provide the Sales Director with real-time, actionable insights into revenue, sales quantity, market trends, and top customers to make data-driven decisions.

## Tech Stack Used
* **Database:** MySQL (Local Database Server)
* **BI Tool:** Power BI Desktop
* **Language:** SQL, DAX (Data Analysis Expressions)

## Data Architecture & Cleaning (Power Query)
Data was extracted directly from a local MySQL database instance. The following transformations were performed using Power Query:
* **Currency Standardization:** Standardized conflicting transaction values (handling transactions in USD vs INR) to maintain a unified revenue model.
* **Data Filtering:** Cleaned and filtered garbage values from the `sales markets` table (such as empty strings or invalid zones).
* **Star Schema Modeling:** Established a clean dimensional model linking transaction facts with product, customer, date, and market dimensions.

## Dashboard Showcase
Below is the interactive sales report built in Power BI Desktop:

![Atliq Hardware Sales Dashboard](https://github.com/Sumaid05/Atliq-Hardware-Sales-Insights/blob/main/Dashboard%20Screenshot.png?raw=true)

## Key Insights Discovered
* **Top Markets:** Delhi NCR and Mumbai emerged as the highest revenue-generating hubs, contributing significantly to the overall business.
* **Revenue Trend:** Identified significant seasonal dips in specific quarters, allowing management to track shifting purchasing behaviors over the years (2017–2020).
* **Customer Analysis:** Pinpointed the top 5 high-value corporate clients driving the bulk of sales quantity, emphasizing the importance of key account management.

## How to Run This Project
1. Clone this repository to your local machine.
2. Import the `db_dump.sql` file into your local MySQL server using MySQL Workbench.
3. Open the `sales_insights.pbix` file using Power BI Desktop.
