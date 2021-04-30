# DP-203T00: Data Engineering on Azure

Welcome to the course DP-203: Data Engineering on Azure. To support this course, we will need to make updates to the course content to keep it current with the Azure services used in the course.  We are publishing the lab instructions and lab files on GitHub to allow for open contributions between the course authors and MCTs to keep the content current with changes in the Azure platform.

- **Are you a MCT?** - Have a look at our [GitHub User Guide for MCTs](https://microsoftlearning.github.io/MCT-User-Guide/).
                                                                       
## How should I use these files relative to the released MOC files?

- The instructor handbook and PowerPoints are still going to be your primary source for teaching the course content.

- These files on GitHub are designed to be used in conjunction with the student handbook, but are in GitHub as a central repository so MCTs and course authors can have a shared source for the latest lab files.

- the lab instructions for each module are found in the /Instructions/Labs folder. Each subfolder within this location refers to each module. For example, Lab01 relates to module01 etc. A README.md file exists in each folder with the lab instructions that the students will then follow.

- It will be recommended that for every delivery, trainers check GitHub for any changes that may have been made to support the latest Azure services, and get the latest files for their delivery.

- Please note that some of the images that you see in these lab instructions will not neccessarily reflect the state of the lab environment that you will be using in this course. For example, while browsing for files in a data lake, you may see adiitional folders in the images that may not exist in your environment. This is by design, and your lab instructions will still work.

## What about changes to the student handbook?

- We will review the student handbook on a quarterly basis and update through the normal MOC release channels as needed.

## How do I contribute?

- Any MCT can submit a issues to the code or content in the GitHub repro, Microsoft and the course author will triage and include content and lab code changes as needed.
## Classroom Materials

It is strongly recommended that MCTs and Partners access these materials and in turn, provide them separately to students.  Pointing students directly to GitHub to access Lab steps as part of an ongoing class will require them to access yet another UI as part of the course, contributing to a confusing experience for the student. An explanation to the student regarding why they are receiving separate Lab instructions can highlight the nature of an always-changing cloud-based interface and platform. Microsoft Learning support for accessing files on GitHub and support for navigation of the GitHub site is limited to MCTs teaching this course only.

## Lab overview

The following is a summary of the lab objectives for each module:

### Lab 1 - Explore compute and storage options for data engineering workloads

This lab teaches ways to structure the data lake, and to optimize the files for exploration, streaming, and batch workloads. The student will learn how to organize the data lake into levels of data refinement as they transform files through batch and stream processing. The students will also experience working with Apache Spark in Azure Synapse Analytics.  They will learn how to create indexes on their datasets, such as CSV, JSON, and Parquet files, and use them for potential query and workload acceleration using Spark libraries including Hyperspace and MSSParkUtils.

### Lab 2 - Design and implement the serving layer

This lab teaches how to design and implement data stores in a modern data warehouse to optimize analytical workloads. The student will learn how to design a multidimensional schema to store fact and dimension data. Then the student will learn how to populate slowly changing dimensions through incremental data loading from Azure Data Factory.

### Lab 3 - Data engineering considerations for source files

In this lab, you will be directed by your instructor to work alone, or in groups for 20 minutes to read through the following information presented below. You will then answer the questions and present back to the classroom your findings based on the requirements.

### Lab 4 - Run interactive queries using Azure Synapse Analytics serverless SQL pools

In this lab, students will learn how to work with files stored in the data lake and external file sources, through T-SQL statements executed by a serverless SQL pool in Azure Synapse Analytics. Students will query Parquet files stored in a data lake, as well as CSV files stored in an external data store. Next, they will create Azure Active Directory security groups and enforce access to files in the data lake through Role-Based Access Control (RBAC) and Access Control Lists (ACLs).

### Lab 5 - Explore, transform, and load data into the Data Warehouse using Apache Spark

This lab teaches you how to explore data stored in a data lake, transform the data, and load data into a relational data store. You will explore Parquet and JSON files and use techniques to query and transform JSON files with hierarchical structures. Then you will use Apache Spark to load data into the data warehouse and join Parquet data in the data lake with data in the dedicated SQL pool.

### Lab 6 - Data Exploration and Transformation in Azure Databricks

This lab teaches you how to use various Apache Spark DataFrame methods to explore and transform data in Azure Databricks. You will learn how to perform standard DataFrame methods to explore and transform data. You will also learn how to perform more advanced tasks, such as removing duplicate data, manipulate date/time values, rename columns, and aggregate data. They will provision the chosen ingestion technology and integrate this with Stream Analytics to create a solution that works with streaming data.

### Lab 7 - Ingest and load data into the data warehouse

This lab teaches students how to ingest data into the data warehouse through T-SQL scripts and Synapse Analytics integration pipelines. The student will learn how to load data into Synapse dedicated SQL pools with PolyBase and COPY using T-SQL. The student will also learn how to use workload management along with a Copy activity in a Azure Synapse pipeline for petabyte-scale data ingestion.

### Lab 8 - Transform data with Azure Data Factory or Azure Synapse Pipelines

This lab teaches students how to build data integration pipelines to ingest from multiple data sources, transform data using mapping data flows and notebooks, and perform data movement into one or more data sinks.

### Lab 9 - Integrate data from Notebooks with Azure Data Factory or Azure Synapse Pipelines

In the lab, the students will create a notebook to query user activity and purchases that they have made in the past 12 months. They will then add the notebook to a pipeline using the new Notebook activity and execute this notebook after the Mapping Data Flow as part of their orchestration process. While configuring this the students will implement parameters to add dynamic content in the control flow and validate how the parameters can be used.

### Lab 10 - Optimize query performance with dedicated SQL pools in Azure Synapse

In this lab, students will learn strategies to optimize data storage and processing when using dedicated SQL pools in Azure Synapse Analytics. The student will know how to use developer features, such as windowing and HyperLogLog functions, use data loading best practices, and optimize and improve query performance.

### Lab 11 - Analyze and Optimize Data Warehouse Storage

This lab teaches you how to analyze and optimize the data storage of the Azure Synapse dedicated SQL pools. You will know techniques to understand table space usage and column store storage details. Next, you will know how to compare storage requirements between identical tables that use different data types. Finally, you will observe the impact materialized views have when executed in place of complex queries and learn how to avoid extensive logging by optimizing delete operations.

### Lab 12 - Support Hybrid Transactional Analytical Processing (HTAP) with Azure Synapse Link

This lab teaches you how Azure Synapse Link enables seamless connectivity of an Azure Cosmos DB account to a Synapse workspace. You will understand how to enable and configure Synapse link, then how to query the Azure Cosmos DB analytical store using Apache Spark and SQL Serverless.

### Lab 13 - End-to-end security with Azure Synapse Analytics

In this lab, students will learn how to secure a Synapse Analytics workspace and its supporting infrastructure. The student will observe the SQL Active Directory Admin, manage IP firewall rules, manage secrets with Azure Key Vault and access those secrets through a Key Vault linked service and pipeline activities. The student will understand how to implement column-level security, row-level security, and dynamic data masking when using dedicated SQL pools.

### Lab 14 - Real-time Stream Processing with Stream Analytics

This lab teaches you how to process streaming data with Azure Stream Analytics. You will ingest vehicle telemetry data into Event Hubs, then process that data in real time, using various windowing functions in Azure Stream Analytics. You will output the data to Azure Synapse Analytics. Finally, you will learn how to scale the Stream Analytics job to increase throughput.

### Lab 15 - Create a Stream Processing Solution with Event Hubs and Azure Databricks

This lab teaches you how to ingest and process streaming data at scale with Event Hubs and Spark Structured Streaming in Azure Databricks. You will learn the key features and uses of Structured Streaming. You will implement sliding windows to aggregate over chunks of data and apply watermarking to remove stale data. Finally, you will connect to Event Hubs to read and write streams.

### Lab 16 - Build reports using Power BI integration with Azure Synapse Analytics

In this lab, the student will learn how to integrate Power BI with their Azure Synapse workspace to build reports in Power BI. The student will create a new data source and Power BI report in Azure Synapse Studio. Then the student will learn how to improve query performance with materialized views and result-set caching. Finally, the student will explore the data lake with serverless SQL pools and create visualizations against that data in Power BI.

### Lab 17 - Perform Integrated Machine Learning Processes in Azure Synapse Analytics

In the lab, the students will explore the integrated, end-to-end Azure Machine Learning and Azure Cognitive Services experience in Azure Synapse Analytics. You will learn how to connect an Azure Synapse Analytics workspace to an Azure Machine Learning workspace using a Linked Service and then trigger an Automated ML experiment that uses data from a Spark table. You will also learn how to use trained models from Azure Machine Learning or Azure Cognitive Services to enrich data in a SQL pool table and then serve prediction results using Power BI.
