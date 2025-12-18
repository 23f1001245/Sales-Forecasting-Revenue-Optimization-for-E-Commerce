# Sales Forecasting & Revenue Analysis for E-Commerce

## Overview

This project focuses on solving real-world **inventory planning and revenue optimization** problems for a mid-sized e-commerce business using data analytics and machine learning. The objective is to forecast product demand accurately, identify key revenue drivers, and design demand-sensitive pricing strategies that improve profitability without increasing operational overhead.

The analysis is based on a large-scale transactional dataset and emphasizes **business decision-making**, not just model building.

---

## Business Problems Addressed

* Frequent **stockouts** of high-demand products
* **Overstocking** of low-impact SKUs
* Lack of a **data-driven pricing and revenue strategy**

---

## Dataset

* Source: Kaggle – UK Online Retail Dataset
* Records: 500,000+ transactional entries
* Time Period: December 2010 – December 2011
* Key Fields:

  * InvoiceNo, StockCode, Description
  * Quantity, UnitPrice, InvoiceDate
  * CustomerID, Country

---

## Methodology

### 1. Data Cleaning & Feature Engineering

* Removed missing and invalid transactions (returns, zero pricing)
* Converted timestamps and extracted time-based features
* Computed transaction-level revenue

### 2. Exploratory Data Analysis (EDA)

* Revenue trends across time (monthly, weekly, weekday)
* Product-level revenue concentration (Pareto analysis)
* Customer segmentation using **RFM (Recency, Frequency, Monetary)**

### 3. Demand Forecasting

* Aggregated weekly product demand
* Applied:

  * **Moving Averages** for trend smoothing
  * **ARIMA models** for time-series demand forecasting
* Focused on top revenue-generating SKUs to guide inventory planning

### 4. Revenue Modeling & Prediction

* Built and compared multiple models:

  * Multiple Linear Regression
  * **Random Forest Regressor** (best-performing model)
  * XGBoost and LightGBM
* Identified key revenue drivers using feature importance analysis

### 5. Price Elasticity & Simulation

* Analyzed relationship between price and demand
* Simulated category-wise pricing strategies (Low / Mid / Premium)
* Estimated demand drops and revenue impact post price adjustments

---

## Key Results

* Recovered **£35,000+ monthly revenue** by fixing understocking of top products
* Achieved **~4.8% overall revenue uplift** through forecast-based inventory planning
* Generated **~£420K simulated revenue gain** via elasticity-based pricing strategies
* Confirmed **quantity sold** as the strongest driver of revenue

---

## Tools & Technologies

* **Python**
* Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels
* Models: ARIMA, Random Forest, XGBoost, LightGBM
* Excel (initial validation and business summaries)

---

## Project Structure

```
├── data/               # Raw and cleaned datasets
├── notebooks/          # EDA, forecasting, and modeling notebooks
├── results/            # Visualizations and summary outputs
├── README.md           # Project documentation
```

---

## Key Takeaway

This project demonstrates how **analytics translates into business value** when forecasting, modeling, and simulations are aligned with operational decisions like inventory planning and pricing.

---

## Author

**Swaraj Choudhary**
BS in Data Science & Applications
Indian Institute of Technology Madras

---

## Disclaimer

This project is based on a publicly available dataset and is intended solely for academic and learning purp
