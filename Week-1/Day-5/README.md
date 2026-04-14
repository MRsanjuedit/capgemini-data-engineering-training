# **Phase 5: Data Cleaning & Pattern Extraction

---

## 🔹 Objective

The objective of this phase is to perform data cleaning, transformation, and pattern extraction using PySpark and Regular Expressions (Regex).

This involves handling real-world data challenges such as inconsistent formats, missing values, and extracting structured information from unstructured text fields.

---

## 🔹 Problem Summary

The dataset used in this phase contained multiple data quality issues, including:

* Mixed-format text fields (combination of alphabets and numbers)
* Columns like email, phone numbers, and IDs requiring pattern extraction
* Presence of NULL values across several columns
* Inconsistent categorical values and formatting issues

The main goal was to:

* Clean and standardize the dataset
* Extract meaningful patterns using Regex
* Handle missing values effectively
* Perform structured transformations using PySpark

---

## 🔹 Approach

The solution was implemented in a step-by-step manner:

1. Loaded the dataset into a PySpark DataFrame
2. Performed initial data inspection (schema, nulls, inconsistencies)
3. Applied filtering conditions to isolate relevant records
4. Cleaned and standardized columns using transformations
5. Used Regular Expressions to extract patterns from text fields
6. Applied sorting and deduplication techniques
7. Generated a final structured and analysis-ready dataset

---

## 🔹 Key Transformations Used

### 🔸 Regular Expressions (Regex)

Regex was extensively used for extracting structured patterns from unstructured text:

* Extracted numeric values from alphanumeric strings
* Parsed email into username and domain
* Extracted country codes from phone numbers
* Identified patterns at the beginning/end of strings
* Separated alphabets and numeric components

**Why it matters:**
Regex is critical for processing real-world messy data where structured formats are not guaranteed.

---

### 🔸 Data Filtering

* Applied conditional filters on columns
* Combined multiple logical conditions for precise extraction

**Why it matters:**
Helps reduce noise and focus only on relevant subsets of data.

---

### 🔸 Column Transformations

* Renamed columns for clarity
* Created derived columns
* Standardized inconsistent categorical values

**Why it matters:**
Improves data readability and ensures consistency across datasets.

---

### 🔸 Conditional Logic

* Applied business rules using conditional expressions
* Categorized values based on defined logic

**Why it matters:**
Transforms raw data into meaningful, analysis-ready information.

---

### 🔸 NULL Handling

* Identified missing values across columns
* Replaced NULLs with appropriate defaults

**Why it matters:**
Prevents downstream processing errors and ensures data completeness.

---

### 🔸 Sorting & Deduplication

* Sorted records based on key columns
* Removed duplicate entries

**Why it matters:**
Ensures clean, reliable, and unique datasets.

---

### 🔸 Date Functions

* Added current date columns
* Derived past and future dates

**Why it matters:**
Supports time-based tracking and analysis.

---

### 🔸 String Operations

* Standardized text (upper/lower case)
* Split and formatted string columns

**Why it matters:**
Enhances usability and consistency of textual data.

---

## 🔹 Output / Results

After processing, the dataset achieved the following:

* Cleaned and standardized structure
* Extracted key patterns including:

  * Email components (username, domain)
  * Phone number country codes
  * Numeric and alphabetic segments
* Eliminated NULL-related inconsistencies
* Sorted and deduplicated records
* Final dataset ready for downstream analytics

---

## 🔹 Data Engineering Considerations

* Ensured robust NULL handling strategies
* Applied Regex carefully to avoid incorrect matches
* Maintained consistency across transformations
* Validated outputs after each processing step

---

## 🔹 Challenges Faced

* Designing accurate Regex patterns for complex strings
* Handling mixed-format columns
* Managing NULL values without data loss
* Ensuring transformations did not distort original data

---

## 🔹 Learnings

* Practical application of Regular Expressions in data processing
* Importance of data cleaning in real-world pipelines
* Efficient use of PySpark DataFrame transformations
* Handling missing and inconsistent data effectively
* Applying business logic using conditional transformations

---

## 🔹 Topics Covered

* Regular Expressions (pattern matching & extraction)
* Data filtering and transformation
* NULL value handling
* String manipulation
* Date functions
* Sorting and deduplication
