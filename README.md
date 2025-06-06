
# 📊 SQL Data Warehousing Project

This repository contains a complete end-to-end SQL Data Warehousing pipeline that demonstrates the full ETL and dimensional modeling process, from raw data ingestion to final reporting-ready gold layer.

It covers all major stages of a modern data warehouse architecture: Bronze, Silver, and Gold layers with multiple SQL scripts and real-world sample datasets.

---

## 🏗️ Project Architecture

The data warehouse is built using a multi-layered approach:

1️⃣ **Bronze Layer (Raw Ingestion Layer):**  
   - Raw data ingestion from CRM and ERP source files.
   - Scripts: 
     - `bronze/init_database.sql`
     - `bronze/ddl-bronze.sql`
     - `bronze/procedure_load_bronze.sql`

2️⃣ **Silver Layer (Cleansed & Standardized Layer):**  
   - Data transformations, cleaning, and standardization.
   - Scripts: 
     - `silver/ddl_silver.sql`
     - `silver/proc_load_silver.sql`

3️⃣ **Gold Layer (Business-Ready Layer):**  
   - Dimensional modeling with fact and dimension tables.
   - Script:
     - `gold/ddl_gold.sql`

---

## 📂 Folder Structure

```bash
datasets/
    CRM/    --> CRM source files (cust_info.csv, prd_info.csv, sales_details.csv)
    ERP/    --> ERP source files (cust_az12.csv, loc_a101.csv, px_cat_g1v2.csv)

scripts/
    bronze/ --> Bronze layer DDL and load procedures
    silver/ --> Silver layer DDL and procedures
    gold/   --> Gold layer dimensional modeling
```

---

## 📌 Topics Covered

- SQL Data Warehousing
- ETL Pipeline Development
- Bronze-Silver-Gold Architecture
- Data Cleansing & Standardization
- Dimensional Modeling (Facts and Dimensions)
- SQL Stored Procedures
- Staging and Incremental Loads

---

## 💡 Datasets

- CRM data (customers, products, sales)
- ERP data (customer master, locations, product categories)

---

## 🔧 Requirements

- Microsoft SQL Server
- SQL Server Management Studio (SSMS)
- CSV datasets located under `/datasets/` folder

---

## 🧠 Author Notes

This project serves as a comprehensive demonstration of data warehousing principles and SQL-based ETL pipelines, showcasing both the technical and business aspects of modern data architecture.

---

📌 **Tip:** Run each layer in sequence:  
**Bronze → Silver → Gold** for proper end-to-end pipeline setup.
