# arXiv Metadata Analysis with PySpark and Hadoop

# Overview
This project analyzes a large dataset of metadata from arXiv using PySpark and Hadoop, all set up on an Ubuntu environment. The analysis leverages both RDD and DataFrame APIs to process and extract insights from the data, showcasing important transformations and optimization techniques for handling big data.

# Key Objectives
Data Exploration: Understand the structure and content of arXiv metadata, including fields like abstract, authors, and categories.

Data Processing: Apply PySpark transformations to perform tasks such as filtering, mapping, and aggregating data.

Optimization: Utilize techniques like caching, data persistence, and efficient transformations to optimize data processing.

# Project Components

# 1. RDD-Based Analysis
Data Loading: Read and parse JSON data into RDDs.
Key Transformations:
map: Transform data into key-value pairs.
filter: Select records based on specific criteria.
reduceByKey: Aggregate data by keys.
join: Combine datasets based on common keys.
Optimization Techniques:
Caching (cache): Store intermediate results in memory to speed up subsequent operations.
Persistence (persist): Persist RDDs in memory and disk to prevent recomputation.
Handling Data Skewness with Salting: Introduce a random "salt" to keys in data to distribute skewed data evenly across partitions, preventing certain partitions from becoming bottlenecks due to uneven data distribution.


# 2. DataFrame-Based Analysis
Data Loading: Load JSON data into a structured DataFrame.
Key Transformations:
SQL Queries: Use SQL for complex querying and aggregations.
User-Defined Functions (UDFs): Extend Spark's functionality with custom functions.
Optimization Techniques:
Lazy Evaluation: Spark optimizes the execution plan by delaying evaluation until an action is called.
Catalyst Optimizer: Optimizes the execution of DataFrame queries for performance improvements.
Salting for Skewness: Similar to the RDD approach, salting is used in SQL-based operations to balance the load across partitions, mitigating the impact of data skewness.


# Technologies Used
Apache Spark: Powerful engine for big data processing. <br/>
Hadoop: Storage layer for managing large datasets. <br/>
PySpark: Python interface for Apache Spark. <br/>
Jupyter Notebook: Interactive environment for analysis and visualization. <br/>

# Getting Started
Installation
Apache Spark & PySpark: Follow the official Spark documentation for installation.
Hadoop: Set up Hadoop on Ubuntu for data storage.
Python Packages: Install required packages using pip.

# Running the Analysis
Start Jupyter Notebook.
Open and run the notebooks to explore the analysis and results.

# Conclusion
This project demonstrates effective use of PySpark and Hadoop for big data analysis. By utilizing key transformations and optimization techniques, it highlights the capabilities of both RDD and DataFrame APIs in processing large datasets efficiently.

