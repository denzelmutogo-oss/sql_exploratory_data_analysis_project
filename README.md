# 🔍 SQL Data Exploratory Analysis Project

**Business-Focused Data Exploration Using SQL Server**

---

## 📌 Project Overview

This project demonstrates a **structured, business-driven approach to data exploratory analysis (EDA)** using SQL Server. Rather than ad-hoc querying, the analysis is organized into reusable scripts that help analysts and stakeholders **understand the shape, quality, and business meaning of the data** before reporting or dashboard development.

The goal is to answer foundational business questions such as:

* What data do we have and how is it structured?
* What time periods does the data cover?
* Which dimensions and measures matter most to the business?
* Where are trends, outliers, or performance gaps?

This approach reflects how EDA is performed in **real BI and analytics workflows**, especially in healthcare, finance, and enterprise environments.

---

## 🗄️ Data Model Overview

The analysis is performed on **Gold-layer, analytics-ready tables**, ensuring results are consistent and business-aligned.

### Tables Used

* **gold.dim_customers** – Customer attributes used for segmentation and analysis
* **gold.dim_products** – Product hierarchy and descriptive attributes
* **gold.fact_sales** – Transaction-level sales measures used for KPI calculations

These tables are designed to support **trusted metrics, consistent dimensions, and repeatable analysis**.

---

## 📂 Repository Structure

```text
sql-data-exploration/
│
├── datasets/               # Reference to analytical tables
│   ├── gold.dim_customers
│   ├── gold.dim_products
│   └── gold.fact_sales
│
├── scripts/                # Exploratory analysis scripts
│   ├── init_database.sql
│   ├── database_exploration.sql
│   ├── dimensions_exploration.sql
│   ├── daterange_exploration.sql
│   ├── measures_exploration.sql
│   ├── magnitude_analysis.sql
│   └── ranking_analysis.sql
│
├── LICENSE                 # MIT License
└── README.md               # Project documentation
```

The structure encourages **repeatable analysis**, clarity, and easy onboarding for other analysts.

---

## 🧭 Analysis Breakdown

Each script focuses on a specific analytical objective commonly used in business intelligence.

### 1️⃣ Database Initialization

**Script:** `init_database.sql`

* Creates the analytics database and schemas
* Ensures a clean, controlled environment for analysis
* Reflects production-safe setup patterns (with clear warnings)

---

### 2️⃣ Database Exploration

**Script:** `database_exploration.sql`

* Identifies available tables and schemas
* Inspects column metadata and data types
* Helps analysts quickly understand what data exists and how it is structured

---

### 3️⃣ Dimensions Exploration

**Script:** `dimensions_exploration.sql`

* Reviews distinct values and attributes in dimension tables
* Validates business categories (customers, products, segments)
* Ensures dimensions are usable for filtering and grouping in BI tools

---

### 4️⃣ Date Range Exploration

**Script:** `daterange_exploration.sql`

* Determines minimum and maximum dates in fact data
* Evaluates historical coverage and data freshness
* Supports time-based reporting and trend analysis decisions

---

### 5️⃣ Measures Exploration

**Script:** `measures_exploration.sql`

* Calculates high-level metrics (counts, totals, averages)
* Provides quick insight into overall performance
* Helps validate KPI logic before dashboards are built

---

### 6️⃣ Magnitude Analysis

**Script:** `magnitude_analysis.sql`

* Groups measures by key dimensions
* Identifies distribution patterns across customers, products, or regions
* Supports business questions around scale and contribution

---

### 7️⃣ Ranking Analysis

**Script:** `ranking_analysis.sql`

* Ranks entities using window functions
* Identifies top performers and underperformers
* Supports prioritization and performance monitoring use cases

---

## 🛠️ SQL Techniques Used

* Aggregate functions: `SUM()`, `COUNT()`, `AVG()`
* Window functions: `RANK()`, `DENSE_RANK()`, `ROW_NUMBER()`
* Filtering and grouping: `GROUP BY`, `ORDER BY`
* Metadata inspection using `INFORMATION_SCHEMA`

---

## 🎯 Business Value

This project shows how structured SQL exploration:

* Builds **confidence in data before reporting**
* Reduces misinterpretation of KPIs
* Accelerates dashboard development in Tableau or Power BI
* Helps stakeholders understand trends, coverage, and performance drivers

It demonstrates not just SQL proficiency, but **analytical thinking and business awareness**.

---

## 👤 About Me

**Denzel Mutogo**
*Tableau Developer | Data Analyst | Business Intelligence*

I focus on using SQL and BI tools to transform data into **clear, actionable insights**. My work emphasizes structured analysis, trusted metrics, and business-ready datasets across **healthcare and finance** environments.

---

📄 **License:** MIT
