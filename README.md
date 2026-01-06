# Data Warehouse and Analytics Project

## Overview

This project is a hands-on implementation of a modern SQL-based data warehouse and analytics workflow, built to reinforce core data engineering and data analytics concepts. The project walks through the full lifecycle of transforming raw operational data into analytics-ready datasets, from data ingestion and cleansing to dimensional modeling and analytical SQL development.

### Key Features
- End-to-end SQL-based data warehouse design
- Data cleansing and quality enforcement prior to analysis
- Dimensional modeling optimized for analytics
- Business-focused analytical SQL queries

## Tools & Technologies

- Database: SQL Server
- Languages: SQL
- Data Modeling: Dimensional modeling (fact and dimension tables)
- Analytics: SQL-based analytical queries
- Data Sources: CSV files (ERP and CRM systems)

## Data Sources

The data used in this project comes from two source systems:
- ERP system: Sales transactions and product-related data
- CRM system: Customer and customer attribute data
Both sources are provided as CSV files and represent the latest snapshot of operational data. Historical tracking is intentionally out of scope to focus on analytical modeling and querying.

## Data Warehouse Architecture

This project follows a Medallion Architecture approach with Bronze, Silver, and Gold layers, simulating a modern data warehouse workflow.
### High-Level Architecture
Sources → Data Warehouse → Consumption
### 1. Bronze Layer – Raw Data
- Stores data as-is from source systems (CSV files from ERP and CRM)
- Ingested into SQL Server using batch processing (truncate & insert)
- No transformations applied; retains original structure
### 2. Silver Layer – Cleaned & Standardized Data
- Performs data cleansing, standardization, normalization, and enrichment
- Adds derived columns to improve analytics readiness
- Batch loading with truncate & insert
- Data remains in table format, optimized for intermediate processing
### 3. Gold Layer – Business-Ready Data
- Stores curated, analytics-ready datasets in star schema format
- Includes fact and dimension tables, aggregated tables, and views
- Applies business logic, integrations, and aggregations
- Used for reporting, ad-hoc SQL queries, and analytics


The Gold layer enables downstream use cases such as:
Power BI dashboards and other BI tools
Ad-hoc SQL analysis for decision-making
Basic machine learning and analytical workflows
