# Azure - Ecommerce Data Engineering Project

## Overview
The primary goal of this project is to ensure the secure management, optimization, and analysis of structured data from the E-Commerce API

## Steps Performed
The process goes as follows:

- Integrated the E-Commerce API seamlessly into Azure Data Factory through the Rest_Api service. Stored the JSON data in the ADLS Gen2, organized within the bronze folder.
- Further, used databricks which collects data from bronze folder and perform some transformations like dropping a column, padding etc. Data gets stored into silver folder with parquet delta format.
- In the final transformation phase, data from silver folder is transformed to meet business needs. This includes minor changes like column renaming and essential operations such as grouping, calculations, enrichments, and use-case optimizations
- After data enters the gold layer, it's utilized in Azure Synapse Analytics for advanced analysis, including metrics like average sales per category, identifying categories with the highest and lowest profits 
  and many more…
- Data Visualization with PowerBI to present into comprehensible format 

- For more info on Bronze, silver & gold layer please do refer my post - https://www.linkedin.com/feed/update/urn:li:activity:7134486959044841472

## Services used:
1. Azure Data Factory for seamless workflow automation.
2. Azure Databricks for transformation.
3. Azure Data Lake Gen 2 for secure data management.
4. Azure Synapse Analytics for complex analytics.
5. Azure Storage Account for reliable storage.
6. Azure Key Vault & Azure Active Directory for security & governance.


## Dataset Used
This is an E-Commerce dummy API


## Project Goals
1. Data Ingestion — Build a mechanism to ingest data from API
2. ETL System — We are getting data in raw format, transforming this data into the proper format
3. Data lake — We will be getting data from API so we need location to store them
4. Scalability — As the size of our data increases, we need to make sure our system scales with it
5. Cloud — We can’t process API data so we need to use the cloud, in this case, we will use Azre
6. Reporting — Build a dashboard to get answers to the question we asked earlier.


## Architecture Diagram
<img src="architecture diagram.gif">
