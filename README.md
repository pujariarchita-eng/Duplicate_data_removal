# AI/ML Internship Task: Duplicate Data Removal Using Pandas

## 📌 Project Overview

This project focuses on identifying and removing duplicate records from a dataset using Python and the Pandas library. Duplicate data removal is an important data-cleaning technique used before performing data analysis and machine learning.

This task was completed as part of the AI/ML internship at **Veda Technology**.

## 🎯 Objective

* Identify duplicate records in a dataset.
* Count the number of duplicate rows.
* Remove duplicate records using Pandas.
* Compare row counts before and after cleaning.
* Verify that no duplicate rows remain in the cleaned dataset.

## 🛠️ Tools and Technologies

* **Programming Language:** Python
* **Library:** Pandas
* **Environment:** Jupyter Notebook
* **Version Control:** GitHub

## 📊 Dataset Description

A sample student dataset was created manually using Pandas. It contains the following columns:

| Column Name | Description                             |
| ----------- | --------------------------------------- |
| Student_ID  | Unique identifier assigned to a student |
| Name        | Student's name                          |
| Age         | Student's age                           |
| Department  | Student's department                    |

The dataset contains 10 rows, including 3 duplicate records.

## ⚙️ Methodology

### 1. Create the Dataset

Create a sample dataset containing student information and intentional duplicate records.

### 2. Identify Duplicate Records

Use `df.duplicated()` to identify repeated rows.

### 3. Count Duplicates

Use `df.duplicated().sum()` to calculate the number of duplicate rows.

### 4. Remove Duplicates

Use `df.drop_duplicates()` to remove repeated rows while retaining the first occurrence.

### 5. Compare Row Counts

Compare the number of rows before and after cleaning to determine how many duplicate records were removed.

### 6. Verify the Cleaned Dataset

Use `cleaned_df.duplicated().sum()` to confirm that no full-row duplicates remain.

## 💻 Key Python Functions

```python
# Identify duplicate records
df.duplicated()

# Count duplicate records
df.duplicated().sum()

# Display duplicate records
df[df.duplicated()]

# Remove duplicate records
cleaned_df = df.drop_duplicates()

# Compare row counts
print("Rows before cleaning:", len(df))
print("Rows after cleaning:", len(cleaned_df))

# Verify duplicate removal
print("Remaining duplicates:", cleaned_df.duplicated().sum())
```

## 📈 Results

| Metric                        | Result |
| ----------------------------- | -----: |
| Original number of rows       |     10 |
| Duplicate records identified  |      3 |
| Duplicate records removed     |      3 |
| Rows after cleaning           |      7 |
| Remaining full-row duplicates |      0 |

## 🔍 Observations

* The original dataset contained 10 rows.
* Three duplicate records were identified.
* The duplicate records were removed successfully.
* The cleaned dataset contains 7 rows.
* No full-row duplicates remain after cleaning.

## ✅ Conclusion

This project demonstrates how Pandas can be used to perform basic data cleaning by identifying and removing duplicate records. The `duplicated()` and `drop_duplicates()` functions help improve data quality and prepare datasets for reliable analysis and machine learning.

## 📚 Learning Outcomes

* Learned to create and manipulate DataFrames using Pandas.
* Understood how to identify and count duplicate records.
* Learned to remove duplicate rows efficiently.
* Practiced comparing dataset sizes before and after cleaning.
* Understood the importance of data quality in machine learning workflows.

## 👩‍💻 Internship

**Organization:** Veda Technology
**Task:** Duplicate Data Removal
**Domain:** Artificial Intelligence and Machine Learning

---

*This project demonstrates a fundamental data preprocessing technique used in real-world data analysis and machine learning projects.*
