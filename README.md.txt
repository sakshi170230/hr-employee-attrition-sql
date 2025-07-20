# HR Employee Attrition Analysis Using SQL

This project analyzes employee attrition using SQL to identify patterns and insights that may help HR departments improve employee retention.

## Project Overview

The dataset contains information on 1,470 employees, including features like age, department, job role, monthly income, overtime status, and whether the employee has left the organization. A sample of 50 rows is used for demonstration in this project.

The primary goal is to write SQL queries to explore the relationships between attrition and different employee attributes.

## Dataset

- Source: IBM HR Analytics Employee Attrition dataset
- Format: CSV (converted to SQL insert statements)
- Sample Size: 50 records (for demonstration purposes)
- Key columns:
  - Attrition
  - Age
  - Department
  - JobRole
  - MonthlyIncome
  - Overtime
  - EducationField
  - Gender

## Tools and Technologies

- SQLite
- SQL (DDL, DML, aggregate queries, subqueries)
- Git & GitHub

## How to Use

1. Clone the repository:

```bash
git clone https://github.com/sakshi170230/hr-employee-attrition-sql.git
cd hr-employee-attrition-sql
Launch SQLite and run:

bash
Copy
Edit
sqlite3 hr_data.db
.read schema.sql
.read hr_data_inserts.sql
.read hr_queries.sql
View query results in the terminal.

SQL Queries
The following types of analysis are performed:

Count of total employees

Count and percentage of attrition

Attrition by department and job role

Average income by department

Gender-wise attrition

Attrition by overtime status

Attrition across age groups and education fields

Sample Insights
Approx. 24% of employees in the sample have left.

Sales department has higher attrition compared to others.

Employees doing overtime show significantly higher attrition.

Monthly income does not always correlate with retention.

R&D department shows lower attrition compared to Sales.

File Structure
pgsql
Copy
Edit
.
├── schema.sql            -- Table schema for the HR dataset
├── hr_data_inserts.sql   -- INSERT statements (50 rows)
├── hr_queries.sql        -- SQL analysis queries
├── insights.md           -- Summary of key insights (optional)
└── README.md             -- Project documentation
Author
Sakshi Mishra
B.Tech, Alliance College of Engineering and Design
GitHub: sakshi170230