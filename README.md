# End-to-end Azure Data Engineering project using ADLS Gen2, ADF, Databricks and Synapse.


#  Azure Data Engineering Project – Tokyo Olympics Analytics

This is an end-to-end **Azure data engineering pipeline** I built as a student to learn real-world cloud data engineering.

##  Tech Stack

- Azure Data Lake Storage Gen2 (ADLS) – raw, silver, gold layers  
- Azure Data Factory – ingestion from source to ADLS  
- Azure Databricks (PySpark) – transformations  
- Azure Synapse Analytics – querying the gold layer  

##  Architecture (High Level)

1. Ingest raw Tokyo Olympics CSV data into **ADLS Gen2 (raw container)** using **Azure Data Factory**  
2. Use **Databricks (PySpark)** to clean and transform data → write to **silver**  
3. Aggregate medal counts by country and create a **gold** dataset in ADLS  
4. Query the gold data using **Azure Synapse serverless SQL**

##  What I learned

- How to connect ADF → ADLS Gen2 → Databricks → Synapse  
- How to design raw/silver/gold (medallion) layers  
- How to write basic PySpark transformations  
- How to build analytics-ready tables for reporting
