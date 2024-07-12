# Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services
☁️🛠️ This project leverages Azure Data Factory, Azure Data Lake Storage Gen2, Azure Databricks, Azure Synapse Analytics, and Power BI to create a comprehensive data pipeline and analysis framework for the 2021 Tokyo Olympics dataset. The repository showcases the end-to-end workflow, from initial data setup to in-depth data analytics and visualization, including the creation of a dynamic dashboard. 🗂️🚀

## Architecture
![Architecture](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/architecture.jpg)

## Data Source
The dataset is sourced from Kaggle and contains detailed information about over 11,000 athletes, 47 disciplines, and 743 teams that participated in the 2021 (2020) Tokyo Olympics. It includes details about the athletes, coaches, teams, entries by gender, and medals won. The data is stored in GitHub’s CSV files accessible in this repository.

## Tools Used
- **GitHub:** For version control and managing data sources.
- **Azure Data Factory (ADF):** For orchestrating data ingestion and workflow automation.
- **Azure Data Lake Storage Gen 2 (ADLS Gen2):** For storing raw and processed data.
- **Azure Databricks:** For robust data transformation capabilities.
- **Azure Synapse Analytics:** For data warehousing and complex SQL queries for analysis.
- **Power BI :** For building dashboard and gaining actionable insights through data visualization.


## Project Workflow

### Data Ingestion
The data ingestion process starts with Azure Data Factory (ADF), which facilitates the smooth transfer of data from the CSV files stored in GitHub to the raw layer of Azure Data Lake Storage Gen 2 (ADLS Gen 2). ADF pipelines are configured to connect to the GitHub repository and copy the CSV files into ADLS. This initial step ensures that the raw data is securely and efficiently ingested into the Azure ecosystem, laying the groundwork for subsequent processing and analysis.

![1](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic1.jpg)

Once the data is ingested, it is stored in the raw layer of Azure Data Lake Storage Gen2. ADLS Gen2 provides a scalable and secure storage solution, which is essential for handling large datasets. Proper directory structures are established within ADLS to organize the raw and processed / transformed data layers, ensuring that the data is well-managed and easily accessible for further processing.

![2](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic2.jpg)
![3](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic3.jpg)

### Data Transformation
Azure Databricks is used for the data transformation phase. A Databricks cluster is set up, and notebooks are developed to clean, transform, and enrich the raw data stored in ADLS Gen2. Various data processing operations are performed, including data cleaning, normalization, and enrichment. The transformed data is then stored back in ADLS Gen2, but this time in the processed layer, making it ready for advanced analytics.

![6](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic6.jpg)
![4](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic4.jpg)
![5](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic5.jpg)

### Analytics
With the data transformed and enriched, Azure Synapse Analytics is employed for robust data warehousing and detailed analysis. The processed data from ADLS Gen2 is loaded into Azure Synapse, where complex queries and analytical operations are conducted. This stage involves the creation of data models, running advanced queries, and performing in-depth analyses to extract meaningful insights from the dataset. Azure Synapse provides the computational power and flexibility needed to handle large-scale data analysis tasks.

![7](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic7.jpg)
![9](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic9.jpg)

### Dashboard
The final phase of the project involves visualizing the insights obtained from Azure Synapse Analytics using Power BI. Power BI is connected to Azure Synapse to create interactive and informative dashboards. These dashboards provide a comprehensive view of the Tokyo Olympic data, allowing to explore the dataset visually and gain valuable insights. 

![10](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic10.jpg)

![11](https://github.com/snowieeeee/Data-Pipeline-and-Analysis-Tokyo-Olympics-with-Azure-Services/blob/main/screens/pic11.jpg)

