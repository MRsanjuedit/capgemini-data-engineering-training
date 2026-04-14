# **Phase 4: SQL Data Cleaning & Transformation

---

## 🔹 Objective

In this phase, the objective is to understand and apply SQL functions for data cleaning and transformation.

The focus is on handling missing values, standardizing text data, and performing date-based operations to derive meaningful insights.

---

## 🔹 Problem Summary

The datasets used in this phase contained several common data quality issues:

* Missing (NULL) values affecting calculations
* Text data with inconsistent formatting (uppercase, lowercase, extra spaces)
* Date columns requiring extraction and comparison

The key tasks were to:

* Handle NULL values effectively
* Clean and standardize text data
* Extract insights from date columns
* Apply conditional logic for data classification

---

## 🔹 Approach

A systematic approach was followed to clean and transform the data:

1. Identified columns with missing and inconsistent values
2. Applied NULL-handling functions to avoid incorrect results
3. Standardized string data for consistency and readability
4. Used date functions to extract components and calculate differences
5. Applied conditional logic to categorize and enrich data

---

## 🔹 Key Transformations Used

### 🔸 NULL Functions

These functions were used to handle missing values in the dataset:

* Replaced NULL values with default values
* Ensured calculations do not return NULL results
* Enabled safe comparisons without unexpected behavior

**Why it matters:**
Proper NULL handling is essential to ensure accuracy in aggregations and calculations.

---

### 🔸 String Functions

Used to clean and standardize textual data:

* Converted text to uppercase/lowercase
* Formatted strings into readable formats
* Extracted specific parts of strings
* Removed extra spaces and unwanted characters

**Why it matters:**
Improves data consistency, readability, and usability for analysis and reporting.

---

### 🔸 Date Functions

Used for handling and analyzing date-related data:

* Extracted components like year and month
* Calculated differences between dates
* Retrieved current date for comparisons
* Converted dates into required formats

**Why it matters:**
Enables time-based analysis such as duration calculation and trend identification.

---

### 🔸 Conditional Logic

Applied logic-based transformations:

* Categorized data using CASE statements
* Applied business rules to derive new columns

**Why it matters:**
Helps convert raw data into meaningful, business-relevant insights.

---

## 🔹 Output / Results

The transformations resulted in:

* Clean datasets with properly handled NULL values
* Standardized and well-formatted text data
* Accurate date-based calculations
* Categorized outputs based on defined business rules

---

## 🔹 Data Engineering Considerations

* Proper NULL handling ensures reliable and accurate results
* Consistent string formatting improves downstream usability
* Accurate date calculations are critical for time-based analysis
* Logical classification enhances business understanding of data

---

## 🔹 Challenges Faced

* Managing NULL values without impacting calculations
* Selecting appropriate string functions for different scenarios
* Understanding date difference calculations
* Applying correct conditional logic for classification

---

## 🔹 Learnings

* Importance of data cleaning before analysis
* Practical application of SQL NULL-handling functions
* Role of string functions in improving data quality
* Use of date functions for deriving insights
* Applying conditional logic for meaningful categorization

---

## 🔹 Topics Covered

* NULL handling functions (COALESCE, IFNULL, etc.)
* String manipulation functions
* Date functions and calculations
* Conditional logic (CASE statements)
* Data cleaning and transformation in SQL
