# SAP Sales PnP Dashboard

A full SAP Analytics Cloud (SAC) project featuring store sales analytics with performance KPIs and planning simulation for future periods.

This project demonstrates a **Performance and Planning (PnP)** dashboard using **SAP Analytics Cloud (SAC)** with real-world retail sales data. We walk through the entire workflow — from raw CSVs to a fully interactive dashboard — highlighting forecasting, planning, and KPI tracking.

---

## 📁 Project Folder Structure

```bash
sap-sales-pnp-dashboard/
├── data/                   # Cleaned and raw data CSVs
│   ├── train.csv
│   ├── stores.csv
│   ├── transactions.csv
│   └── sales_clean.csv
│   ├── target_sales_city.csv
├── figures/                # Charts and SAC screenshots
│   ├── performance-total_sales.png
│   ├── performance-sales_by_store.png
│   ├── performance-top_products.png
│   ├── performance-monthy_sales.png
│   ├── planning-actual_target_variance.png
├── notebooks/              # Data prep and forecasting notebooks
│   ├── 01_clean_sales_data.ipynb
│   └── 02_generate_target_sales_by_city.ipynb
├── docs/                   # Exported SAC dashboard as PDF
│   └── sap_sales_pnp_dashboard_preview.pdf
├── README.md               # Project overview and setup instructions
```

---

## ✅ Project Summary

**Goal:** Build an interactive dashboard that shows store sales performance and compares it with planning targets using SAP Analytics Cloud.

**Key Features:**

- Data preparation using Python (pandas, Jupyter)
- Forecasted targets by city
- SAC dashboard with KPI cards, blended charts, planning table

---

## 🔄 Workflow Summary


### 0. Environment Setup

- Managed using `pipenv`
- Required packages: `pandas`, `matplotlib`, `seaborn`, `jupyter`

### 1. Data Cleaning

- Source: Kaggle Store Sales Forecasting dataset
- Files used:
  - `train.csv` – Daily sales per store/product
  - `stores.csv` – Store metadata
  - `transactions.csv` – Daily store footfall
- Merged and cleaned to create `sales_clean.csv`

### 2. Forecast Target Generation

- Aggregated average 2017 sales by city
- Simulated targets with `avg_sales`
- Output saved as `target_sales_city.csv`

### 3. SAP Analytics Cloud Setup

- Activated free SAC trial (14 days)
- Uploaded `sales_clean.csv` → `sales_model`
- Uploaded `target_sales_city.csv` → `target_model`
- Created blended dataset on `city`
- Designed the dashboard with:
  - Performance KPIs:
    - Total Sales, Sales Distribution by Stores, Top Products, Monthly Sales
  - Planning KPI:
    - Actual sales vs target (+/- variance)

### 4. Final Dashboard Export

- Dashboard exported as PDF (see `docs/`)
- Screenshots saved in `figures/`

---

## 📊 Tools Used

- Python (Jupyter, pandas)
- SAP Analytics Cloud (modeling, story building)
- GitHub (portfolio packaging)

---

## 📝 Author Notes

This project is part of my analytics portfolio to demonstrate:

- Forecasting and planning skills
- Enterprise BI tool experience (SAC)
- Dashboard development for stakeholders

> Built with 💡 and coffee.

---

## 🔗 Medium Blog Post

A full narrative blog post will accompany this repo. Stay tuned!

