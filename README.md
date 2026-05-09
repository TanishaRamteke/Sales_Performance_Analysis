# 📊 Sales Performance Analysis
### End-to-end sales analytics using SQL and Python — uncovering revenue trends, profit drivers, and category-level business insights.

---

## 🗂️ Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Tools & Technologies](#tools--technologies)
- [Analysis Performed](#analysis-performed)
- [Key Insights](#key-insights)
- [Project Structure](#project-structure)
- [How to Run](#how-to-run)
- [Conclusion](#conclusion)

---

## Overview

This project delivers a full analytical workflow on transactional sales data — from structured querying in SQL to visual storytelling in Python.

The goal is to answer core business questions:
- Which product categories are most and least profitable?
- How do sales and profit trend over time?
- What relationships exist between key metrics like discount, sales, and profit?

---

## Dataset

| Attribute | Details |
|-----------|---------|
| **Source** | Superstore Sales Dataset |
| **Format** | CSV + SQLite database |
| **Key Fields** | Sales, Profit, Category, Sub-Category, Order Date, Region, Discount |
| **Scope** | Multi-year transactional records across product categories and regions |

---

## Tools & Technologies

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-SQLite-lightgrey?logo=sqlite&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4c72b0)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)

---

## Analysis Performed

### 1. 🗃️ SQL Data Extraction
- Loaded CSV data into a SQLite database using Python
- Wrote structured SQL queries to extract aggregated sales and profit data by category, sub-category, and month
- Used `GROUP BY`, `ORDER BY`, and aggregate functions (`SUM`, `AVG`) for business-level summaries

### 2. 📅 Monthly Sales Trend Analysis
- Parsed and grouped order dates by month to observe seasonality
- Visualized sales volume over time to identify peak and low-performing periods

### 3. 🏷️ Category-wise Sales & Profit Analysis
- Compared total sales and profit across the three main product categories
- Identified which categories generate the most revenue vs. the most profit

### 4. 🔗 Correlation Analysis
- Computed a correlation matrix across numerical fields (Sales, Profit, Discount, Quantity)
- Used a Seaborn heatmap to visualize metric relationships and detect profit-eroding patterns

### 5. 📈 Performance Visualizations
- Bar charts for category and sub-category breakdowns
- Line charts for monthly trend analysis
- Heatmap for correlation structure

---

## Key Insights

> ⚠️ *Note: Replace the placeholders below with your actual values from the notebook.*

- 📦 **Technology** is the highest-revenue category, contributing approximately **XX%** of total sales
- 💰 **Office Supplies** shows the strongest profit margin relative to its sales volume
- 🪑 **Furniture** — despite significant sales — yields the lowest profit, likely driven by discounting
- 📉 A **negative correlation** between Discount and Profit suggests aggressive discounting is hurting margins
- 📆 Sales peak noticeably in **Q4**, indicating strong seasonal demand patterns

---

## Project Structure

```
Sales_Performance_Analysis/
│
├── Sales_Performance_Analysis_SQL_Python.ipynb   # Main analysis notebook
├── superstore_big.csv                            # Raw dataset
├── superstore_big.db                             # SQLite database
├── README.md                                     # Project documentation
└── visuals/                                      # (Recommended) Exported chart images
```

---

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/TanishaRamteke/Sales_Performance_Analysis.git
cd Sales_Performance_Analysis

# 2. Install dependencies
pip install pandas matplotlib seaborn jupyter

# 3. Launch the notebook
jupyter notebook Sales_Performance_Analysis_SQL_Python.ipynb
```

> No additional setup needed — the SQLite database is created from the CSV within the notebook.

---

## Conclusion

This project demonstrates a practical, end-to-end approach to sales analytics — combining the querying power of SQL with Python's data manipulation and visualization capabilities.

The analysis surfaces actionable insights around category profitability, discount impact, and seasonal trends that could directly inform inventory, pricing, and marketing decisions.

**What's next:**
- 🔮 Add a 30-day sales forecasting model (Prophet / ARIMA)
- 👥 Build RFM-based customer segmentation
- 🚀 Deploy an interactive dashboard using Streamlit

---

<p align="center">
  Made by <a href="https://github.com/TanishaRamteke">Tanisha Ramteke</a>
</p>
