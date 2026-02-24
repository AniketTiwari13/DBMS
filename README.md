# 📊 DBMS Lab Experiments: Portfolio

## 🎓 Author: ANIKET TIWARI

A documentation of my progress through the DBMS syllabus. I’ve included all the SQL scripts used in our lab sessions, starting with simple table setups and moving into advanced queries and data reporting.

---

## 🗄️ Database Schema

The database 2CSE22_1403 consists of two primary tables:

### 1. EMPLOYEE
Contains details about staff, including salaries, roles, and department associations.

| Column | Type | Description |
| :--- | :--- | :--- |
| EMPNO | INT (PK) | Unique Employee ID |
| ENAME | VARCHAR | Employee Name |
| JOB | VARCHAR | Designation/Role |
| HIREDATE | DATE | Date of joining |
| SAL | DECIMAL | Monthly Salary |
| COMM | DECIMAL | Commission (where applicable) |
| DEPTNO | INT | Department ID |

### 2. DEPARTMENT
Contains the organizational structure.

| DEPTNO | DNAME |
| :--- | :--- |
| 10 | RESEARCH |
| 20 | ACCOUNTING |
| 30 | SALES |
| 40 | OPERATIONS |

---

## 🚀 Getting Started

To set up this environment locally, run the following commands in your SQL terminal:

sql
-- Create and use the database
CREATE DATABASE 2CSE22_1403;
USE 2CSE22_1403;

-- Create the Employee Table
CREATE TABLE EMPLOYEE (
    EMPNO INT PRIMARY KEY,
    ENAME VARCHAR(20) NOT NULL,
    JOB VARCHAR(20),
    MGR INT,
    HIREDATE DATE,
    SAL DECIMAL(10,2),
    COMM DECIMAL(10,2),
    DEPTNO INT
);


## BY- Aniket Tiwari
