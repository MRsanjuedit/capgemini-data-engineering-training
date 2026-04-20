# Week 2 Day 3 – Medallion Architecture Pipeline

## Objective

Build an end-to-end data pipeline using **Medallion Architecture (Bronze, Silver, Gold)** to transform raw data into clean, analytics-ready datasets.

---

## Tasks Completed

### 1. Flipkart Data Pipeline

* Implemented Bronze, Silver, and Gold layers
* Processed transactional dataset with real-world data issues
* Generated business-ready insights for analysis

### 2. Synthetic Data Generation

* Generated 20,000+ records using PySpark
* Introduced realistic data challenges:

  * NULL values
  * Duplicate records
  * Negative values
  * Incremental updates
* Stored data as CSV for pipeline ingestion

---

## Medallion Architecture

### Bronze Layer (Raw)

* Ingested raw CSV data
* Stored data in Delta format
* Followed append-only strategy (no transformations)

---

### Silver Layer (Cleaned)

* Handled NULL values (`amount`, `city`)
* Converted data types (amount → integer, date → date)
* Removed duplicate records (based on `order_id`)
* Retained latest records (handled incremental updates)
* Filtered out negative values

---

### Gold Layer (Business)

**Aggregations:**

* Sales by product, category, and city

**Customer Metrics:**

* Total number of orders
* Total customer spending

**Insights Generated:**

* Top-performing products
* High-value customers

---

## Data Issues Handled

* NULL values
* Duplicate records
* Negative amounts
* Incremental data updates

---

## Key Learnings

* Importance of layered data architecture
* Practical data cleaning and validation techniques
* Handling real-world data inconsistencies
* Designing scalable and maintainable pipelines

---

## Tools Used

* **PySpark**
* **Delta Lake**
* **Python**

---

## Outcome

* Built a structured pipeline from raw → cleaned → analytics-ready data
* Produced datasets ready for dashboards and reporting

---
