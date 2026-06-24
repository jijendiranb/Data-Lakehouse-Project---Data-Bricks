# 🚀 Modern Data Lakehouse on Databricks using Medallion Architecture

## 📋 Project Overview

This project demonstrates the design and implementation of a scalable Modern Data Lakehouse using Databricks, PySpark, Spark SQL, and Delta Lake following the Medallion Architecture (Bronze, Silver, Gold).

The solution ingests raw ERP and CRM datasets from CSV files, transforms them through multiple processing layers, and delivers business-ready dimensional models optimized for analytics and reporting.

The project also includes automated orchestration using Databricks Workflows, enabling end-to-end execution from data ingestion to Gold layer creation.

---

## 🎯 Project Objectives

* Build a scalable Data Lakehouse using Databricks and Delta Lake.
* Implement industry-standard Medallion Architecture.
* Develop robust ETL/ELT pipelines using PySpark and Spark SQL.
* Create modular and reusable transformation notebooks.
* Automate pipeline execution using Databricks Workflows and Jobs.
* Deliver analytics-ready dimensional models for reporting and business intelligence.

---

# 🏗️ Architecture Overview

The project follows the Medallion Architecture pattern:

## Bronze Layer (Raw Data)

* Ingest ERP and CRM CSV datasets.
* Store raw data in Delta format.
* Preserve source data with minimal transformations.
* Maintain auditability and traceability.

## Silver Layer (Cleansed & Conformed Data)

* Data quality validation.
* Standardization of formats and values.
* Null handling and cleansing.
* Deduplication.
* Business rule implementation.
* Creation of six curated Silver tables.

## Gold Layer (Business Layer)

Business-ready dimensional models optimized for analytics.

### Dimension Tables

* Dim Customer
* Dim Product

### Fact Tables

* Fact Sales

---

# ⚙️ Technology Stack

| Category             | Technology             |
| -------------------- | ---------------------- |
| Data Platform        | Databricks             |
| Processing Engine    | Apache Spark           |
| Programming Language | PySpark                |
| Query Language       | Spark SQL              |
| Storage Format       | Delta Lake             |
| Architecture         | Medallion Architecture |
| Orchestration        | Databricks Workflows   |
| Data Modeling        | Star Schema            |
| Version Control      | Git & GitHub           |
| Source Systems       | ERP & CRM CSV Files    |

---

# 📂 Repository Structure

```text
databricks-lakehouse-project/

├── notebooks/
│
├── bronze/
│   ├── bronze_erp_customers
│   ├── bronze_erp_products
│   └── bronze_crm_sales
│
├── silver/
│   ├── silver_customers
│   ├── silver_products
│   ├── silver_sales
│   ├── silver_locations
│   ├── silver_categories
│   └── silver_reference_data
│
├── gold/
│   ├── dim_customers
│   ├── dim_products
│   └── fact_sales
│
├── orchestration/
│   └── workflow_job
│
├── source_data/
│   ├── ERP
│   └── CRM
│
├── architecture/
│   └── medallion_architecture.png
│
└── README.md
```

---

# 🛠️ ETL/ELT Workflow

### Step 1: Data Ingestion

* Read ERP and CRM source files from CSV format.
* Load data into Bronze Delta tables.

### Step 2: Data Transformation

* Apply data quality checks.
* Handle missing values.
* Standardize columns and formats.
* Remove duplicates.
* Create curated Silver tables.

### Step 3: Business Modeling

* Build analytical Gold layer tables.
* Create Star Schema model.
* Generate Dimension and Fact tables.

### Step 4: Orchestration

* Execute notebooks through Databricks Workflows.
* Configure task dependencies.
* Automate end-to-end pipeline execution.

---

# 🚀 Key Features

### Delta Lake Implementation

* ACID Transactions
* Schema Enforcement
* Schema Evolution
* Time Travel Support

### Data Engineering Best Practices

* Layered Medallion Architecture
* Modular Notebook Design
* Reusable Transformation Logic
* Data Quality Validation

### Workflow Automation

* Databricks Workflows
* Job Scheduling
* Dependency Management
* End-to-End Pipeline Automation

### Data Modeling

* Star Schema Design
* Fact and Dimension Modeling
* Analytics-Optimized Tables

---

# 🏆 Project Outcome

Successfully designed and implemented a production-style Modern Data Lakehouse solution using Databricks and Delta Lake.

The solution automates the complete data lifecycle from raw ingestion to business-ready analytics datasets while following industry-standard Medallion Architecture principles and modern Data Engineering best practices.

---

## 📄 License

This project is licensed under the MIT License.

