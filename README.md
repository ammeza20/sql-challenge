# sql-challenge
Employee Database Analysis

Overview

This project sets up and analyzes an Employee Database using PostgreSQL. The schema is designed to store employee details, department assignments, salaries, and job titles.

Technologies Used

SQL (PostgreSQL)

Jupyter Notebook (for queries & analysis)

CSV Files for Data Import

Database Schema

The database consists of six tables:

Employees

Stores employee details, including birth date, hire date, gender, and job title.

Departments

Stores department names and their unique department IDs.

Salaries

Records employee salaries.

Titles

Stores job titles and their corresponding IDs.

Department_Employee

Links employees to their respective departments.

Department_Manager

Identifies managers of each department.

File Structure

SCHEMA.sql - SQL script to create database tables.

Data_Analysis.sql - SQL queries for analyzing employee data.

CSV Files:

employees.csv

departments.csv

dept_emp.csv

dept_manager.csv

salaries.csv

titles.csv

Instructions

1. Setup Database

Open PostgreSQL and create a new database:

CREATE DATABASE employee_db;

Open SCHEMA.sql and execute the script to create tables.

2. Import Data

Run the following SQL commands to import CSV files:

COPY employees FROM 'path_to/employees.csv' DELIMITER ',' CSV HEADER;
COPY departments FROM 'path_to/departments.csv' DELIMITER ',' CSV HEADER;
COPY dept_emp FROM 'path_to/dept_emp.csv' DELIMITER ',' CSV HEADER;
COPY dept_manager FROM 'path_to/dept_manager.csv' DELIMITER ',' CSV HEADER;
COPY salaries FROM 'path_to/salaries.csv' DELIMITER ',' CSV HEADER;
COPY titles FROM 'path_to/titles.csv' DELIMITER ',' CSV HEADER;

3. Run Data Analysis Queries

Execute the queries from Data_Analysis.sql to:

Retrieve average salaries.

List employees by department.

Identify department managers.

Notes

Ensure the file paths in COPY commands match your local directory.

Use pgAdmin or PSQL to interact with the database.

