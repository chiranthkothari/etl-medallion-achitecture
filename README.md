# ETL Pipeline with Medallion Architecture (CRM + ERP Data)
This project implements a complete ETL pipeline using the Medallion architecture (Bronze, Silver, Gold layers) to process CRM and ERP data. The pipeline is built using Azure Data Lake for storage and Databricks for processing and transformation.

## Data architecture
The data architecture for this project follows Medallion Architecture Bronze, Silver, and Gold layers:

<img width="881" alt="Screenshot 2025-05-28 at 10 39 17 PM" src="https://github.com/user-attachments/assets/a334b0da-d7ef-47e7-a5ae-23ca731c935f" />

* **Bronze Layer**: Stores raw data as-is from the source systems. Data is loaded here from data folder of this rrepository using Azure data factory.
* **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
* **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

📁 Source Data:
* Total files: 6 CSVs
* Types: CRM and ERP data
* Storage: Azure Data Lake (Landing zone)

## Project overview
This project involves:
* Data Architecture: Designing a Modern Data lakehouse Using Medallion Architecture Bronze, Silver, and Gold layers.
* ETL Pipelines: Extracting, transforming, and loading data from source systems into the lakehouse.
* Data Modeling: Developing fact and dimension tables optimized for analytical queries.

## 🚀 Project Requirements

### Building the ETL pipeline to process sales, customer and products data

#### Objective
Develop an ETL pipeline using Azure Lakehouse, Databricks to consolidate sales data, enabling analytical reporting and informed decision-making.

#### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

Resource: https://www.youtube.com/watch?v=9GVqKuTVANE
