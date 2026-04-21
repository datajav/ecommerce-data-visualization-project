# 🛒 E-Commerce Customer Analytics Dashboard

> A full-stack analytics project combining Python-powered data preprocessing and a customer segmentation engine with Power BI for interactive business intelligence — built on a synthetic e-commerce dataset.

---

## 📌 Project Overview

This repository delivers a comprehensive customer behavior and sales performance analysis pipeline. It ingests a synthetic e-commerce dataset across four key dimensions and transforms it into actionable business insights via an interactive Power BI dashboard.

| Data Layer | Fields |
|---|---|
| 👤 Customer Demographics | Customer ID, gender, age |
| 🛍️ Product Information | Product ID, name, category |
| 🧾 Transaction Details | Order date, quantity, price |
| ⭐ Customer Experience | Payment method, review score, city |

---

## 🔬 Analysis Scope

The dashboard delivers multi-dimensional insights across five areas:

- **Sales Overview** — Revenue trends and order volume over time
- **Customer Demographics** — Age group and gender segmentation
- **Geographic Analysis** — Sales distribution by city and region
- **Product Performance** — Top-selling categories and individual products
- **Customer Satisfaction & Loyalty** — Review scores and retention metrics

---

## 🧠 Customer Segmentation Engine *(Jupyter Notebook)*

A standalone segmentation engine was built in Jupyter Notebook to classify customers into meaningful behavioral segments, feeding directly into the Power BI dashboard.

**What it does:**
- Groups customers by purchasing frequency, spend, and recency (RFM-style logic)
- Creates labeled segments such as high-value returners, one-time buyers, and at-risk customers
- Outputs a clean `.csv` that Power BI consumes for segment-level filtering and visuals

**Key steps in the notebook:**
```
1. Load & clean raw transaction data
2. Engineer RFM-style features per customer
3. Apply segmentation logic (binning / clustering)
4. Assign segment labels and export to /data/customer_segments.csv
```

> 📓 See [`notebooks/customer_segmentation.ipynb`](notebooks/customer_segmentation.ipynb) for the full implementation.

---

## 📊 Executive Summary

Key findings surfaced from the analysis:

| Metric | Finding |
|---|---|
| 📅 Peak Sales Month | December 2024 recorded the highest item quantities sold |
| 🏆 Top Category | Electronics contributed the most to overall revenue |
| 💳 Avg. Order Value | $87.76 — indicating stable, consistent purchase behavior |
| 👴 Top Spending Bracket | Age 60–70 showed the strongest purchasing power |
| 🚺 Gender Breakdown | Female customers made 44.56% more purchases |
| 🏙️ Top Cities | East Robert, South Tonya, and Port Melissaborough led in revenue |
| ⭐ Avg. Review Score | 3.99 / 5 — reflecting relatively positive customer feedback |

---

## 🛠️ Technical Implementation

### Python Pipeline

```
Raw Data → Data Wrangler → Feature Engineering → Statistical Analysis → CSV Export → Power BI
```

| Step | Tool | Details |
|---|---|---|
| Data Cleaning | Data Wrangler | Remove duplicates, handle missing values |
| Feature Engineering | Pandas | Age groups, customer segments, calculated fields |
| Statistical Analysis | Pandas, NumPy | Deeper behavioral insights |
| Segmentation Engine | Scikit-learn / custom logic | RFM-based customer classification |
| Export | Pandas `.to_csv()` | Processed data piped into Power BI |

### Power BI Layer

- DAX (Data Analysis Expressions) for calculated measures
- Power Query M Language for data transformation
- Data visualization best practices for executive-facing reporting

---

## 📈 Key Visualizations

- 📉 Time-series analysis of sales performance
- 🗺️ Geographic distribution maps
- 🌳 Product category treemaps
- 👥 Customer demographic breakdowns
- ⭐ Review score distribution analysis
- 💳 Payment method comparison

---

## 💼 Business Applications

| Use Case | Description |
|---|---|
| 🎯 Targeted Marketing | Segment-driven campaign personalization |
| 🔄 Customer Retention | Loyalty programs for high-value returning customers |
| 📦 Demand Forecasting | Predict product demand by category and region |
| 🌍 Geographic Expansion | Identify high-growth cities for investment |

---

## 🚀 Recommendations

### 1. Improve Customer Retention
- Offer personalized promotions based on purchasing behavior from the segmentation engine
- Implement a loyalty program targeting high-value returning customers
- Address low review scores by identifying common customer pain points

### 2. Optimize Marketing Efforts
- Focus campaigns on the top-performing 60–70 age segment
- Enhance regional targeting by investing in high-growth cities

### 3. Streamline Product Offerings
- Prioritize stocking best-selling categories (Electronics)
- Discontinue underperforming items based on category treemap analysis
- Refine pricing strategies using demand and spending pattern data

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data%20Analysis-yellow?style=flat)

---

## 📁 Project Structure

```
ecommerce-analytics/
├── data/
│   ├── synthetic_online_retail_data                    # Original synthetic dataset
│   └── cleaned_and_uncleaned_data_from_data_wrangler
│   └── customer_segments.csv 
├── notebooks/
│   └── customer_segmentation.ipynb # 🧠 Segmentation engine
|   └── Project_1.ipynb 
├── powerbi/
│   └── Project_1.pbix          # Power BI report file
└── README.md
```