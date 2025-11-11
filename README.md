# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀  
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

---
## 🏗️ Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:

<img width="1062" height="650" alt="image" src="https://github.com/user-attachments/assets/8aaa3865-a747-417a-bd80-aef6212d63b9" />

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

---
## 📖 Project Overview

This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.

🎯 This repository is an excellent showcase expertise in:
- SQL Development
- Data Architect
- Data Engineering  
- ETL Pipeline Developer  
- Data Modeling  
- Data Analytics  
---

## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

#### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

---

### BI: Analytics & Reporting (Data Analysis)

#### Objective
Develop SQL-based analytics to deliver detailed insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

## 📂 Repository Structure
```
data-warehouse-project/
│
├── datasets/                           # Source data folders used for ingestion
│   ├── source_crm/                     # Contains CRM (Customer Relationship Management) raw data
│   └── source_erp/                     # Contains ERP (Enterprise Resource Planning) raw data
│
├── scripts/                            # SQL scripts for database setup and ETL processing
│   ├── bronze/                         # Scripts for creating and loading raw (bronze) layer tables
│   │   ├── ddl_bronze.sql              # DDL script for defining bronze tables
│   │   └── proc_load_bronze.sql        # Procedure for loading raw data into bronze layer
│   │
│   ├── silver/                         # Scripts for transforming and cleaning data (silver layer)
│   │   ├── ddl_silver.sql
        └── proc_load_silver.sql
│   │
│   ├── gold/                           # Scripts for creating curated analytical (gold) layer tables
│   │   └── ddl_gold.sql                # DDL script for defining gold layer tables
│   │
│   └── init_database.sql               # Script for initializing database and schema setup
│
├── tests/                              # SQL scripts for data validation and quality assurance
│   ├── quality_checks_gold.sql         # Quality tests for gold layer data
│   └── quality_checks_silver.sql       # Quality tests for silver layer data
│
├── LICENSE                             # License information for the project
├── README.md                           # Project overview and setup instructions

---
