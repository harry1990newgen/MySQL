Database Notes
📌 Basic Definitions
🔹 Data

Smallest unit of information.
Example: Information inside a single Excel cell.

🔹 Metadata

Data about data (information or details describing the data).

🔹 Database

A structured collection of data stored in rows and columns.

📂 Types of Databases
1️⃣ Structured Database

Data stored in rows & columns (tabular format) like Excel.

Examples:

Excel

MySQL

Oracle

PostgreSQL

2️⃣ Unstructured Database

Data not stored in row & column format.

Examples:

Images (jpg, png)

Text files (.txt)

PPT files

Word documents

🗣 Language to Communicate with Database
SQL (Structured Query Language)

Used to:

Create data

Fetch data

Insert data

Update data

Delete data

SQL is divided into:

Type	Meaning	Commands
DDL	Data Definition Language	CREATE, ALTER, DROP, INDEX
DML	Data Manipulation Language	SELECT, INSERT, UPDATE, DELETE
DCL	Data Control Language	GRANT, REVOKE
TCL	Transaction Control Language	COMMIT, ROLLBACK
🎯 Goal

Install MySQL Database

Create Database in MySQL

Create Credentials (Users)

Run DDL & DML Commands

Create Small Node.js Project

Connect Database with Node.js

Store and Fetch Data

🛠 MySQL Installation Commands
Installation Methods

Using yum/apt repository

Using wget/curl (official or third-party repository)

Using rpm -i

🔍 Check MySQL Version
mysql --version
mysql -V
systemctl status mysqld

Or inside MySQL:

SELECT VERSION();
🔐 Important MySQL Commands
Secure MySQL Installation
mysql_secure_installation
Login to MySQL
mysql -u root -p
Show Databases
SHOW DATABASES;
Create Database
CREATE DATABASE DevOps20;
👤 Create User in MySQL
CREATE USER 'user1'@'%' IDENTIFIED BY '1234';
GRANT ALL PRIVILEGES ON DevOps20.* TO 'user1'@'%';
FLUSH PRIVILEGES;
🗄 Working with Database
Select Database
USE DevOps20;
🧱 Create Table

Before creating table, decide:

Number of rows & columns

Column names

Data types

Table name

Data to insert

Example:

Table Name → Class20

Columns → Stud_Name, Class, Timing, Batch_No

Data Types → varchar(20), varchar(10), float, int

CREATE TABLE Class20 (
    Stud_Name VARCHAR(20),
    Class VARCHAR(10),
    Timing FLOAT,
    Batch_No INT
);
➕ Insert Data into Table

Steps:

Collect data

Select database

Insert using INSERT query

INSERT INTO Class20 VALUES ('harry', 'devops', 8.15, 20);
INSERT INTO Class20 VALUES ('rahul', 'devops', 8.15, 20);
INSERT INTO Class20 VALUES ('naveen', 'platform', 10.40, 22);
INSERT INTO Class20 VALUES ('pankaj', 'java', 11.30, 21);
Describe Table
DESCRIBE Class20;
🔎 SELECT Query (Fetch Data)

Used to retrieve data from table.

Syntax:
SELECT * FROM <table_name>;
SELECT column_name FROM <table_name>;
Examples:
SELECT * FROM Class20;
SELECT Stud_Name, Timing FROM Class20;
SELECT Stud_Name, Batch_No FROM Class20;
SELECT Batch_No FROM Class20;
SELECT Class FROM Class20;
SELECT Stud_Name, Timing, Class, Batch_No FROM Class20;
✅ Conclusion

Installed MySQL Database Server

Created Database → DevOps20

Created Table → Class20

Inserted Data into Table

Retrieved Data using SELECT Queries

🚀 Your basic database workflow is now complete!

If you want, I can also format this with:

Table of Contents

Better GitHub Markdown styling

Add diagrams

Add Node.js connection example

Just tell me 👍
