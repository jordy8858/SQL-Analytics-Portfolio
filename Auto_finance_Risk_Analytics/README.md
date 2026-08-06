# Automotive Loan Portfolio & Risk Analytics: Credit Risk & LTV Exposure

## 📌 Project Overview
This project simulates and analyzes a complete enterprise auto finance portfolio dataset to evaluate credit risk, portfolio health, and collateral exposure. Moving from raw database schema generation using SQLite to advanced SQL querying and risk matrix visualizations, this analysis translates financial data into actionable business intelligence for corporate lending operations. 

The primary objective is to demonstrate core data analyst competencies: designing relational schemas, writing complex SQL queries (CTEs and conditional aggregations), tracking portfolio credit tiers, and quantifying Loan-to-Value (LTV) risk.

## 🛠️ Technical Stack
* **Languages:** SQL, Python 3
* **Libraries:** `pandas`, `sqlite3`, `seaborn`, `matplotlib`, `faker`
* **Environment:** Google Colab, SQLite
* **Key Skills Demonstrated:** Relational Database Architecture, Synthetic Enterprise Data Generation, Advanced SQL (CTEs, Conditional Aggregations), Exploratory Data Analysis (EDA), Financial Risk Metrics (Delinquency Rates, LTV Exposure).

## 🗂️ Repository Contents
* `Auto_Finance_Risk_Analytics.ipynb`: The primary Google Colab notebook containing the end-to-end environment setup, database generation, SQL queries, and visual outputs.

## 📊 Key Analytical Highlights
This analysis mirrors the core risk-assessment workflows managed by automotive financial services divisions, focusing on two main pillars:

1. **Delinquency Risk by Credit Tier:** 
   Utilized SQL Common Table Expressions (CTEs) and conditional logic to segment borrowers into credit tiers (Super Prime down to Deep Subprime) based on credit scores. The query aggregates total portfolio value and computes severe delinquency rates (60+ days past due) across tiers to isolate high-risk capital exposure.
   
2. **Loan-to-Value (LTV) & Collateral Exposure:** 
   Bridged loan records with vehicle collateral details to calculate average LTV percentages and average APRs by make and model. The analysis isolates "underwater" loans where the outstanding loan balance exceeds current market value (LTV > 100%), highlighting potential losses upon default.

## 💡 Strategic Business Recommendations
Based on the analytical insights generated within the notebook, the following risk-mitigation strategies are recommended:

* **Refine Lending Criteria for Subprime Segments:** Given that Subprime and Deep Subprime tiers exhibit significantly elevated severe delinquency rates, underwriting teams should tighten approval thresholds, adjust interest rate pricing curves, or enforce higher minimum down payments for these segments.
* **Monitor High-Exposure Vehicle Models:** Continuously track vehicle models showing high volumes of underwater loans. Implementing stricter LTV caps on rapidly depreciating vehicle classes will protect the portfolio against collateral shortfalls.
* **Proactive Delinquency Management:** Establish early-intervention workflows for borrowers approaching the 60-day delinquency threshold in high-risk credit tiers to reduce default rates through targeted communication and flexible restructuring plans.
* **Data-Driven Pricing Strategy:** Align interest rates more closely with collateral-specific risk matrices to ensure yields adequately compensate for vehicle-specific depreciation trends and borrower credit profiles.

---
*This project is Part 3 of my broader SQL & Data Analytics Portfolio. [Return to Main Portfolio](Link_To_Main_Repo_Here)*
