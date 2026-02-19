# Digital Prescription Analytics

This project focuses on analyzing digital prescription data using Python, MySQL, SQL, and Matplotlib.

The goal of this project is to clean raw healthcare data, apply business rules, store the cleaned data in MySQL, and generate meaningful insights using SQL queries and visualizations.

---

## Project Overview

Healthcare prescription data often contains duplicate records, missing values, and inconsistent entries.  

In this project:

- Raw CSV files are loaded using Python (Pandas)
- Data cleaning and validation are performed using defined business rules
- Clean data is inserted into MySQL tables
- SQL queries are used to perform analytical operations
- Matplotlib is used to generate visual dashboards

This project demonstrates an end-to-end ETL and analytics workflow.

---

## Business Rules Implemented

- Age must be between 0 and 100  
- Duplicate prescriptions are removed  
- Prescriptions without valid patient or doctor are rejected  
- Missing dosage or frequency is replaced with "Not Provided"  
- Unknown gender is marked as "U"  

---

## ETL Pipeline Flow

CSV Files (Dirty Data)  
        ↓  
Python ETL (Pandas)  
- Deduplication  
- Null handling  
- Business rule validation  
        ↓  
MySQL Clean Tables (DDL + Constraints)  
        ↓  
SQL Analytics + Matplotlib Dashboards  

---

## Business Insights Generated

- Most frequently prescribed medicines  
- Doctor-wise prescription volume comparison  
- Gender-wise prescription distribution  
- Age group vs number of prescriptions  
- Detect doctors issuing unusually high prescriptions  
- Daily prescription trend over time  
- Data quality comparison (before vs after cleaning)  

---

## Project Structure

```
Project_revature/
│
├── data/                       # Raw CSV datasets
│   ├── patients_1000.csv
│   ├── doctors_1000.csv
│   ├── medicines_1000.csv
│   └── prescriptions_1000.csv
│
├── Python-code/                # ETL and visualization notebook
│   └── project_python_file.ipynb
│
├── sql/                        # SQL schema and analytical queries
│   └── project_sql_query.sql
│
├── docs/                       # Project documentation
│   ├── Digital Prescription Record Analysis.docx
│   └── Digital Prescription Problem statement.docx
│
└── README.md
```

---

## Technologies Used

- Python (Pandas, NumPy)
- MySQL
- SQL
- Matplotlib
- PyMySQL
- Git & GitHub

---

## What I Learned

- Designing and implementing an ETL pipeline  
- Handling missing and invalid data properly  
- Writing analytical SQL queries  
- Connecting Python with MySQL  
- Creating business dashboards using Matplotlib  
- Managing and structuring projects using Git  

---

This project demonstrates a complete data pipeline from raw healthcare data to business insights.
