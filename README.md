# TIBCO Spotfire Global Retail Analytics Dashboard

## 📋 Project Overview
This project is an end-to-end Business Intelligence (BI) solution built using **TIBCO Spotfire** and **SQL** to analyze and optimize global retail operations. The interactive 3-page dashboard transforms raw transactional data into strategic insights, enabling executive leadership to track sales performance, evaluate regional profitability, and perform deep-dive transaction-level analysis.

---

## 🛠️ Tech Stack & Technical Skills Demonstrated
* **BI Tool:** TIBCO Spotfire
* **Database & Querying:** SQL (Data Cleaning, Aggregations, Inner Joins, Subqueries)
* **Data Visualizations:** Treemaps (Heatmaps), Scatter Plots, Cross Tables, Line Charts, Pie Charts, Bar Charts.
* **Analytical Skills:** Data Aggregation & Unaggregation, Trend Identification, Margin Analytics, Multi-dimensional Filtering, and Outlier Detection.

---

## 💾 SQL Scripts & Data Preparation
Before importing the data into Spotfire, SQL was utilized to structure, clean, and pre-aggregate the relational tables. The SQL scripts included in this repository demonstrate:
* **Relational Joins:** Combining transactional tables with product and regional metadata using `INNER JOIN`.
* **Data Filtering:** Isolating high-value transactions and segmenting products using operators like `LIKE` and `WHERE`.
* **Performance Metrics:** Calculating profit margins and total sales using aggregation functions (`SUM`, `GROUP BY`).

---

## 📊 Dashboard Architecture & Page Breakdown

### 📌 Page 1: Sales Overview
* **Focus:** Macro-level business health and structural sales trends.
* **Key Components:**
  * **Sales Distribution by Customer Segment:** Analyzes which customer categories (Consumer, Corporate, Home Office) drive the most volume.
  * **Geographic Profitability & Sales Performance:** Visualizes revenue distribution across global markets.
  * **Monthly Sales Comparison:** A time-series trend analysis to identify seasonality and monthly growth trajectories.

### 📌 Page 2: Market Analysis
* **Focus:** Regional performance, structural costs, and product matrix efficiency.
* **Key Components:**
  * **Regional Profitability Heatmap (Treemap):** High-level view of market sizes nested with profit margins to immediately spot high-revenue but low-profit zones.
  * **Product Performance:** Breaks down which product categories and lines are generating healthy margins versus those causing revenue leaks.
  * **Sales Metrics by Country:** A detailed cross-table breakdown providing precise operational numbers for regional managers.

### 📌 Page 3: Details & Insights
* **Focus:** Granular, transaction-level efficiency and micro-analytics.
* **Key Components:**
  * **Profit vs. Sales Scatter Plot:** The core analytical visual mapping individual transactions.
  * **Profitability Analysis by Transaction:** By unaggregating data points using the `Marker By: Order ID` mechanism, this chart plots hundreds of individual orders against a linear fit/trend line. This enables instantaneous discovery of low-volume high-profit wins and high-risk, negative-margin (bleeding) transactions.
