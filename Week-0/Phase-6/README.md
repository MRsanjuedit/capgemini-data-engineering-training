# **Phase 6 – Spark Playground Exit Sprint (Advanced Practice Lab)**

## **🔹 Objective**

Strengthen proficiency in **PySpark** by solving advanced data engineering problems involving joins, window functions, data cleaning, and end-to-end pipeline execution on real-world, imperfect datasets.

---

## **🔹 Problem Statement**

The datasets (`customers` and `orders`) contained multiple data quality issues:

* Null values in critical fields
* Invalid records (e.g., negative transaction amounts, incorrect foreign keys)
* Duplicate entries

### **Key Requirements**

* Clean and validate raw datasets
* Ensure referential integrity between tables
* Perform joins and aggregations
* Apply window functions for analytical insights
* Build a complete, production-style data pipeline

---

## **🔹 Architecture / Approach**

1. **Data Ingestion**

   * Loaded raw datasets into PySpark DataFrames

2. **Data Cleaning**

   * Removed null values in critical columns using `dropna()`
   * Filtered invalid records (e.g., negative amounts)
   * Trimmed string columns for consistency
   * Eliminated duplicate records using `dropDuplicates()`

3. **Data Validation**

   * Verified referential integrity between datasets
   * Used **`left_anti` join** to identify invalid foreign keys

4. **Data Integration**

   * Applied appropriate join strategies:

     * `inner join` → for valid records
     * `left join` → for validation and completeness checks

5. **Transformation Layer**

   * Aggregated customer-level metrics:

     * Total spend
     * Order count
   * Applied filtering to maintain clean datasets

6. **Analytics Layer**

   * Implemented window functions:

     * Customer ranking based on total spend
     * Running totals
     * Lag-based comparisons

7. **Time-Based Analysis**

   * Extracted temporal features using `to_date()` and `month()`
   * Performed monthly sales aggregation

8. **Output Generation**

   * Generated and stored final curated datasets

---

## **🔹 Key Transformations**

| Transformation         | Purpose                                    |
| ---------------------- | ------------------------------------------ |
| `join()`               | Combine customers and orders               |
| `left_anti join`       | Detect invalid foreign key relationships   |
| `groupBy()`            | Perform aggregations                       |
| `agg()`                | Compute metrics (SUM, COUNT)               |
| `filter()`             | Remove invalid records                     |
| `dropna()`             | Handle missing values                      |
| `dropDuplicates()`     | Remove duplicate records                   |
| Window Functions       | Ranking, running totals, lag analysis      |
| `to_date()`, `month()` | Date transformation and feature extraction |

---

## **🔹 Analytical Use Cases**

* **Data Quality Validation**

  * Identified invalid foreign key relationships using `left_anti` join

* **Customer-Level Metrics**

  * Total spend per customer
  * Order count per customer

* **Customer Ranking**

  * Ranked customers based on total spending using window functions

* **Time-Series Analysis**

  * Monthly sales aggregation
  * Trend analysis over time

---

## **🔹 Outputs / Deliverables**

* Cleaned and standardized datasets (`customers`, `orders`)
* Invalid records report (foreign key mismatches)
* Aggregated customer-level metrics
* Ranked customer dataset
* Monthly sales summary dataset

---

## **🔹 Data Engineering Best Practices Applied**

* Performed **data cleaning prior to transformations**
* Ensured **referential integrity validation** using joins
* Prevented **duplicate records post-join operations**
* Handled **null and invalid values systematically**
* Validated outputs using **row counts and sampling techniques**

---

## **🔹 Challenges & Resolutions**

| Challenge                                   | Resolution                                   |
| ------------------------------------------- | -------------------------------------------- |
| Identifying invalid foreign keys            | Used `left_anti` joins for precise detection |
| Handling dirty data (nulls, invalid values) | Applied systematic cleaning and filtering    |
| Understanding window functions              | Practiced with incremental datasets          |
| Managing complex transformations            | Structured pipeline into modular steps       |

---

## **🔹 Key Learnings**

* Mastery of **advanced join techniques** (`inner`, `left`, `left_anti`)
* Importance of **data validation in ETL pipelines**
* Practical application of **window functions for analytics**
* Handling **real-world dirty datasets effectively**
* Designing **end-to-end PySpark data pipelines**

---

## **🔹 Pipeline Flow**

```id="k8dm21"
Data Ingestion → Data Cleaning → Data Validation → Data Transformation → Analytics → Reporting
```

---

## **🔹 Tech Stack**

* **Platform:** Apache Spark / Databricks
* **Language:** PySpark
* **Data Format:** CSV
* **Concepts:** ETL, Data Cleaning, Data Validation, Window Functions, Aggregations
