# **Phase 6: Analytical Transformations & Output Storage

---

## 🔹 Objective

In this phase, the objective is to perform analytical transformations on the cleaned dataset and store the final outputs for further usage.

This includes generating business insights such as top customers, repeat customers, and sales trends, along with saving results in optimized formats for reporting and downstream processing.

---

## 🔹 Problem Summary

After completing data cleaning, validation, and transformation, the next step was to:

* Perform advanced analysis on sales data
* Identify top-performing customers
* Detect repeat customers
* Analyze monthly revenue trends
* Store processed results efficiently for future use

---

## 🔹 Approach

The implementation followed a structured analytical pipeline:

1. Used cleaned and validated DataFrames from previous phases
2. Joined multiple datasets (customers, cars, sales)
3. Created derived columns such as revenue
4. Applied aggregations and window functions
5. Generated analytical insights
6. Saved outputs in optimized storage formats

---

## 🔹 Key Transformations Used

* **join()** → Combined multiple datasets to create a unified view
* **withColumn()** → Created derived columns (e.g., revenue calculation)
* **groupBy()** → Grouped data for aggregation
* **agg()** → Calculated metrics such as total revenue and counts
* **row_number() (Window Function)** → Ranked customers within partitions
* **filter()** → Extracted specific subsets of data
* **date_format()** → Enabled time-based analysis

---

## 🔹 Analysis Performed

### ✅ 1. Top 3 Customers per City

* Applied window function using ROW_NUMBER
* Partitioned data by city
* Ranked customers based on revenue
* Selected top 3 customers per city

---

### ✅ 2. Repeat Customers

* Grouped data by customer
* Counted number of purchases
* Filtered customers with more than one transaction

---

### ✅ 3. Monthly Sales Trend

* Extracted month from sale_date
* Aggregated total revenue per month
* Generated trend analysis for business insights

---

## 🔹 Output / Results

The following analytical outputs were generated:

* Top customers per city
* Repeat customer list
* Monthly revenue trends

**Storage Formats Used:**

* Parquet → Optimized for performance and large-scale processing
* CSV → Easy readability and sharing

---

## 🔹 Data Engineering Considerations

* Used window functions to retain row-level detail while ranking
* Ensured aggregations were performed only after proper data cleaning
* Chose Parquet format for efficient storage and faster queries
* Prevented duplicate records during joins
* Validated outputs using sample checks and intermediate results

---

## 🔹 Challenges Faced

* Correct implementation of window functions
* Managing joins across multiple datasets without data duplication
* Ensuring accurate revenue calculations
* Handling date formatting for time-based analysis

---

## 🔹 Learnings

* Performing analytical transformations using PySpark
* Practical usage of window functions in real-world scenarios
* Understanding differences between aggregation and window functions
* Generating meaningful business insights from processed data
* Best practices for storing and optimizing big data outputs

---

## 🔹 Topics Covered

* Data joins and transformations
* Aggregations and group-based analysis
* Window functions (ROW_NUMBER)
* Time-based analysis
* Data filtering
* Output storage (Parquet & CSV)
