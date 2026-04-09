# **Phase 5 – Databricks + Olist (End-to-End Data Pipeline)**

## **🔹 Objective**

Design and implement an end-to-end data pipeline using **Databricks and PySpark** on a real-world e-commerce dataset (Olist).
The pipeline covers data ingestion, validation, transformation, advanced analytics, and reporting.

---

## **🔹 Problem Statement**

The Olist dataset consists of multiple relational tables, including:

* `orders`
* `customers`
* `order_items`
* `payments`
* `products`

### **Key Requirements**

* Ingest and manage raw data in Databricks
* Integrate multiple datasets into a unified model
* Perform aggregations and analytical transformations
* Apply window functions for advanced insights
* Generate business-ready reporting datasets

---

## **🔹 Architecture / Approach**

1. **Environment Setup**

   * Configured Databricks cluster
   * Created notebooks for modular pipeline execution

2. **Data Ingestion**

   * Uploaded CSV datasets to `FileStore`
   * Organized under schema: `olist`
   * Loaded data into PySpark DataFrames

3. **Data Validation**

   * Schema validation
   * Null checks and data consistency verification
   * Sample data inspection

4. **Data Modeling**

   * Designed and built a centralized **fact table (`fact_orders`)**
   * Integrated multiple dimension tables via joins

5. **Transformation Layer**

   * Applied business logic and feature engineering
   * Performed aggregations and derived metrics

6. **Analytics Layer**

   * Implemented window functions for advanced insights
   * Generated customer and product-level analytics

7. **Reporting Layer**

   * Created final curated datasets for reporting and visualization

---

## **🔹 Key Transformations**

| Transformation   | Purpose                               |
| ---------------- | ------------------------------------- |
| `join()`         | Combine multiple datasets             |
| `groupBy()`      | Aggregate data                        |
| `agg()`          | Compute metrics (SUM, COUNT, etc.)    |
| `withColumn()`   | Create derived columns                |
| `when()`         | Apply conditional logic               |
| Window Functions | Ranking, running totals, segmentation |

---

## **🔹 Analytical Use Cases**

* **Top Customers per City**

  * Identified using ranking functions

* **Daily & Cumulative Sales**

  * Running totals using window functions

* **Top Products by Category**

  * Applied `DENSE_RANK()` for ranking

* **Customer Lifetime Value (CLV)**

  * Total spend per customer

* **Customer Segmentation**

  * Categorized into:

    * Gold
    * Silver
    * Bronze

* **Final Reporting Dataset**

  * Consolidated business insights into a single dataset

---

## **🔹 Outputs / Deliverables**

* Customer-level spend and segmentation dataset
* Product-level sales performance insights
* Daily and cumulative sales trends
* Final aggregated reporting table

---

## **🔹 Data Engineering Best Practices Applied**

* Ensured **accurate join conditions** across tables
* Prevented **duplicate records** during joins
* Performed **data validation checks** (row counts, sampling)
* Used appropriate **data types for calculations**
* Maintained **modular and scalable pipeline design**

---

## **🔹 Challenges & Resolutions**

| Challenge                                   | Resolution                                    |
| ------------------------------------------- | --------------------------------------------- |
| Complex table relationships                 | Analyzed schema and defined correct join keys |
| Missing attributes (e.g., product category) | Applied fallback logic / handled nulls        |
| File path handling in Databricks            | Standardized FileStore paths                  |
| Writing window functions                    | Iterative testing with small datasets         |

---

## **🔹 Key Learnings**

* Hands-on experience with **real-world data pipelines**
* Importance of **fact table design** in analytics
* Practical usage of **window functions**
* End-to-end workflow in **Databricks + PySpark**
* Translating **business requirements into data transformations**

---

## **🔹 Pipeline Flow**

```
Data Ingestion → Data Validation → Data Transformation → Analytics → Reporting
```

---
