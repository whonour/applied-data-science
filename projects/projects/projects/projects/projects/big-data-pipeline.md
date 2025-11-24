---
layout: page
title: "Big Data Pipeline: NiFi → HDFS → Hive → Spark ML → HBase"
permalink: /projects/big-data-pipeline/
---

# Big Data Pipeline: NiFi → HDFS → Hive → Spark ML → HBase

![Big Data Pipeline Diagram](../assets/img/bigdata-pipeline-diagram.png)

[![Apache NiFi](https://img.shields.io/badge/ETL-Apache%20NiFi-blue.svg)]()
[![Spark](https://img.shields.io/badge/Compute-Apache%20Spark-orange.svg)]()
[![HBase](https://img.shields.io/badge/Store-HBase-red.svg)]()

End-to-end big data pipeline built for the `ml_sample_customers` dataset, connecting ingestion, storage, query, modeling, and metric persistence. :contentReference[oaicite:16]{index=16}

## 🧱 Components

1. **NiFi → HDFS**  
   - ListFile / FetchFile to ingest `ml_sample_customers.csv`  
   - UpdateAttribute to standardize metadata  
   - PutHDFS to write into `/user/william/week11/ml_sample_customers/`  

2. **Hive Managed Table**  
   - Hive schema modeled around customer ID, demographics, and behavioral features  
   - Managed table so Hive controls lifecycle in the warehouse  
   - Aggregation queries to validate schema & data load  

3. **Environment Setup & HBase Thrift**  
   - Installed Python dependencies (`numpy`, `pandas`, `happybase`, etc.)  
   - Started HBase Thrift server to allow Spark → HBase communication  

4. **PySpark ML Pipeline**  
   - Supervised learning (e.g., churn/response prediction)  
   - Stages: missing-value handling, feature vectorization, categorical indexing, Random Forest / GBT classifier  
   - Evaluated with accuracy, precision, recall, F1  

5. **HBase Metrics Table**  
   - Composite row key: `run_id#timestamp` for scan-friendly ordering  
   - Single column family (e.g., `cf`) with columns: `accuracy`, `precision`, `recall`, `f1`, etc.  

6. **End-to-End Validation**  
   - HBase `scan` command confirms metrics written per run  
   - Demonstrates fully working NiFi → HDFS → Hive → Spark → HBase pipeline. :contentReference[oaicite:17]{index=17}  

## 📂 Repository

- *(Add your Week 11 big data repo link here)*

## 📄 Supporting Docs

- Week 11 Explanations PDF  
- NiFi screenshots  
- Hive DDL & queries  
- Spark ML code  
- HBase create/scan commands
