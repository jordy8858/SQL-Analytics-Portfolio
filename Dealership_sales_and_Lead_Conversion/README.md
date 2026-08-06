# Dealership Sales and Lead Conversion Analysis

**Author:** Jordan Smith  
**Target Domain:** Automotive Sales Operations & Business Intelligence 

## 📌 Project Overview
This project simulates a high-volume automotive dealership's operations, focusing on Customer Relationship Management (CRM) data, lead conversion metrics, and inventory turnover. By generating a synthetic relational database and performing advanced SQL analytics, this project bridges the gap between front-line sales operations and actionable business intelligence. 

The goal of this analysis is to identify top-performing lead sources, track monthly sales representative performance, and manage inventory aging to optimize marketing spend and operational efficiency.

## 🛠️ Tech Stack & Tools
* **Languages:** Python, SQL (SQLite)
* **Libraries:** `Faker` (Synthetic Data Generation), `Pandas` (Data Manipulation), `Seaborn` & `Matplotlib` (Data Visualization)
* **Environment:** Google Colab / Jupyter Notebook

## 🗄️ Relational Database Schema
A local SQLite database was engineered to mirror a standard automotive CRM and Dealer Management System (DMS). It consists of four interconnected tables:
1. **`sales_reps`**: Employee demographics, hire dates, and department assignments (Floor, Internet, Fleet).
2. **`vehicles`**: Inventory details including VIN, Make, Model, MSRP, and acquisition dates.
3. **`leads`**: Customer inquiry logs tracking lead source, inquiry date, and conversion status.
4. **`sales`**: Finalized transactions linking converted leads to specific vehicles and sales representatives.

## 📈 Key SQL Techniques Demonstrated
This notebook goes beyond basic aggregations, showcasing mid-to-senior level SQL querying designed for corporate reporting:

* **Lead Source ROI (CTEs & JOINs):** Utilized Common Table Expressions to calculate conversion rates and gross revenue across different marketing channels (e.g., TrueCar, Cars.com).
* **Monthly Sales Leaderboard (Window Functions):** Applied `DENSE_RANK() OVER (PARTITION BY ...)` to dynamically rank sales representatives based on monthly revenue generation.
* **Inventory Aging Analysis (Date Logic & `CASE WHEN`):** Leveraged `JULIANDAY()` date math and conditional `CASE WHEN` logic to segment vehicle inventory into aging buckets (Sold within 30 days vs. Aged over 60 days).
* **Executive Dashboards (`VIEW` Creation):** Engineered a reusable virtual `VIEW` (`executive_daily_summary`) to streamline daily KPI reporting for integration with BI tools like Tableau or Power BI.

## 💡 Business Insights & Recommendations
1. **Optimize Marketing Spend:** **TrueCar** and **Cars.com** consistently deliver the highest conversion rates (~14-15%) and drive the majority of gross revenue. Marketing budgets should be reallocated to maximize volume from these channels.
2. **Inventory Velocity:** Analytical models flagged specific makes and models averaging over 190 days on the lot. Implementing targeted promotions or adjusting pricing strategies for vehicles aged over 60 days is recommended to reduce holding costs.
3. **Sales Coaching:** Data highlights clear performance gaps among representatives. The monthly leaderboard can be used to restructure incentive programs and pair top performers with struggling reps for targeted coaching.

## 🚀 How to Run the Project
1. Clone this repository to your local machine.
2. Open `Dealership_Sales_and_Lead_Conversion_SQL.ipynb` in Google Colab or Jupyter Notebook.
3. Run the cells sequentially to generate the mock dataset, build the SQLite database, and execute the analytical queries.
