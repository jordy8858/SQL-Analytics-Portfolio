# Commercial Aviation Operations: Optimizing Hub Efficiency & Turnaround Times

## 📌 Project Overview
This project synthesizes and analyzes a complete operational data pipeline for a commercial airline fleet. From raw data generation to advanced SQL database querying and Python-based executive visualizations, this analysis identifies critical operational bottlenecks affecting on-time performance. The goal is to translate raw operational logs into actionable business intelligence that can improve scheduling, fleet availability, and ground operations.

My lifelong foundation in aviation dynamics and mechanics—stemming from early hands-on work in air museums and flight training—drives the analytical approach here. Understanding the physical realities of aircraft mechanics and airspace congestion ensures these insights go beyond surface-level numbers to address true operational logistics.

## 🛠️ Technical Stack
* **Languages:** SQL, Python 3
* **Libraries:** `pandas`, `sqlite3`, `seaborn`, `matplotlib`, `faker`
* **Environment:** Google Colab, SQLite
* **Key Skills Demonstrated:** Relational Database Architecture, Synthetic Data Generation, Advanced SQL (Window Functions, CTEs, Aggregations), Exploratory Data Analysis (EDA), Data Storytelling.

## 🗂️ Repository Contents
* `Aviation_Operations_Analytics.ipynb`: The primary Google Colab notebook containing the end-to-end Python environment setup, database generation, SQL queries, and visual outputs.

## 📊 Key Analytical Highlights
This analysis mirrors the day-to-day operational challenges faced by major commercial carriers, focusing on three core areas:

1. **Hub Departure Delay Analysis:** 
   Leveraged SQL aggregations and conditional logic to identify network bottlenecks. The data isolates severe departure delays (45+ minutes) across major high-volume network nodes like DFW and PHX, comparing them against regional non-hub airports.
   
2. **Maintenance Impact on Fleet Availability:** 
   Utilized SQL `JOIN`s and datetime mathematics to bridge ground operations and fleet mechanics. This section analyzes how unscheduled repairs and avionics calibrations impact overall availability across different aircraft types (e.g., Boeing 777 vs. Airbus A321neo).

3. **Ground Turnaround Efficiency:** 
   Applied advanced SQL Window Functions (`LAG()`) to calculate precise ground turnaround times for individual tail numbers. By measuring the exact time between a prior arrival and subsequent departure, this query highlights variance in operational ground efficiency.

## 💡 Strategic Business Recommendations
Based on the data insights generated in this project, the following operational adjustments are recommended:

* **Pad Block Times at Major Hubs:** Data indicates higher concentrations of severe departure delays at primary network nodes like DFW and PHX. Adjusting scheduled block times during peak traffic windows (14:00 - 18:00) will help absorb taxiway congestion and prevent cascading network delays.
* **Proactive Maintenance Staging:** Unscheduled repairs on older, narrow-body aircraft routinely exceed baseline duration averages. Staging specialized maintenance personnel and parts at high-traffic hubs for these specific fleets will reduce grounded time.
* **Standardize Wide-Body Turnarounds:** Ground turnaround distributions show significant variance for high-capacity aircraft like the Boeing 777. Streamlining boarding procedures and standardizing ground service equipment allocation can tighten these turnaround windows and improve daily fleet utilization.

## 🚀 Future Scope
Future iterations of this project will integrate live weather data APIs and passenger load factors to train a predictive machine learning model (Random Forest / Logistic Regression) capable of forecasting the probability of severe delays before they occur.

---
*This project is Part 2 of my broader SQL Analytics Portfolio. [Return to Main Portfolio](Link_To_Main_Repo_Here)*
