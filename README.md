# E-commerce-Event-Driven-Data-Pipeline

Project Overview

This project implements a production-grade, event-driven data pipeline for an e-commerce platform using Databricks and Delta Lake. The pipeline processes data from multiple business domains, ensures high data quality, maintains historical changes, and delivers analytics-ready datasets for business intelligence.

The solution follows modern data engineering best practices, including schema enforcement, data validation, SCD Type 2 handling, automated orchestration, and monitoring.
<img width="3058" height="1630" alt="image" src="https://github.com/user-attachments/assets/36ef7464-28e1-4b71-8d06-80e9cc2fdd91" />


# E-commerce Event-Driven Data Pipeline

## 📌 Project Overview
This project demonstrates an **industrial-grade, event-driven data pipeline** for an e-commerce platform. It is designed to ingest, validate, enrich, and analyze data from multiple business domains using modern **lakehouse architecture** principles.

The pipeline is **scalable, fault-tolerant, and production-ready**, leveraging Databricks-native services for orchestration, storage, and analytics.

---

## 🛠️ Tech Stack
- Databricks  
- PySpark  
- Delta Lake  
- Databricks Volumes  
- Databricks Workflows  
- GitHub  

---

## 🔄 Key Features & Architecture

### 1️⃣ Multi-Source Data Ingestion Pipeline
- Ingests data from multiple domains:
  - Orders  
  - Customers  
  - Products  
  - Inventory  
  - Shipping  
- Source data loaded from **Databricks Volumes**
- Automated file-based ingestion with schema validation
- Supports batch and incremental processing

---

### 2️⃣ Advanced Data Validation & Quality Assurance
- Cross-table validation across staging datasets
- Business rule validation:
  - Null checks  
  - Referential integrity  
  - Value range validation  
- Data quality scoring with severity levels:
  - Critical  
  - Warning  
  - Informational  
- Centralized error logging and validation metrics

---

### 3️⃣ Data Enrichment & Business Intelligence
- Customer segmentation based on purchase behavior
- Product performance analysis
- Seasonal trend analysis
- Customer Lifetime Value (CLV) calculation
- Analytics-ready enriched datasets

---

### 4️⃣ SCD Type 2 Implementation
- Implements **Slowly Changing Dimension (SCD) Type 2**
- Maintains full historical tracking using:
  - Effective start date  
  - Expiry date  
  - Active record flag  
- Automated `MERGE` operations using Delta Lake

---

### 5️⃣ Automated File Management
- Source file archiving after successful processing
- Batch tracking using unique batch IDs
- Error file segregation for failed records
- End-to-end processing status monitoring

---

### 6️⃣ Analytics & Reporting Layer
- Real-time analytics summary tables
- Customer segment insights
- Product performance KPIs
- Business metrics ready for BI consumption

---

### 7️⃣ Event-Driven Workflow Orchestration
- Pipeline triggered using **JSON control files**
- Sequential notebook execution via **Databricks Workflows**
- Centralized monitoring and execution logs
- Designed for near real-time and scheduled batch runs

---

## 📊 Outcome
This project showcases a **production-ready, event-driven lakehouse pipeline** suitable for real-world e-commerce analytics, with strong focus on data quality, historical accuracy, and business intelligence.

---

## 📁 Repository Structure


Project 1 : E-commerce Event-Driven Data Pipeline (Industrial Project) Tech Stack: Databricks, PySpark, Delta Lake, Databricks Volumes, Databricks Workflows, GitHub

→ Multi-Source Data Ingestion Pipeline - Process orders, customers, products, inventory, and shipping data from Databricks Volumes with automated file-based loading and schema validation

→ Advanced Data Validation & Quality Assurance - Cross-reference validation across staging tables, business rule validation, and comprehensive data integrity checks with severity-based scoring

→ Data Enrichment & Business Intelligence - Customer segmentation, product performance analysis, seasonal trends, and Customer Lifetime Value (CLV) calculations

→ SCD2 Implementation - Slowly Changing Dimension Type 2 logic for maintaining historical data with effective/expiry date tracking and automated merge operations

→ Automated File Management - Source file archiving after processing, batch tracking, error logging, and processing status monitoring

→ Analytics Dashboard - Real-time analytics summary tables, customer segment analysis, product performance tracking, and business KPIs

→ Event-Driven Workflow Orchestration - JSON trigger files for batch processing, sequential notebook execution, and comprehensive pipeline monitoring
