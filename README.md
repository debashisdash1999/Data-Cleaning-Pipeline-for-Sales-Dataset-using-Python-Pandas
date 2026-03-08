# Sales Data Cleaning and Validation using Python (Pandas)

## Project Overview

This project demonstrates the process of cleaning and preparing a raw sales dataset using Python and the Pandas library.
The dataset initially contained missing values, invalid entries, incorrect data types, and inconsistent records. The goal of this project was to transform the raw dataset into a clean, structured, and analysis-ready format.

---

## Dataset Description

The dataset contains transaction-level sales records with the following columns:

* Transaction ID
* Item
* Quantity
* Price Per Unit
* Total Spent
* Payment Method
* Location
* Transaction Date

These fields represent individual purchase transactions in a retail environment.

---

## Data Cleaning Steps

### 1. Data Loading

The dataset was imported from a CSV file into a Pandas DataFrame for further processing and analysis.

### 2. Initial Data Exploration

Basic inspection of the dataset was performed to understand the structure of the data.
This included reviewing column names, checking data types, and identifying potential issues within the dataset.

### 3. Duplicate Removal

Duplicate records were identified and removed to ensure each transaction was represented only once in the dataset.

### 4. Handling Invalid Values

The dataset contained invalid entries such as **"UNKNOWN"** and **"ERROR"**.
Rows containing these values were removed to maintain data quality and reliability.

### 5. Data Type Correction

Several columns were stored in incorrect formats.
Appropriate data types were assigned to ensure proper data handling:

* Transaction ID → String
* Item → String
* Quantity → Integer
* Price Per Unit → Float
* Total Spent → Float
* Payment Method → String
* Location → String
* Transaction Date → Datetime

Correct data types allow accurate calculations and enable efficient data analysis.

### 6. Index Reset

After removing invalid rows and duplicates, the DataFrame index was reset to maintain a clean and sequential row structure.

---

## Data Validation

To ensure the accuracy and integrity of the dataset, additional validation checks were performed.

### Transaction ID Validation

Each transaction ID was verified to ensure it followed the expected format beginning with the prefix **"TXN_"**.

### Revenue Validation

A validation check was performed to confirm that the **Total Spent** value matched the calculation:

**Total Spent = Quantity × Price Per Unit**

This step helped identify potential inconsistencies in financial records.

---

## Final Dataset

After completing the cleaning and validation process:

* Invalid records were removed
* Duplicate rows were eliminated
* Data types were corrected
* Data quality checks were applied

The final dataset is clean, consistent, and ready for further analysis or reporting.

---

## Tools and Technologies Used

* Python
* Pandas
* Jupyter Notebook
* CSV Data Files


