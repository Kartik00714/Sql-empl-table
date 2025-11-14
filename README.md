# Sql-empl-table
.

📁 usersaitm Database – Employee Table (emp)

This repository contains a MySQL dump file that defines and populates the emp table inside the usersaitm database.
The dump was generated using MySQL 8.0.44 on Windows (x86_64).


usersaitm_emp

📄 Table: emp

The SQL file creates an emp table with the following structure:

CREATE TABLE `emp` (
  `name` varchar(30) DEFAULT NULL,
  `empid` int DEFAULT NULL,
  `salary` int DEFAULT NULL
);


usersaitm_emp

Columns
Column	Type	Description
name	VARCHAR(30)	Employee name
empid	INT	Unique employee ID
salary	INT	Employee salary (annual)
🧪 Sample Data

The file inserts 5 employee records into the table:

INSERT INTO `emp` VALUES 
('Kartik',1000,1500000),
('Shivam',1001,1200000),
('Sujal',1002,950000),
('Prince',1003,100000),
('Pawan',1004,890000);


usersaitm_emp

Inserted Records
Name	EmpID	Salary
Kartik	1000	15,00,000
Shivam	1001	12,00,000
Sujal	1002	9,50,000
Prince	1003	1,00,000
Pawan	1004	8,90,000
🚀 How to Import the SQL File
Using MySQL CLI
mysql -u root -p usersaitm < usersaitm_emp.sql

Using MySQL Workbench / phpMyAdmin

Create database usersaitm (if not exists)

Go to Import

Select usersaitm_emp.sql

Run

🧾 Notes

No primary key is defined in the table; you may add one depending on your project requirements.

The salary field stores numeric amounts without formatting.

Character set used: utf8mb4


usersaitm_emp
