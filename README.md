# Azure Data Engineering Pipeline: Ingestion to Visualization

## Overview

This project demonstrates an end-to-end data engineering workflow built using Microsoft Azure services. It showcases the process of ingesting, transforming, and visualizing data from multiple sources using a modular and scalable pipeline architecture.

The solution is centered around the **Medallion Architecture (Bronze, Silver, Gold)** and involves seamless data flow across ingestion, transformation, and visualization stages.

![image](https://github.com/user-attachments/assets/402b00fc-5dad-4407-b42b-3b1407cc15d1)

## Key Objectives

- Ingest data from structured and semi-structured sources (GitHub-hosted CSVs and SQL databases).
- Store raw data in **Azure Data Lake Storage Gen2** (Bronze layer).
- Perform transformations and enrichment using **Azure Databricks**, with support from external sources like MongoDB.
- Load the processed data into a curated zone (Silver and Gold layers).
- Enable downstream analytics using **Azure Synapse** and visualization tools like **Power BI**, **Tableau**, or **Microsoft Fabric**.

## Components Used

- **Azure Data Factory**: Orchestrates data pipelines and manages ingestion from multiple sources.
- **Azure Data Lake Gen2**: Stores both raw and processed data in a hierarchical namespace for scalable management.
- **Azure Databricks**: Executes transformation logic, joins, filtering, and enrichment using Spark-based processing.
- **MongoDB**: Serves as an enrichment source during data transformation.
- **Azure Synapse Analytics**: Enables query performance optimization and supports downstream business intelligence tools.
- **Power BI / Tableau / Fabric**: Used for interactive data visualization and reporting.

## Architecture Pattern

This project follows the **Medallion Architecture**:
- **Bronze Layer**: Raw, unfiltered data as ingested.
- **Silver Layer**: Cleaned, filtered, and joined datasets.
- **Gold Layer**: Aggregated, curated datasets ready for analytics and visualization.

## Highlights

- Built parameterized pipelines to automate ingestion across multiple files.
- Used lookup activities to decouple configuration from orchestration logic.
- Leveraged dynamic content and metadata-driven design for scalability.
- Demonstrates real-world data engineering practices such as staging, enrichment, and schema evolution handling.

---

For any queries/feedback, contact: Feroz Khan (ferozk@uw.edu)
