# Analysis of Patents in Virus Engineering


## Overview

This project explores the patent landscape in virus engineering using big data techniques. By examining patent trends, technological advances, key inventors, and geographic distributions, we aim to understand the field's current state and future potential in gene therapy, oncolytic virotherapy, and vaccine development.

## Objectives

Our key objectives include:
- **Identifying Trends:** Uncover emerging technologies and innovation trends.
- **Analyzing Advances:** Understand significant technological breakthroughs.
- **Spotting Key Players:** Identify leading countries, organizations, and inventors.
- **Evaluating Distribution:** Assess geographic trends and collaborations.
- **Mapping the Landscape:** Provide a detailed overview of technological advancements.
- **Gaining Insights:** Offer insights into competitive dynamics and market trends.


 ## Project Rchetecture
 
 ![ProjectArchitecture](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/c78197cc-9a14-4454-92ee-44564259b74d)

  
## Data Collection

![image](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/3f6c3edf-4a98-4c45-ba53-af5ed7264c39)

Patent data was collected from several sources, including:
- **Google Patents:** Comprehensive data on patent details and publication.
- **Espacenet:** Focuses on publication timelines and priority dates.
- **Free Patents Online (FPO):** Provides concise patent identification data.
- **USPTO:** Detailed data including classification, relevancy, and family ID.
- **WIPO:** Covers essential patent details for broad understanding.

## Data Storage and Preparation

![image](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/f951a94e-e5c5-466d-8dae-c714c9e598fe)

We used Amazon S3 for initial data storage due to its scalability and durability. Data cleaning and preprocessing were done using Apache Spark and Pandas. The cleaned data was then transferred to Azure Blob Storage for further processing.

## ETL Process and Architecture

![image](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/4fe06623-4c8e-4d15-952b-ed5997ddf9d0)

We implemented an ETL (Extract, Transform, Load) process using Azure Databricks, following the Medallion architecture:
- **Extraction:** Data sourced from AWS was transferred to Azure.
- **Transformation:** Data was cleaned, normalized, and enriched through bronze, silver, and gold stages.
- **Loading:** Transformed data was loaded into Azure SQL Database.

## Data Analysis and Visualization

![image](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/a7095296-6d55-4d4a-9785-9938d7f54b7a)
![image](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/eda84c07-efa1-4489-ad55-380b12c4c168)
![image](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/3cfdc008-f86c-4e0b-8be9-c5229d133097)

Using Power BI, we visualized the patent data to identify trends and insights:
- **Count of Patents by Year:** A pie chart showing patents distribution by year.
- **Count of Inventors by Country:** A bar chart depicting the distribution of inventors across countries.
- **Number of patents by country and Year**
- ...
- 

## Website Functionality

![image](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/eaa1587f-75d7-410b-99b0-677d92cf9046)
![image](https://github.com/BoukayouaLoubna/PatentAnalysis/assets/161256795/f4104ea9-3d47-4b2b-b050-92ce2e46e206)

We developed a website to facilitate patent searches and analysis. Key features include:
- **Patent Search:** Allows users to search patents by keywords.
- **Search Results:** Displays results in a tabular format.
- **User Interaction:** Provides user registration and login functionalities.


## Conclusion
Our analysis provides a comprehensive understanding of the virus engineering patent landscape. By leveraging big data, we have identified key trends and advancements, offering valuable insights for future research and development in this rapidly evolving field.
