# **Phase 2 – SQL Joins, Aggregations & Data Analysis (Week 1 - Day 2)**

## **🔹 Objective**

Develop a strong foundation in **SQL joins, aggregations, and data analysis** by working with multiple related datasets and solving real-world query scenarios.

This phase focuses on:

* Combining data from multiple tables
* Performing aggregations using `GROUP BY`
* Solving practical SQL problems
* Understanding relational data modeling

---

## **🔹 Problem Statement**

Multiple relational tables were provided, including:

* `employees`
* `departments`
* `projects`
* `salary` *(optional dataset)*

### **Key Requirements**

* Perform different types of joins
* Apply grouping and aggregation operations
* Solve **30 SQL practice problems**
* Handle missing and inconsistent data

---

## **🔹 Architecture / Approach**

1. **Data Understanding**

   * Analyzed table schemas and relationships
   * Identified **primary keys** and **foreign keys**

2. **Data Integration**

   * Applied appropriate join types based on use case
   * Ensured correct mapping between related tables

3. **Aggregation & Analysis**

   * Used `GROUP BY` for summarization
   * Applied aggregate functions (`COUNT`, `SUM`, `AVG`)

4. **Filtering & Data Cleaning**

   * Used `WHERE` for row-level filtering
   * Used `HAVING` for post-aggregation filtering
   * Handled NULL values and inconsistencies

5. **Validation**

   * Verified outputs using sample datasets and expected results

---

## **🔹 Key Concepts & Transformations**

### **Joins**

| Join Type         | Description                                                  |
| ----------------- | ------------------------------------------------------------ |
| `INNER JOIN`      | Returns only matching records                                |
| `LEFT JOIN`       | Returns all records from left table + matches                |
| `RIGHT JOIN`      | Returns all records from right table + matches               |
| `FULL OUTER JOIN` | Returns all records from both tables                         |
| `SELF JOIN`       | Joins a table with itself (e.g., employee-manager hierarchy) |

---

### **GROUP BY & Aggregations (Core Concept)**

| Function   | Purpose                            |
| ---------- | ---------------------------------- |
| `GROUP BY` | Groups rows based on column values |
| `COUNT(*)` | Counts total records               |
| `SUM()`    | Calculates total values            |
| `AVG()`    | Calculates average values          |

#### **Example**

```sql id="sqlgrp1"
SELECT department, COUNT(*) AS emp_count
FROM employees
GROUP BY department;
```

**Use Cases:**

* Department-wise employee count
* Salary aggregation
* Project-level analysis

---

### **Filtering Techniques**

| Clause   | Purpose                         |
| -------- | ------------------------------- |
| `WHERE`  | Filters rows before aggregation |
| `HAVING` | Filters aggregated results      |

---

### **Data Cleaning Techniques**

* Removed NULL values using filtering conditions
* Handled missing relationships using joins
* Eliminated duplicate records
* Corrected inconsistent data
* Ensured proper data types

---

## **🔹 Analytical Use Cases**

* Employee–Manager hierarchy using **SELF JOIN**
* Employees with/without departments
* Projects with/without assigned employees
* Department-wise employee distribution
* Salary-based insights and aggregations
* Identifying employees without projects or departments

---

## **🔹 Outputs / Deliverables**

* Employee hierarchy dataset
* Department-level employee metrics
* Project allocation insights
* Aggregated salary reports
* Exception reports (missing relationships)

---

## **🔹 Data Engineering Best Practices Applied**

* Used appropriate **join strategies** to avoid data loss
* Handled **NULL values carefully** for accurate results
* Prevented **duplicate records during joins**
* Ensured correct application of **aggregations**
* Validated outputs using **test datasets and sampling**

---

## **🔹 Challenges & Resolutions**

| Challenge                  | Resolution                              |
| -------------------------- | --------------------------------------- |
| Choosing correct join type | Mapped use case to join behavior        |
| Handling NULL values       | Applied filtering and conditional logic |
| WHERE vs HAVING confusion  | Practiced query execution order         |
| Complex query writing      | Broke problems into smaller steps       |
| Implementing SELF JOIN     | Visualized hierarchical relationships   |

---

## **🔹 Key Learnings**

* Strong understanding of **SQL joins and relationships**
* Practical expertise in **GROUP BY and aggregations**
* Ability to solve **real-world SQL problems**
* Clear distinction between **WHERE vs HAVING**
* Importance of **data cleaning before analysis**
* Introduction to **window functions**

---

## **🔹 Pipeline Flow**

```id="sqlflow"
Data Understanding → Data Joining → Aggregation → Filtering → Analysis → Validation
```

---

## **🔹 Tech Stack**

* **Language:** SQL
* **Concepts:** Joins, Aggregations, Filtering, Data Analysis
* **Data Type:** Relational Tables
