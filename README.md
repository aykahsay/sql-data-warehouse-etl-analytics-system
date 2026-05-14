# 📊 SQL Data Warehouse & ETL Analytics System

An end-to-end **data engineering and analytics system** that transforms raw ERP and CRM data into a structured, analytics-ready **data warehouse** using SQL Server. The project implements

- ⚙️ **Automated ETL Pipelines** using Python / SSIS for scheduled and scalable data ingestion
- 🕒 **Slowly Changing Dimensions (SCD Type 2)** to track historical changes in customer and product data over time
- 🔄 **Real-Time Data Pipeline Integration** enabling near real-time analytics from source systems to the data warehouse
- 🏗️ Designed with modular architecture to support scalability and enterprise-level data processing

These enhancements simulate real-world data engineering systems used in modern analytics platforms.
a full **ETL pipeline, medallion architecture, and star schema modeling** to enable scalable business intelligence and decision-making.

---

## 🧠 Problem Statement

Organizations often store data across disconnected systems (ERP, CRM, spreadsheets), leading to:
- Data inconsistency
- Slow reporting cycles
- Poor decision-making visibility

This project builds a centralized **data warehouse system** that integrates, cleans, and structures data for analytics.

---

## 🏗️ Data Architecture (Medallion Design)

The system follows a **Bronze → Silver → Gold architecture**:

### 🥉 Bronze Layer (Raw Data Ingestion)
- Raw ERP and CRM data ingested from CSV files
- Stored in original format for traceability
---

### 🥈 Silver Layer (Cleaned & Standardized Data)
- Data cleaning (null handling, duplicates removal)
- Standardization of formats (dates, currency)
- Integration of ERP + CRM datasets via CustomerID

---

### 🥇 Gold Layer (Business-Ready Data)
- Star schema implementation
- Fact and dimension tables optimized for analytics
**📌 Architecture Overview:**
<img width="883" height="769" alt="image" src="https://github.com/user-attachments/assets/f06ccd68-6fb2-4595-986e-2df83319b22e" />


## ⚙️ ETL Pipeline

### 🔹 Extract
- Data extracted from ERP and CRM systems (CSV files)

### 🔹 Transform
- Data cleaning and preprocessing
- Schema alignment across sources
- Joins using CustomerID
- Data validation and consistency checks

### 🔹 Load
- Data loaded into staging tables
- Final loading into fact and dimension tables
📌 ETL Transformation Pipeline:
<img width="1256" height="752" alt="image" src="https://github.com/user-attachments/assets/b931be1b-4e02-4300-a2d0-8f218194134c" />
---

## 🧱 Data Modeling

Star Schema design:

- `FactSales`
- `DimCustomer`
- `DimProduct`
- `DimDate`
📌 Star Schema Data Model:
<img width="1252" height="775" alt="image" src="https://github.com/user-attachments/assets/f49be9ff-b1c5-4f3a-9363-9ea695070ca8" />

This enables:
- Fast analytical queries
- Simplified reporting logic
- Scalable BI integration

---

## 🧪 Data Quality Checks

- Missing value detection and handling
- Duplicate record removal
- Data type validation
- Referential integrity checks

---

## 📊 SQL Analytics

Business insights generated:

- Top 10 best-selling products by region
- Monthly sales trends
- Customer segmentation analysis
- Conversion funnel analysis

---

## 📈 Business Impact

This system enables organizations to:

- Reduce reporting time from hours → seconds
- Improve cross-department data consistency
- Enable real-time decision support
- Provide unified business visibility

---

## 🧰 Tools & Technologies

- SQL Server
- SSMS (SQL Server Management Studio)
- Draw.io / dbdiagram (Architecture design)
- Excel / CSV
- Power BI (optional visualization)

---

## 🚀 Future Improvements

-
- Integrate Power BI dashboards

---

## 📄 License

MIT License — free to use, modify, and extend.

---
