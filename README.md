# APACHE SPARK: Data Analysis, Transformation, and Visualisation with PySpark
# IPL Data Analysis with Apache Spark and PySpark on Databricks

## Introduction

Welcome to the IPL Data Analysis project using Apache Spark and PySpark on Databricks! This project aims to demonstrate the power of big data processing and analytics using Spark, specifically focusing on IPL (Indian Premier League) cricket data. We will leverage the Databricks Community Edition for our computations and showcase how to analyze large datasets efficiently.

This README file will guide you through the entire process, from setting up your Databricks environment to running the analysis on IPL data. Whether you are a beginner or an experienced data analyst, this step-by-step guide will help you get started with Apache Spark and PySpark.

## What is Apache Spark and PySpark?

Apache Spark is an open-source, distributed computing system that provides an interface for programming entire clusters with implicit data parallelism and fault tolerance. PySpark is the Python API for Spark, which allows you to write Spark applications using Python.

### Differences between Apache Spark, PySpark, and Pandas

- **Apache Spark**: A fast, distributed processing engine suitable for large-scale data processing tasks.
- **PySpark**: The Python interface to Apache Spark, enabling Python developers to leverage Spark's power.
- **Pandas**: A Python library for data manipulation and analysis, ideal for small to medium-sized datasets. Unlike Spark, Pandas operates on a single machine.

## Packages Used in This Project

- **pyspark**: The Python API for Spark, enabling us to use Spark functionalities in Python.
- **pandas**: A data manipulation library used for smaller data processing tasks.
- **matplotlib**: A plotting library used for data visualization.
- **seaborn**: A statistical data visualization library built on top of Matplotlib.
- **databricks-cli**: A command-line interface for interacting with Databricks.
- **boto3**: The Amazon Web Services (AWS) SDK for Python, used to interact with S3.

## Project Setup

### Step 1: Create a Databricks Community Edition Account

1. Visit the [Databricks Community Edition](https://community.cloud.databricks.com/login.html) website.
2. Click on "Get Started for Free".
3. Fill in your details to create an account.
4. Verify your email address and log in to Databricks.

### Step 2: Create a New Cluster

1. After logging in, click on "Clusters" in the left-hand menu.
2. Click "Create Cluster".
3. Name your cluster (e.g., "IPL-Analysis-Cluster").
4. Select the appropriate Databricks runtime version.
5. Click "Create Cluster".

### Step 3: Upload Data to Databricks

You can either upload the data files directly to Databricks or use S3 for storage.

#### Option A: Upload Data Directly to Databricks

1. Click on "Data" in the left-hand menu.
2. Click "Add Data" and select "Upload File".
3. Upload the IPL data CSV files.

#### Option B: Use Amazon S3

1. If you have your data stored in S3, you can access it directly from Databricks.
2. Ensure you have the necessary AWS credentials configured.
3. Use the following code snippet to read data from S3:
   ```python
   df = spark.read.csv("s3a://your-bucket-name/your-file.csv", header=True, inferSchema=True)
   ```

### Step 4: Clone the Project Repository

1. In your Databricks workspace, click on "Repos" in the left-hand menu.
2. Click "Add Repo" and select "Clone Existing Repo".
3. Enter the URL of the repository: `https://github.com/TravelXML/APACHE-SPARK-PYSPARK-DATABRICKS.git`
4. Click "Create Repo".

### Step 5: Open the Notebook

1. Navigate to the cloned repository in the "Repos" section.
2. Open the notebook file `IPL_DATA_ANALYSIS_SPARK_SAP.ipynb`.

## Running the Analysis

1. Attach your notebook to the cluster you created earlier.
2. Follow the steps in the notebook to perform data analysis.
3. The notebook contains code cells with detailed explanations of each step, including data loading, cleaning, transformation, and visualization.

## Summary of Analysis

This project provides a comprehensive analysis of IPL data, covering various aspects such as:

- Data ingestion and schema inference using PySpark.
- Data cleaning and preprocessing.
- Exploratory data analysis (EDA) using PySpark and Pandas.
- Visualization of key insights using Matplotlib and Seaborn.

## Conclusion

By following this guide, you should be able to set up a Databricks environment, upload data, and run a complete data analysis project using Apache Spark and PySpark. This project serves as a practical introduction to big data analytics with Spark, demonstrating its capabilities and how it can be used for real-world data analysis tasks.

We hope this project helps you get started with Spark and PySpark and inspires you to explore further possibilities in big data analytics.

## Additional Resources

- [Databricks Documentation](https://docs.databricks.com/)
- [Apache Spark Documentation](https://spark.apache.org/documentation.html)
- [PySpark Documentation](https://spark.apache.org/docs/latest/api/python/)

Feel free to reach out if you have any questions or need further assistance. Happy coding!
