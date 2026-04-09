Phase 1 – Databricks Interface & Basic Data Cleaning
---
🔹 Objective

In this phase, the goal is to understand the Databricks environment and perform basic data cleaning operations on a CSV dataset using PySpark.

This phase focuses on:

Learning the Databricks interface
Working with notebooks and clusters
Performing initial data cleaning tasks

🔹 Problem Summary

We were given a small CSV dataset containing inconsistent and dirty data.

The task was to:

Upload and read the dataset in Databricks
Explore the data
Clean the dataset by handling nulls, duplicates, and incorrect values

🔹 Approach

Navigated the Databricks workspace
Created and attached a cluster
Uploaded the CSV file to DBFS
Loaded the dataset using PySpark DataFrame
Explored the data using basic functions
Applied data cleaning techniques
Verified the cleaned output

🔹 Databricks Concepts Learned

Workspace → Organizing notebooks and files
Clusters → Compute environment to run code
Notebooks → Writing and executing PySpark code
DBFS (Databricks File System) → Storage for files
DataFrame Display → Viewing data interactively

🔹 Data Cleaning Techniques Used

dropna() → Removed rows with null values
fillna() → Replaced missing values
dropDuplicates() → Removed duplicate records
withColumn() → Modified or cleaned columns
cast() → Converted data types
filter() → Removed invalid data

🔹 Output / Results

Cleaned dataset with no null values
Removed duplicate records
Corrected data types
Improved data quality for further processing

🔹 Data Engineering Considerations

Ensured schema correctness using inferSchema
Handled missing values to avoid incorrect results
Verified cleaned data using .show() and .describe()
Maintained data consistency

🔹 Challenges Faced

Understanding Databricks interface initially
Handling null values properly
Fixing incorrect data types
Identifying duplicate records

🔹 Learnings

Basics of Databricks platform
How to work with PySpark DataFrames
Importance of data cleaning
Handling real-world dirty data
Understanding schema inference
