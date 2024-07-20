# Spotify Songs ETL and Visualization Project

## Project Overview
This project invloves extracting, transforming and loading (ETL) data from the CSV file "Most Streamed Songs on Spotify" using Microsoft Azure services. The data is sourced from Kaggle and is used under the following license: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). The final output is visualized using PowerBI.

 ## Architecture and Tools
 - **Data Source :** Kaggle Dataset
 - **Storage :** Azure Data Lake Gen2 Storage Account
 - **ETL Processing :** Azure Synapse Studio
 - **NoteBook Development :** Azure Synapse Workspace with Spark Pool
 - **Pipeline Monitoring :** Azure Monitor
 - **Visualization :** PowerBI

## Steps Involved
### 1. Data Storage
The dataset from Kaggle was stored in an Azure Data Lake Gen2 Storage Account to facilitate efficient and scalable data access.
### 2. ETL Process
- **Azure Synapse Workspace:** Created a Synapse workspace to manage and organize the ETL process.
- **Spark Pool:** Set up a Spark pool within the Synapse workspace to handle data processing.
- **Notebook Development:** Developed a notebook in Synapse studio, attached it to the spark pool, and wrote Pyspark queries to:
- - Transform the data
  - Filter the data
  - Aggregate the data
- **ETL Pipeline:** Built an ETL pipeline within Synapse Studio that:
- - Executes the Spark notebook
  - Writes the processed data back into Azure Data Lake Gen2 Storage Account
- **Pipeline Monitoring:** Used Azure Monitor to run and monitor the ETL pipeline.

## Data Visualization
The final output was visualized using PowerBI to derive insights and present the findings in an intuitive manner.

## How to run the project
1. **Set up Azure Data Lake Storage Account:** Set up an Azure Data Lake Storage Account and then create a container and store the dataset inside the storage account.
2. **Create Azure Synapse Workspace:** Set up a Synapse workspace and create a Spark pool.
3. **Develop and Run notebook:** Create a notebook in Synapse studio, attach the Spark pool and write Pyspark queries for data transformation, filtering and aggregation.
4. **Build ETL Pipeline :** Create a pipeline in Synapse studio to run the notebook and upon success of that activity save the output of processed data into the Azure Data Lake Storage Account.
5. **Visualize Data with PowerBI:** Connect to PowerBI to the processed data in Azure Data Lake Storage and create visua;izations to present the findings.

## License
The dataset used in this project is available under the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license.

## Conclusion
This project demonstrates the use of Microsoft Azure services to perform ETL processes and visualize data. By leveraging Azure Synapse Studio, Spark and PowerBI, we can efficiently process and analyze large datasets to extract meaningful insights.

