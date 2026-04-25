# 🍽️ Egyptian Restaurant Analytics — End-to-End Data Pipeline & Dashboard

> **Transforming 1.5 GB of raw restaurant data into actionable business decisions using a modern data stack.**

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Fivetran](https://img.shields.io/badge/Fivetran-0073E6?style=for-the-badge&logo=fivetran&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

---

## 📌 Project Overview

This project delivers a full end-to-end analytics solution for a **multi-branch Egyptian restaurant chain**. The pipeline ingests raw transactional data from multiple sources, processes it at scale using Databricks SQL, and visualizes the results in an interactive Power BI dashboard — enabling data-driven decisions across operations, sales, and customer experience.

---

## 📊 Dashboard Preview

| Overview Page | Sales Page |
|:---:|:---:|
| ![Overview](Dashboard/Overview.png) | ![Sales](Dashboard/Sales.png) |

---

## 🗂️ Dataset

| Property | Details |
|---|---|
| **Total Rows** | 11,000,000+ |
| **Source Files** | 7 CSV files + 2 JSON files |
| **Total Size** | ~1.5 GB |
| **Source Location** | Google Drive |
| **Time Range** | 2020 – 2025 |

---

## ⚙️ Tech Stack

| Layer | Tool |
|---|---|
| **Data Ingestion** | Fivetran (Google Drive → Databricks) |
| **Data Processing** | Databricks (SQL / ELT) |
| **Data Modeling** | Star Schema on Databricks |
| **Visualization** | Power BI |

---

## 🔄 Pipeline Architecture

```
Google Drive (CSV + JSON)
        │
        ▼
   [Fivetran]  ── Automated Ingestion
        │
        ▼
  [Databricks]
   ├── Raw Layer     → Landing zone for source data
   ├── Silver Layer  → Cleaned & standardized tables
   └── Gold Layer    → Business-ready data models
        │
        ▼
   [Power BI]  ── Interactive Dashboard
```

---

## 📈 Key Insights

### 💰 Revenue & Orders
- **Total Revenue:** 2.90 Billion EGP from **11 Million orders**
- **Average Order Value (AOV):** 261 EGP — a healthy indicator of basket size
- **Top Branch:** Cairo leads significantly at ~3.8M orders, highlighting a load-balancing opportunity

### ⭐ Customer Satisfaction
- Majority of orders (6.2M) are rated **4 stars** — solid but with clear room to reach 5
- Only 0.9M orders rated 5 stars — a key area for service improvement

### 💳 Payment Methods
| Method | Share |
|---|---|
| Cash | ~50% |
| Card | ~30% |
| Wallet | ~20% |

> 50% cash dependency signals a strong opportunity for **digital payment adoption**.

### 🛵 Order Type Breakdown
| Type | Revenue Share |
|---|---|
| Dine-in | ~40% |
| Takeaway | ~30% |
| Delivery | ~30% |

### 🥩 Top Revenue Categories
1. **مشويات (Grills)** — 1.01 Billion EGP
2. **طواجن (Tagines)** — 0.81 Billion EGP
3. **محاشي (Stuffed Dishes)** — 0.54 Billion EGP

### 📅 Order Trends (2020–2025)
- Decline in **2022** → gradual recovery through **2024**
- Early signs of a **2025 dip** → warrants deeper seasonality analysis

### 🕘 Peak Hours
- Orders surge between **8 PM and 10 PM** — critical window for staffing and kitchen capacity optimization

---

## 💡 Business Recommendations

| # | Recommendation | Priority |
|---|---|---|
| 1 | **Load balance** across branches, especially Cairo | 🔴 High |
| 2 | **Improve service quality** to push ratings from 4 → 5 stars | 🔴 High |
| 3 | **Incentivize digital payments** to reduce cash dependency | 🟡 Medium |
| 4 | **Scale Delivery channel** to improve reach and revenue growth | 🟡 Medium |
| 5 | **Leverage top categories** (Grills, Tagines) in marketing campaigns | 🟢 Low |
| 6 | **Investigate 2025 trend dip** — seasonality vs. market shift analysis | 🔴 High |

---

## 👤 Author

**[Mohamed Magdy]**  
Data Engineer | Analytics Enthusiast  

---

> *"It's not about the size of the data — it's about the decisions you extract from it."*
