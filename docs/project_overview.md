# Flight Data Engineering Pipeline

## Overview

This project implements an end-to-end data engineering pipeline for processing and analyzing flight performance data.

The objective is to build a scalable data platform that ingests raw flight data, processes it using distributed computing, stores optimized datasets, and enables analytical querying.

The pipeline follows a data lake architecture using Apache Airflow, PySpark, Amazon S3, AWS Glue, and Amazon Athena.

---

## Business Problem

Airlines generate large volumes of flight operational data including schedules, delays, cancellations, and route information.

Business teams need reliable and optimized datasets to analyze:

- Flight delay patterns
- Airline performance
- Airport efficiency
- Route-level insights
- Cancellation trends

Raw CSV files are difficult to manage and query efficiently at scale.

---

## Project Goals

The main goals of this project are:

- Build an automated data ingestion pipeline
- Store raw data in a cloud data lake
- Process large datasets using PySpark
- Convert raw files into optimized Parquet format
- Implement partitioned storage
- Create analytics-ready datasets
- Enable SQL analysis using Amazon Athena

---

## Key Technologies

- Python
- Apache Airflow
- Apache Spark (PySpark)
- Amazon S3
- AWS Glue
- AWS Glue Data Catalog
- Amazon Athena
- Parquet

---

## High Level Flow

Raw Dataset  
→ Amazon S3 (Bronze Layer)  
→ PySpark Transformation  
→ Parquet (Silver Layer)  
→ Aggregation Layer (Gold)  
→ Athena Analytics