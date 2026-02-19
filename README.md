# 🏥 Digital Prescription Analytics System

A CLI-based ETL and Healthcare Analytics project built using Python, MySQL, and Matplotlib.

This project extracts prescription data from CSV files, applies business validation rules, loads clean data into MySQL, and generates analytical insights using SQL and Matplotlib dashboards.

---

## 🚀 Project Overview

This system implements:

- End-to-end ETL pipeline
- Data cleaning and validation using business rules
- MySQL database design with constraints
- SQL-based analytics
- Data visualization using Matplotlib

---

## 📂 Dataset Files

The project uses the following CSV files:

- `patients_1000.csv`
- `doctors_1000.csv`
- `medicines_1000.csv`
- `prescriptions_1000.csv`

These files simulate real-world healthcare prescription data.

---

## 🧠 Business Rules Implemented

- Age must be between 0–100
- Duplicate prescriptions are removed
- Prescriptions without valid patient/doctor are rejected
- Missing dosage/frequency → "Not Provided"
- Unknown gender → "U"

---

## 🔄 ETL Pipeline Flow

CSV Files (Dirty Data)  
        ↓  
Python ETL using Pandas  
- Deduplication  
- Null handling  
- Business rule validation  
        ↓  
MySQL Clean Tables (DDL + Constraints)  
        ↓  
SQL Analytics  
        ↓  
Matplotlib Dashboard  

---

## 📊 Business Insights Generated

- Most frequently prescribed medicines
- Doctor-wise prescription volume comparison
- Gender-wise prescription distribution
- Age group vs number of prescriptions
- Detection of doctors issuing unusually high prescriptions
- Daily prescription trend over time
- Data quality comparison (before vs after cleaning)

---

## 🛠️ Technologies Used

- Python
- Pandas
- PyMySQL
- MySQL
- Matplotlib
- SQL

## 📁 Project Structure

```
Project_revature/
│
├── data/                       # Contains all raw CSV datasets
│   ├── patients_1000.csv
│   ├── doctors_1000.csv
│   ├── medicines_1000.csv
│   └── prescriptions_1000.csv
│
├── Python-code/                # ETL pipeline & analytics
│   └── project_python_file.ipynb
│
├── sql/                        # SQL DDL and analytical queries
│   └── project_sql_query.sql
│
├── docs/                       # Documentation files
│   ├── Digital Prescription Record Analysis.docx
│   └── Digital Prescription Problem statement.docx
│
└── README.md                   # Project documentation
```


## ⚙️ How to Run the Project

### 1️⃣ Install Required Libraries

```bash
pip install pandas pymysql matplotlib
```

### 2️⃣ Create MySQL Database

Create database:

```sql
CREATE DATABASE digital_prescription_db;
```

Run table creation scripts inside MySQL.

### 3️⃣ Open the Notebook

Open:

```
project_python_file.ipynb
```

Run cells step-by-step to:

- Perform ETL
- Load cleaned data into MySQL
- Execute analytics queries
- Generate Matplotlib dashboards

---

## 📈 Key Outcomes

- Designed normalized relational database schema
- Implemented data validation and cleaning rules
- Built ETL pipeline using Pandas
- Performed SQL-based analytical queries
- Created healthcare analytics dashboard using Matplotlib
- Handled database connections efficiently

---

## 🎯 Learning Highlights

This project demonstrates:

- Data Engineering concepts (ETL)
- SQL Analytics
- Business rule enforcement
- Data quality improvement
- Healthcare data analysis

---

## 👩‍💻 Author

Sahana P  
Healthcare Data Analytics Project  
