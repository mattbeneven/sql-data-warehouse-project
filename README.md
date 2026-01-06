# Data Warehouse and Analytics Project

## Overview

This project implements a modern SQL-based data warehouse and analytics solution designed to support analytical reporting and business decision-making. The project covers the full lifecycle from raw data ingestion and data modeling to analytical SQL queries that generate actionable business insights.
The repository demonstrates core data engineering and data analytics concepts, including data cleansing, dimensional modeling, and analytical SQL development, following best practices commonly used in production data warehouse environments.

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
The project follows a structured data warehousing approach designed for analytics use cases.
### Data Ingestion & Cleansing
- Raw data is imported from ERP and CRM CSV files into staging tables
- Data quality issues such as missing values, inconsistent formats, and duplicate records are identified and resolved prior to loading analytics tables
### Data Integration & Modeling
- Data from both source systems is integrated into a unified data model
- A user-friendly dimensional schema is created to support analytical queries
- Fact and dimension tables are designed to optimize query performance and usability for reporting
