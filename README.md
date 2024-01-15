# Azure - Ecommerce Data Engineering Project

## Overview
The primary goal of this project is to ensure the secure management, optimization, and analysis of structured data from the E-Commerce API

## Steps Performed
The process goes as follows:

- Entered the E-Commerce API into the Azure Data Factory using Rest_Api service. Stored the Json data into ADLS Gen2 at bronze folder.
- Further, Used databricks which collects data from bronze folder and perform some transformations like droping a column, padding etc. Data gets stored into Silver folder with parquet delta fromat.
- Finaly stage of transformation, Silver folder's data gets tranforms based on business needs like renaming of column as we had small amount of data not major transform required. But we can perform like group, 
  calculations, enrichments, use-case specific optimizations etc.
- Once we get data into gold layer, Data gets consumed into azure synapse analysis for further analysis like Avg sales per category, Cateogry with highes and lowest profit and many more...
- Display data using PowerBI a visulation tool.
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
