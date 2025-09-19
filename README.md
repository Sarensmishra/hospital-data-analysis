
---

# **Hospital Data Analysis - SQL Project**

## 📖 Project Overview
This project demonstrates a comprehensive analysis of hospital operational data using **SQL**. The goal was to import, validate, and query a dataset to extract key performance indicators (KPIs) that could aid in hospital management decisions, such as resource allocation, financial planning, and departmental efficiency.

![SQL Hospital Analysis](https://images.unsplash.com/photo-1532938911079-1b06ac7ceec7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80)
*Image Source: Unsplash*

## 🗃️ Dataset
The dataset, `hospital.csv`, contains simulated records with the following attributes:
- `hospital_name`: Name of the hospital.
- `location`: City where the hospital is located.
- `department`: Medical department (e.g., Cardiology, Neurology).
- `doctors_count`: Number of doctors in the department.
- `patients_count`: Number of patients admitted.
- `admission_date`: Date of patient admission.
- `discharge_date`: Date of patient discharge.
- `medical_expenses`: Total medical expenses for the treatment.

## 🛠️ Tech Stack
- **Database System:** PostgreSQL
- **Language:** SQL
- **Tools:** pgAdmin (or any PostgreSQL client)

## 📋 Project Steps

### 1. Database Schema Design
The first step was to design a SQL table schema that accurately reflected the structure of the CSV file.
```sql
CREATE TABLE hospital_data (
    hospital_name VARCHAR(255),
    location VARCHAR(100),
    department VARCHAR(100),
    doctors_count INTEGER,
    patients_count INTEGER,
    admission_date DATE,
    discharge_date DATE,
    medical_expenses NUMERIC(10, 2)
);
```

### 2. Data Import & Validation
The data was imported into PostgreSQL using the pgAdmin import utility. A simple `SELECT` statement was used to validate the successful import and check data integrity.
```sql
SELECT * FROM hospital_data;
```

### 3. SQL Querying & Analysis
Ten specific business questions were answered using advanced SQL queries, leveraging aggregation, grouping, sorting, and date functions.

## 🔍 Key Analysis & Insights

The SQL queries were designed to find answers to the following critical questions:

1.  **Total Number of Patients** across all hospitals.
2.  **Average Number of Doctors** per hospital.
3.  **Top 3 Departments** with the highest number of patients.
4.  Hospital with the **Maximum Medical Expenses**.
5.  **Daily Average Medical Expenses** for each hospital.
6.  Record for the **Longest Hospital Stay** by a patient.
7.  **Total Patients Treated** in each city.
8.  **Average Length of Stay** for patients in each department.
9.  Department with the **Lowest Number of Patients**.
10. **Monthly Medical Expenses Report** for financial tracking.

## 📊 Sample Insights & Visualization
*(You can add a screenshot of your query results here. You can create a simple chart in Excel or Google Sheets based on your results and add it below.)*

**Example: Top 3 Departments by Patient Count**
| Department | Total Patients |


*You can use a tool like [QuickDBD](https://www.quickdatabasediagrams.com/) to generate an ERD diagram, even if it's a single table, to make your README more professional.*

![Database Schema](https://i.imgur.com/qvQ+W0k.png)

## 🚀 How to Run This Project Locally

1.  **Prerequisites:** Ensure you have PostgreSQL and pgAdmin installed on your system.
2.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-username/hospital-data-sql-analysis.git
    ```
3.  **Set Up Database:**
    -   Open pgAdmin and create a new database (e.g., `hospital_db`).
    -   Run the `CREATE TABLE` statement provided in the `queries.sql` file to create the table schema.
4.  **Import Data:**
    -   Right-click on the `hospital_data` table in pgAdmin.
    -   Select **Import/Export**.
    -   Switch to **Import**, browse to the `hospital.csv` file, and set the format to CSV. Click **OK**.
5.  **Run Queries:**
    -   Open a new query tool in pgAdmin.
    -   Copy and execute the queries from the `queries.sql` file one by one to see the results.

## 📁 Repository Structure
```
hospital-data-sql-analysis/
│
│── hospital.csv                 # Original dataset
│
├── queries.sql                      # All SQL queries and table schema
│
└── README.md                        # Project documentation (this file)
```

## ✨ Skills Demonstrated
- **Data Definition Language (DDL):** `CREATE TABLE`
- **Data Manipulation Language (DML):** `SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`
- **Aggregate Functions:** `SUM()`, `AVG()`, `COUNT()`
- **Date Functions:** `EXTRACT()`, date arithmetic
- **Data Import/Export:** Using pgAdmin's GUI tools
- **Analytical Thinking:** Translating business questions into SQL queries.

## 📝 Conclusion
This project served as a practical application of core SQL concepts. It reinforced my ability to not just write queries, but to manage the entire data analysis workflow—from database design and data ingestion to generating actionable insights.

## 📧 Contact
- **Name:** Sarens Mishra
- **Email:** sarensmishra@gmail.com
- **LinkedIn:**  (https://in.linkedin.com/in/sarens-mishra-359575352)

---

