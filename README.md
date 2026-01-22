# 🔍 SQL Data Exploratory Analysis (EDA)

---

## 📌 Project Overview

This project focuses on **business-oriented exploratory data analysis (EDA)** using SQL Server. It represents the step that happens **before advanced analytics and dashboards**, where the goal is to understand what data exists, how reliable it is, and how it should be used for reporting.

Rather than running one-off queries, the analysis is organized into clear, repeatable SQL scripts that help answer foundational questions analysts and stakeholders typically ask early in a BI project.

---

## 🎯 Business Questions Addressed

This EDA work is designed to answer questions such as:

* What data is available and how is it structured?
* What time period does the data cover?
* Which dimensions and measures are most relevant for reporting?
* Are there obvious gaps, outliers, or inconsistencies?

These answers help prevent issues later when building dashboards or defining KPIs.

---

## 🗄️ Data Model Used

All exploration is performed on **Gold-layer, analytics-ready tables**, similar to what analysts would use in a production BI environment:

* **gold.dim_customers** – customer attributes for grouping and filtering
* **gold.dim_products** – product hierarchy and descriptive fields
* **gold.fact_sales** – transactional measures used for metrics

Using curated tables keeps exploration aligned with business definitions.

---

## 📂 Repository Structure

```text
sql-data-exploration/
│
├── scripts/                # Exploratory SQL scripts
│   ├── init_database.sql
│   ├── database_exploration.sql
│   ├── dimensions_exploration.sql
│   ├── daterange_exploration.sql
│   ├── measures_exploration.sql
│   ├── magnitude_analysis.sql
│   └── ranking_analysis.sql
│
├── LICENSE
└── README.md
```

---

## 🔍 Types of Analysis Included

* Database and schema exploration
* Dimension value validation
* Date range and data coverage checks
* High-level metric summaries
* Magnitude and distribution analysis
* Basic ranking to identify top and bottom performers

Each script focuses on a single purpose, making the analysis easy to follow and reuse.

---

## 🛠️ SQL Techniques Used

* Aggregations (`SUM`, `COUNT`, `AVG`)
* Window functions (`RANK`, `ROW_NUMBER`)
* Grouping and filtering logic
* Metadata inspection via `INFORMATION_SCHEMA`

---

## 📊 Business Value

In a BI workflow, this type of EDA:

* Builds confidence in the data before reporting begins
* Helps define which KPIs are realistic and meaningful
* Reduces rework during dashboard development
* Creates shared understanding between analysts and stakeholders

This project represents the **foundation step** that supports downstream advanced analytics and BI dashboards.

---

## 👤 About Me

**Denzel Mutogo**
Tableau Developer | Data Analyst | Business Intelligence

---

📄 **License:** MIT
