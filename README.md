# Preface

This project is about migrating enterprise data from SQL Server into Postgres

We'll be using

- SQL
- Python
- Jupyter notebook

# Pseudo code

## High-Level
1.Audit the data in SQL Server(before migration)
2.Extract data from SQL Server(SSMS)
3.Transform the data
4.Load the data in PostgreSQL
5.Validate the data(after migration)
6.Generate a validation report

# Low-Level
- Create a.env file 
- Load env variables
- Connect to SQL Server(pyodbc)
- Connect to Postgres(psycopg2)
- Audit the data
- For each table
    - Get row count
    - Extract all rows
    - Transform the column names to lowercase
    - Convert the data types
    - Create tables in Postgres
    - Load tables into Postgres
- Run post-data migration checks
- Generate validation report

