# Retail Data Engineering Pipeline

## Project Overview

This project demonstrates an end-to-end Retail Data Engineering Pipeline built using Databricks, PySpark, Delta Lake, and Power BI. The pipeline ingests raw retail datasets, processes them through Bronze, Silver, and Gold layers using Medallion Architecture, and delivers business-ready analytics dashboards in Power BI.

The project focuses on scalable ETL/ELT processing, data quality validation, incremental loading, and analytics reporting for retail sales data.

---

# Architecture

CSV Files → Bronze Layer → Silver Layer → Gold Layer → Databricks Cluster → Power BI Dashboard

### Layers

## Bronze Layer

* Raw data ingestion from CSV files
* Minimal transformations
* Schema enforcement
* Initial data validation

## Silver Layer

* Data cleansing and standardization
* Null handling and deduplication
* Business transformations
* Incremental processing

## Gold Layer

* Business-ready aggregated tables
* KPI-focused datasets
* Reporting and analytics tables
* Optimized for Power BI consumption

---

# Technologies Used

| Technology   | Purpose                           |
| ------------ | --------------------------------- |
| Databricks   | Data processing platform          |
| PySpark      | Distributed data transformations  |
| Delta Lake   | ACID-compliant storage            |
| Python       | ETL scripting                     |
| SQL          | Data querying and transformations |
| Power BI     | Dashboarding and visualization    |
| Git & GitHub | Version control                   |

---

# Pipeline Flow

1. Load raw CSV retail datasets into Databricks.
2. Store raw data in Bronze tables.
3. Clean and transform data into Silver tables.
4. Create business aggregations in Gold tables.
5. Connect Databricks tables to Power BI.
6. Build interactive dashboards for analytics.

---

# Key Features

* End-to-end ETL pipeline using Medallion Architecture
* PySpark-based scalable transformations
* Incremental loading support
* Data validation and reconciliation
* Delta Lake implementation
* Power BI dashboard integration
* Modular notebook structure

---

# Power BI Dashboard

### Dashboard Includes

* Total Sales KPI
* Region-wise Sales Analysis
* Product Category Analysis
* Channel-wise Sales Distribution
* Monthly Sales Trends

---

# Screenshots

Add your screenshots in the `screenshots/` folder.

Recommended screenshots:

* Databricks workspace
* Bronze/Silver/Gold tables
* Notebook execution
* Cluster configuration
* Power BI dashboard
* Architecture diagram

Example:

```text
screenshots/
├── bronze_table.png
├── silver_table.png
├── gold_table.png
├── powerbi_dashboard.png
└── architecture.png
```

---

# Steps to Run

## Step 1 — Upload Dataset

Upload CSV retail datasets into Databricks FileStore or Volume.

## Step 2 — Run Bronze Notebook

Execute Bronze notebook to ingest raw data.

## Step 3 — Run Silver Notebook

Execute Silver notebook for cleansing and transformations.

## Step 4 — Run Gold Notebook

Execute Gold notebook to generate analytics-ready tables.

## Step 5 — Start Databricks Cluster

Start your Databricks compute cluster.

## Step 6 — Connect to Power BI

* Copy JDBC/ODBC connection details
* Generate Personal Access Token
* Connect using Azure Databricks connector in Power BI

## Step 7 — Build Dashboard

Use Gold tables to create KPIs and visualizations.

---

# Future Enhancements

* Real-time streaming using Kafka
* Automated orchestration with Airflow
* CI/CD deployment pipelines
* Data quality monitoring framework
* dbt integration

---

# Author

Nagavishwas T N

LinkedIn: linkedin.com/in/nagavishwas
