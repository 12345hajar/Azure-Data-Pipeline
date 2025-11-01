# 📘 Azure Data Pipeline – End-to-End Data Engineering Project

## 🧭 Overview

This project demonstrates a **complete end-to-end data engineering pipeline** built on **Microsoft Azure**.
It covers the entire data lifecycle — from ingestion to transformation and reporting — using **Azure Data Factory, Azure Databricks, Synapse Analytics, and Power BI**.

The goal is to design a **modern data architecture** that ensures scalability, automation, and efficient analytics on cloud-based data.

---![pipeline](https://github.com/user-attachments/assets/aec58a42-ae80-427b-85da-7b66290a2b60)


## 🏗️ Architecture Diagram



**Layers Explanation:**

| Layer                              | Description                                            | Azure Service Used      |
| ---------------------------------- | ------------------------------------------------------ | ----------------------- |
| **Data Source**                    | Public dataset accessed through HTTP API               | HTTP                    |
| **Ingestion (Bronze)**             | Raw data ingestion into Data Lake Gen2 using pipelines | Azure Data Factory      |
| **Transformation (Silver & Gold)** | Data cleaning, normalization, and aggregation          | Azure Databricks        |
| **Serving**                        | Processed data stored and queried for reporting        | Azure Synapse Analytics |
| **Reporting**                       | Interactive dashboards and visualizations             | Power BI                |

---

## ⚙️ Tools & Technologies

| Category                        | Tools                                  |
| ------------------------------- | -------------------------------------- |
| **Cloud Platform**              | Microsoft Azure                        |
| **Storage**                     | Azure Data Lake Storage Gen2           |
| **Orchestration**               | Azure Data Factory                     |
| **Processing & Transformation** | Azure Databricks (PySpark)             |
| **Data Serving**                | Azure Synapse Analytics                |
| **Visualization**               | Power BI                               |
| **Languages**                   | Python, SQL, Spark SQL                 |

---

## 🔄 Data Flow Description

1. **Ingestion – Azure Data Factory**
   * Ingest data from an **HTTP API** (e.g., AdventureWorks dataset)
   * Store raw data in **Bronze layer** (Parquet format) in **Data Lake Gen2**

2. **Transformation – Azure Databricks**
   * Clean and structure data in **Silver & Gold layers**
   * Save transformed data back to Data Lake for consumption

3. **Serving – Azure Synapse Analytics**
   * Create external tables/views pointing to Gold layer
   * Execute queries for  BI

4. **Reporting – Power BI**
   * Connect to Synapse 
   * Build interactive dashboards for business insights

---


