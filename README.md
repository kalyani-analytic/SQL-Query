# 📘 SQL Table Design and Data Querying

## 📌 Overview

This assignment focuses on designing relational database tables and performing basic SQL operations. It includes creating tables, inserting data, and executing queries to retrieve and analyze information.

---

## 🗂️ Tables Created

### 1. Employees Table

The **Employees** table stores employee-related information.

**Structure:**

* EmpID (INT, Primary Key)
* Name (VARCHAR(50))
* Department (VARCHAR(30))
* Salary (DECIMAL(10,2))

**SQL Query:**

```sql
CREATE TABLE Employees (
    EmpID INT PRIMARY KEY,
    Name VARCHAR(50),
    Department VARCHAR(30),
    Salary DECIMAL(10,2)
);
```

---

### 2. Departments Table

The **Departments** table stores department-related information.

**Structure:**

* DeptID (INT, Primary Key)
* DeptName (VARCHAR(50))
* Location (VARCHAR(50))

**SQL Query:**

```sql
CREATE TABLE Departments (
    DeptID INT PRIMARY KEY,
    DeptName VARCHAR(50),
    Location VARCHAR(50)
);
```

---

## 📥 Data Insertion

### Employees Table Data

```sql
INSERT INTO Employees (EmpID, Name, Department, Salary) VALUES
(1, 'John Doe', 'HR', 50000),
(2, 'Jane Smith', 'IT', 60000),
(3, 'Alice Johnson', 'Finance', 55000),
(4, 'Bob Brown', 'HR', 45000),
(5, 'Charlie White', 'IT', 65000);
```

📸 Output Screenshot: **screenshot_1**

---

### Departments Table Data

```sql
INSERT INTO Departments (DeptID, DeptName, Location)
VALUES (101, 'Sales', 'New York');
```

📸 Output Screenshot: **screenshot_2**

---

## 🔍 SQL Queries and Outputs

### a. Retrieve All Employees

```sql
SELECT * FROM Employees;
```

📸 Output Screenshot: **screenshot_3a**

---

### b. List Distinct Departments

```sql
SELECT DISTINCT Department FROM Employees;
```

📸 Output Screenshot: **screenshot_3b**

---

### c. Employees with Salary Greater Than 55000

```sql
SELECT * FROM Employees WHERE Salary > 55000;
```

📸 Output Screenshot: **screenshot_3c**

---

## ⚠️ Notes

* If tables already exist, they should be dropped or renamed before execution.
* All queries were executed successfully without errors.
* Screenshots are included as proof of execution.

---

## ✅ Conclusion

This assignment helped in understanding:

* Table creation using SQL
* Inserting records into tables
* Retrieving and filtering data using SQL queries

These concepts are fundamental for working with relational databases.
---
