# Logistics Performance & Customer Satisfaction Analysis — Olist E-commerce

**Author:** Carlos Hernández Godoy  
**Profile:** Data Analyst | Industrial Engineer  
**Year:** 2026  

---

## Overview

This repository presents an analysis of **logistics performance** in an e-commerce context, focused on understanding how **delivery delays impact customer satisfaction** and identifying **priority areas for operational improvement**.

Using Python for data preparation and analysis, and Power BI for executive visualization, the project evaluates delivery timeliness, customer reviews, and regional performance to support data-driven logistics decisions.

The analysis is designed to move beyond descriptive metrics and provide **actionable insights** that can help reduce late deliveries and improve customer experience.

---

## Objectives of the Analysis

- Measure the **rate of late deliveries** across delivered orders.
- Evaluate the **impact of delivery delays on customer review scores**.
- Identify **regions with higher logistics impact**, combining delay rate and customer satisfaction.
- Prioritize **where to act first** to reduce delays and improve reviews.
- Communicate findings through a **clear, executive-level dashboard**.

---

## Repository Structure
```
data-ecommerce-olist-analysis-2026/
├── 01_data/
│ └── raw/
│ ├── olist_customers_dataset.csv
│ ├── olist_geolocation_dataset.csv
│ ├── olist_order_items_dataset.csv
│ ├── olist_order_payments_dataset.csv
│ ├── olist_order_reviews_dataset.csv
│ ├── olist_orders_dataset.csv
│ ├── olist_products_dataset.csv
│ ├── olist_sellers_dataset.csv
│ └── product_category_name_translation.csv
├── 02_notebooks/
│ └── 01_olist_logistics_analysis.ipynb
├── 03_img/
│ └── executive_dashboard.png
├── 04_outputs/
│ └── tables/
│ ├── monthly_late_delivery_trend.csv
│ ├── review_by_delivery_delay.csv
│ └── state_priority_logistics.csv
├── 05_pbix/
│ └── olist_logistics_dashboard.pbix
└── 06_README.md
```
Raw data files are included in this repository for reproducibility purposes.  
All analytical tables used in Power BI are generated from the notebook and stored under `04_outputs/tables`.
---

## Data Used

- **Source:** Brazilian E-Commerce Public Dataset by Olist (Kaggle)
- **Domain:** E-commerce operations and logistics
- **Time period:** 2016–2018
- **Key entities:** orders, deliveries, customer reviews, customer location

Column names are kept in English to remain consistent with the original dataset.  
Dashboard titles and narrative are also presented in English for international context and portfolio consistency.

---

## Analytical Approach

The analysis follows a **business-oriented and decision-focused approach**, avoiding unnecessary complexity:

- The logistics KPI (**late delivery rate**) is calculated **only for delivered orders**, ensuring metric validity.
- Delivery delays are evaluated not only by frequency, but by their **impact on customer satisfaction**.
- Customer review scores are used as a proxy for **experience quality**.
- Regional prioritization combines:
  - delivery delay rate,
  - average review score,
  - order volume (to avoid low-sample bias).

Each metric and aggregation is designed to answer a concrete operational question, rather than maximize technical complexity.

---

## Tools and Technologies

### Python (pandas)
- Data ingestion and exploration.
- Data cleaning and type validation.
- Definition of logistics KPIs.
- Analysis of delivery delays and customer satisfaction.
- Regional prioritization based on impact.
- Export of finalized analytical tables for visualization.

Notebooks:
- `02_notebooks/01_olist_logistics_analysis.ipynb`

---

### Power BI
- Import of pre-processed tables generated in Python.
- KPI visualization and executive storytelling.
- Single-page dashboard focused on clarity and decision support.
- Minimal DAX, avoiding re-implementation of business logic already defined in Python.

Dashboard file:
- `05_pbix/olist_logistics_dashboard.pbix`

---

### AI (ChatGPT)
- Support in structuring the analytical workflow.
- Validation of analytical logic and KPI definitions.
- Assistance with documentation clarity and narrative refinement.

AI was used strictly as a **support tool**, without replacing analytical judgment or interpretation.

---

## Executive Dashboard Summary

The dashboard is designed for **quick interpretation and prioritization**:

- **Key KPIs**
  - Percentage of late deliveries.
  - Average review score for on-time deliveries.
  - Average review score for late deliveries.
- **Trend analysis**
  - Monthly evolution of late delivery rate.
- **Impact comparison**
  - Customer satisfaction: on-time vs late deliveries.
- **Operational prioritization**
  - Ranking of states with higher logistics impact (delay rate + low reviews).

**Dashboard file:** `05_pbix/olist_logistics_dashboard.pbix`  
**Preview image:** `03_img/executive_dashboard.png`

---

## Key Insights

- Only **~8% of delivered orders** arrive later than the estimated delivery date.
- Despite the low frequency, late deliveries receive **significantly lower customer ratings**:
  - On-time deliveries: **~4.29 average score**
  - Late deliveries: **~2.57 average score**
- This represents a **drop of ~1.7 rating points**, indicating a disproportionate impact on customer satisfaction.
- The issue is not systemic across all regions:
  - Certain states concentrate higher delay rates and lower reviews.
  - Focusing logistics improvements on these regions would yield the **highest return in customer experience**.
- Reducing late deliveries, even marginally, can generate a **positive and measurable improvement in overall reviews**.

---

## Conclusion

This project demonstrates how combining Python-based analysis with focused Power BI visualization enables a clear understanding of logistics performance and its impact on customer satisfaction.

Rather than treating delivery delays as a purely operational metric, the analysis connects logistics outcomes directly to customer perception, allowing for **targeted, data-driven decision-making**.

The work reflects an analyst mindset oriented toward:
- metric validity,
- business relevance,
- and actionable insights.

---

## Contact
```
Carlos Hernández Godoy  
Data Analyst | Python · Power BI · SQL · Excel
Email: carloshernandez.data@gmail.com
```