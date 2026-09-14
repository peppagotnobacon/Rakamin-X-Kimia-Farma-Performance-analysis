# Rakamin-X-Kimia-Farma-Performance-analysis
Final submission for project based internship (Looker studio link: https://datastudio.google.com/s/gxiHGMAR_r0)

# Kimia Farma Business Performance Analysis (2020–2023)

An end-to-end data analytics project uncovering revenue drivers, spatial performance, profit margins, and operational mismatches across Kimia Farma branches nationwide.

---

## Executive Summary

This project evaluates Kimia Farma’s historical performance (2020–2023) to address strategic growth bottlenecks. By consolidating raw transactional and inventory data using **Google BigQuery** and visualizing key metrics in **Looker Studio**, the analysis uncovers revenue stagnation, customer retention challenges, and operational disparities between branch infrastructure ratings and customer transaction experience.

---

## Business Problem & Objectives

### Problem Statement
* **Spatial Performance Gaps:** Insufficient spatial analysis regarding regional profit generation and revenue concentration across provinces.
* **Margin Evaluation Complexity:** Challenges in evaluating net margins stemming from price-tiered profit structures across product categories.
* **Operational Disparities:** Unidentified disparities between branch facility standards and actual customer transaction satisfaction.

### Project Objectives
* **Data Integration:** Consolidate raw datasets into a unified, aggregated master table in Google BigQuery to streamline the analytical pipeline.
* **Exploratory Data Analysis (EDA):** Perform EDA to uncover multi-year transaction trends, evaluate regional profit contributions, and detect operational anomalies between branch quality ratings and customer feedback.
* **Interactive Dashboard:** Build an interactive Looker Studio dashboard to facilitate business performance monitoring and enable deep-dive analysis.
* **Strategic Recommendations:** Formulate actionable, data-driven strategies to support management in optimizing branch operations, customer retention, and market potential.

---

## Data Architecture & Scope

### Data Scope
* **Time Period:** 2020 – 2023 (4 Years)
* **Geographic Coverage:** National scale (covering all provinces and major cities across Indonesia)

### Source Tables
| Table Name | Description |
| :--- | :--- |
| `kf_final_transaction` | Daily operational transaction records |
| `kf_inventory` | Product inventory and stock availability data |
| `kf_kantor_cabang` | Branch office master data (location, province, city, facility rating) |
| `kf_product` | Product catalog details, pricing, and category structures |

### Analytical Pipeline Workflow
[ 1. Create Project ] ➔ [ 2. Create Dataset ] ➔ [ 3. Import Raw Data ] ➔ [ 4. Create Aggregated Table ] ➔ [ 5. Connect to Looker Studio ]

---

## Key Business Insights

1. **Stagnant Multi-Year Growth**  
   Overall business growth remained flat from 2020 to 2023. Annual total sales consistently plateaued at around **IDR 80 Billion**, exhibiting no upward trend, downward slope, or clear monthly seasonality.

2. **West Java Revenue Concentration Driven by Branch Density**  
   West Java generated the highest cumulative sales at **IDR 94.9 Billion**. However, this volume is heavily driven by branch density, West Java accounts for **510 branches (~30% of total Kimia Farma branches nationwide)**.

3. **Homogeneous Performance Across Regions & Categories**  
   Sales performance across 31 provinces and 3 branch categories was nearly identical. This uniformity stems from standardized gross profit margin percentages tied directly to product pricing tiers rather than regional market dynamics.

4. **Facility Rating vs. Transaction Satisfaction Mismatch**  
   A correlation coefficient of **$r = 0.0019$** indicates zero correlation between branch facility ratings and customer transaction satisfaction ratings. High branch ratings do not translate to superior transaction experiences.

5. **Weak Customer Retention Rates**  
   Customer retention remains low **58% of 264,601 unique customers** completed only one transaction throughout the entire 4-year period.

---

## Strategic Recommendations

* **Targeted Regional Expansion:** Prioritize branch expansion in provinces demonstrating high sales performance relative to lower branch density, rather than over-saturating existing high-density regions.
* **Strategic Discount Restructuring:** Reevaluate discounting policies to turn promotional spend into a revenue driver rather than pure cost. Reallocate discounts toward slow-moving items and high-intent first-time customers.
* **Retention Program Implementation:** Launch dedicated customer loyalty initiatives (e.g., membership programs, refill reminders for chronic medication) to improve the single-transaction repeat rate.
* **Operational Audits on Experience Gaps:** Conduct targeted operational audits exclusively on branches displaying the highest disparities between branch facility ratings and low customer transaction ratings.

---

## Tech Stack Used

* **Data Warehousing & SQL:** Google BigQuery
* **Business Intelligence & Data Visualization:** Looker Studio

## Dashboard Preview
<img width="284" height="400" alt="dashboard_kimia_farma" src="https://github.com/user-attachments/assets/c37a2f0b-f0e4-4ab9-88aa-81cbb2373da7" />
