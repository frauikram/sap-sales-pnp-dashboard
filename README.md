# SAP Sales PnP Dashboard

A full SAC project featuring store sales analytics with performance KPIs and planning simulation for future periods.

This project demonstrates a **Planning and Performance (PnP)** dashboard using **SAP Analytics Cloud (SAC)** with real-world retail sales data. We walk through the entire workflow — from raw CSVs to a fully interactive dashboard — highlighting forecasting, planning, and KPI tracking.

---

## 📁 Project Folder Structure

```bash
sap-sales-pnp-dashboard/
├── data/                   # Cleaned and raw data CSVs
│   ├── train.csv
│   ├── stores.csv
│   ├── transactions.csv
│   └── sales_clean.csv
├── figures/                # Charts and SAC screenshots
├── notebooks/              # Data prep and forecasting notebooks
│   └── 01_clean_sales_data.ipynb
├── docs/                   # Setup and walkthroughs
├── README.md               # Project overview and setup instructions
```

---

## ✅ Completed Steps So Far

### 🔹 1. Dataset Preparation

- Source: Kaggle Store Sales Forecasting dataset
- Files used:
  - `train.csv` – Daily sales per store/product
  - `stores.csv` – Store metadata
  - `transactions.csv` – Daily footfall data

Files removed: `oil.csv`, `holidays_events.csv`, `test.csv`, `sample_submission.csv`

### 🔹 2. Environment Setup

- Managed using `pipenv`
- Required packages: `pandas`, `matplotlib`, `seaborn`, `jupyter`

### 🔹 3. Data Cleaning

- Merged `train.csv` with `stores.csv` and `transactions.csv`
- Cleaned missing values in transactions
- Added a `year_month` column for time aggregation
- Exported `sales_clean.csv` for SAP Analytics Cloud upload

```python
# Export command from notebook
sales_clean.to_csv('../data/sales_clean.csv', index=False)
```

---
