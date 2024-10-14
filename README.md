# tokyo-olympic-azure-data-engineering-project
tokyo-olympic-azure-data-engineering-project

#The dataset has been taken from Kaggle.
https://www.kaggle.com/datasets/arjunprasadsarkhel/2021-olympics-in-tokyo


Project Architecture:
 
The Source of the Olympic data is Kaggle and stored into Github repositories and from github to Azure Data Lake Storage account Gen2.

Then the data will be moved to the object container (Data Lake) through Azure data factory with the help of copy activity. 

After data is being stored in Azure data factory, We transfer the data to the Azure Databricks through the connection.

Once data is modified in Azure Databricks, we store that data into Azure data Lake container with the help of pyspark code. 

After Transformation we take that data into Azure Synapse Analytics tool for data visualization and reporting through SQL commands, we perform transformation. 

We can transfer the data into Power BI or Tableau for the reporting. 

