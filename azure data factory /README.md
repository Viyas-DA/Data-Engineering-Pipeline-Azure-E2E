# Azure Data Factory - (adf-etl-demo-01)

Azure Data Factory was the tool used to engineer most of the extract/transform/load (ETL) pipeline.

**Extract:**

* Connected to the local SQL server database using the Key Vault secrets assigned for the username and password.
* Queried for all of the tables in the on-prem database.
* Copied the tables into the Bronze container in the data lake to undergo transformations.

**Transform:**

* Queued the Databricks notebooks to run and process the Bronze layer data
* Initially cleansed data from the Bronze layer and loaded to the Silver layer for further transformation.
* Further refined data from the Silver layer and loaded to Gold layer to be used for reporting and analytics.

**Load:**

* The load piece was completed by Azure Synapse Analytics
* The Gold layer data was loaded into a serverless SQL database.
* Additionally, a trigger was created to run this pipeline daily--completely automating the refinement of new row/column data.

  ![image](https://github.com/user-attachments/assets/d68f5712-d3f5-44c9-9607-d55ca6838034)


