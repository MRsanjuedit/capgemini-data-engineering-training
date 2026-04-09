# Phase 5 – Databricks + Olist (End-to-End Pipeline)

🔹 **Objective**
In this phase, the goal is to work with a real-world dataset using Databricks and PySpark.
This includes data ingestion, validation, building a fact table, applying advanced analytics using window functions, and generating a final reporting dataset.

---

🔹 **Problem Summary**
We were given the Olist e-commerce dataset consisting of multiple tables such as orders, customers, order_items, payments, and products.

The task was to:
• Upload and manage data in Databricks
• Combine multiple datasets
• Perform aggregations and analytics
• Apply window functions
• Generate business insights and final reports

---

🔹 **Approach**

1. Set up Databricks environment (cluster + notebook)
2. Uploaded all dataset files into the catalog named filestore and schema named olist.
3. Loaded CSV files into PySpark DataFrames
4. Validated data using schema checks and sample queries
5. Created a unified dataset (`fact_orders`) using joins
6. Performed transformations and aggregations
7. Applied window functions for advanced analysis
8. Built final reporting dataset

---

🔹 **Key Transformations Used**

• `join()` → to combine multiple tables
• `groupBy()` → for aggregations
• `agg()` → to calculate metrics (sum, count)
• `withColumn()` → to create new columns
• `when()` → for segmentation logic
• `window functions` → for ranking and running totals

---

🔹 **Analytical Tasks Performed**

• Top 3 customers per city using ranking
• Running total of daily sales
• Top products per category using DENSE_RANK
• Customer Lifetime Value calculation
• Customer segmentation (Gold, Silver, Bronze)
• Final reporting table creation

---

🔹 **Output / Results**

The following outputs were generated:
• Customer-level spend and segmentation
• Product-level sales insights
• Daily and cumulative sales trends
• Final combined reporting dataset

---

🔹 **Data Engineering Considerations**

• Ensured correct join conditions between tables
• Avoided duplicate records during joins
• Validated data using row counts and sample checks
• Used proper data types for accurate calculations

---

🔹 **Challenges Faced**

• Understanding relationships between multiple tables
• Handling missing columns like product category
• Managing file paths in Databricks
• Writing correct window functions

---

🔹 **Learnings**

• How to work with real-world datasets
• Importance of fact table (`fact_orders`)
• Use of window functions in analytics
• Building an end-to-end data pipeline
• Applying business logic through segmentation

---

🔹 **Pipeline Overview**

1. Data Ingestion → Load CSV files
2. Data Validation → Check schema and data quality
3. Data Transformation → Join tables and create fact table
4. Analytics → Apply aggregations and window functions
5. Reporting → Generate final dataset

