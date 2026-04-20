# Insurance Data Analysis using PySpark & SQL

## Project Overview

This project focuses on analyzing insurance data using **PySpark** and **SQL** to identify customer risk, ensure data quality, and generate meaningful business insights.

### Dataset Includes

* Customers
* Policies
* Claims
* Agents
* Policy-Agent Mapping

---

## Objectives

* Perform data understanding and cleaning
* Build relationships between datasets
* Compute key business metrics
* Identify high-risk customers
* Apply advanced SQL concepts (Subqueries, CTEs, Window Functions)

---

## Phase-wise Implementation

### Phase 1 – Data Understanding

In this phase, the datasets were explored to understand structure and relationships.

**Key checks performed:**

* Identifying null values
* Detecting negative or invalid values
* Validating schema and column data types
* Understanding dataset relationships

**Relationship flow:**
Customer → Policy → Claim → Agent

---

### Phase 2 – Data Cleaning

Focused on improving overall data quality.

**Actions performed:**

* Handled missing values
* Removed invalid records (e.g., negative premium or claim amounts)
* Standardized text columns for consistency
* Corrected data types
* Enforced referential integrity across tables

---

### Phase 3 – Transformations

Converted raw data into business-level metrics.

**Key transformations:**

* Total premium per customer
* Total claims per customer
* Risk score (claim-to-premium ratio)

These transformations enabled meaningful analysis and decision-making.

---

### Phase 4 – SQL Analysis (Subqueries)

Performed analytical queries to extract business insights.

**Use cases:**

* Identifying top customers
* Detecting repeat customers
* Analyzing trends over time

#### Subqueries – Concept

Subqueries are nested queries used within another query.

**Used for:**

* Dynamic filtering based on aggregated values
* Performing dependent calculations
* Preparing intermediate datasets

**Types used:**

* Scalar subqueries
* Subqueries in WHERE conditions
* Aggregation-based subqueries

Subqueries improved flexibility in solving complex analytical problems.

---

### Phase 5 – Advanced SQL (CTE)

Introduced structured query design using CTEs.

#### CTE (Common Table Expressions) – Concept

A CTE is a temporary result set used within a query to simplify logic.

**Used for:**

* Breaking complex logic into steps
* Reusing intermediate results
* Simplifying joins and aggregations

**Advanced usage:**

* Multiple layered CTEs
* Customer-level aggregations
* Tracking latest activities (e.g., last claim)
* Combining multiple derived datasets

CTEs improved readability and made debugging significantly easier.

---

### Phase 6 – Window Functions

Used for row-level analysis without collapsing data.

**Key applications:**

* Ranking customers and agents
* Comparing values across rows
* Time-based trend analysis

**Techniques:**

* Partitioning (grouping data logically)
* Ordering (sequential calculations)

---

### Phase 7 – Final Output

Combined all processed data into a final dataset.

**Enhancements:**

* Added derived columns (e.g., risk indicators)
* Stored output in efficient formats (Parquet)
* Prepared data for reporting and dashboards

---

## Data Validation

Ensured accuracy and consistency throughout the pipeline.

**Validation checks:**

* Record count comparison (before vs after transformation)
* Null value verification
* Duplicate removal validation
* Referential integrity checks

---

## Key Insights

* Identified high-risk customers based on claim patterns
* Detected temporal trends in claims and premiums
* Evaluated agent performance
* Analyzed customer distribution across regions

---

## Technologies Used

* **PySpark** → Data processing and transformation
* **SQL** → Advanced analytics (Subqueries, CTEs, Window Functions)
* **Parquet** → Efficient data storage

---

## Conclusion

This project demonstrates a complete end-to-end data engineering and analytics workflow:

* Data understanding
* Data cleaning and validation
* Transformation
* Advanced SQL-based analysis

The use of **Subqueries, CTEs, and Window Functions** enabled solving complex business problems in a scalable and structured manner.
