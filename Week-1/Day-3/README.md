# **Phase 3 – SQL Conditional Logic & Window Functions (Week 1 - Day 3)**

## **🔹 Objective**

Develop advanced SQL capabilities by applying **conditional logic (`CASE WHEN`)** and **window functions** for analytical problem-solving.

This phase focuses on:

* Writing conditional transformations using business rules
* Categorizing data dynamically
* Performing ranking and ordering using window functions
* Conducting partition-based analysis

---

## **🔹 Problem Statement**

Multiple datasets were used, including:

* `employees`
* `customer_usage`
* `orders`

### **Key Requirements**

* Apply `CASE WHEN` for business logic implementation
* Solve nested conditional scenarios
* Use window functions (`ROW_NUMBER`, `RANK`, `DENSE_RANK`)
* Perform grouped analysis using `PARTITION BY`

---

## **🔹 Architecture / Approach**

1. **Data Understanding**

   * Analyzed dataset structures and business requirements
   * Identified key columns for transformations and analysis

2. **Conditional Transformations**

   * Applied `CASE WHEN` for categorization
   * Implemented nested conditions for complex business logic

3. **Window-Based Analytics**

   * Used window functions for ranking and comparison
   * Applied `PARTITION BY` and `ORDER BY` for grouped computations

4. **Validation**

   * Verified outputs using sample datasets
   * Ensured correctness of ranking and conditional outputs

---

## **🔹 Key Concepts & Transformations**

### **CASE WHEN (Conditional Logic)**

* Used to apply rule-based transformations
* Enables dynamic categorization of data

#### **Example**

```sql id="case1"
CASE 
    WHEN salary > 80000 THEN 'High'
    ELSE 'Low'
END
```

---

### **Nested CASE WHEN**

* Used for multi-level or dependent conditions
* Handles complex business rules efficiently

---

### **Window Functions**

| Function       | Description                       |
| -------------- | --------------------------------- |
| `ROW_NUMBER()` | Assigns unique sequential numbers |
| `RANK()`       | Assigns rank with gaps            |
| `DENSE_RANK()` | Assigns rank without gaps         |

---

### **Window Clauses**

| Clause         | Purpose                                |
| -------------- | -------------------------------------- |
| `PARTITION BY` | Divides data into logical groups       |
| `ORDER BY`     | Defines ordering within each partition |

---

## **🔹 Analytical Use Cases**

* Employee ranking based on salary
* Department-wise ranking analysis
* Customer segmentation based on usage patterns
* Bonus and salary-based categorization
* Identification of high-value vs low-value users

---

## **🔹 Outputs / Deliverables**

* Ranked employee datasets
* Department-level ranking insights
* Customer usage categorization
* Business rule-based transformations
* Analytical datasets for decision-making

---

## **🔹 Data Engineering Best Practices Applied**

* Ensured correct **evaluation order in CASE WHEN**
* Avoided **overlapping conditions**
* Used **PARTITION BY correctly** to maintain logical grouping
* Explicitly defined sorting (`ASC` / `DESC`)
* Validated ranking outputs for accuracy

---

## **🔹 Challenges & Resolutions**

| Challenge                       | Resolution                                  |
| ------------------------------- | ------------------------------------------- |
| Understanding nested CASE logic | Broke conditions into smaller logical steps |
| RANK vs DENSE_RANK confusion    | Practiced with sample datasets              |
| Writing complex conditions      | Structured queries incrementally            |
| Handling multiple conditions    | Used clear and ordered logic blocks         |

---

## **🔹 Key Learnings**

* Strong understanding of **SQL conditional logic**
* Ability to implement **real-world business rules**
* Practical expertise in **window functions**
* Clear distinction between **grouping vs partitioning**
* Improved **analytical problem-solving skills in SQL**

---

## **🔹 Pipeline Flow**

```id="sqlwinflow"
Data Understanding → Conditional Logic → Window Functions → Analysis → Validation
```

---

## **🔹 Tech Stack**

* **Language:** SQL
* **Concepts:** CASE WHEN, Window Functions, Ranking, Partitioning
* **Data Type:** Relational Tables
