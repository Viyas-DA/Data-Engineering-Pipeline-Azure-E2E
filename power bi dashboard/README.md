# Power BI - (pbi-e2e-de)

This results from the ETL pipeline and offers an interactive reporting and analytics experience.

Power BI Desktop loads the data from the "gold_db" table created in Azure Synapse Analytics.

Why use the Azure Synapse database as the source VS the Gold container in the Data Lake?

* It's an established best practice to use a database as the serving layer for Power BI reporting.
* The Synapse database offers greater scalability and easier maintenance than reporting from the Data Lake.
  
The Desktop version is included in this folder to download and experiment with the visualizations. The dashboard is also published to the Power BI Service (and Microsoft Fabric) but cannot be accessed by users outside my organization.

![image](https://github.com/user-attachments/assets/cb7417fe-7ba9-46d5-8304-50a962eccc88)
