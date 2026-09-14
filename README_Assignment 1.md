# MySQL Assignment 1 – DDL Commands & Constraints

## Overview

This repository contains **MySQL Assignment 1**, focused on **DDL (Data Definition Language) commands and database constraints**.

The assignment uses an employee database schema containing three main tables:

- `Departments`
- `Location`
- `Employees`

## Assignment Objectives

### DDL Commands

The assignment demonstrates:

1. **CREATE** – Create the `employee` database and required tables.
2. **ALTER** – Add, modify, drop, and rename columns in the `Employees` table.
3. **RENAME** – Rename the `Departments` and `Location` tables.
4. **TRUNCATE** – Truncate the `Employees` table.
5. **DROP** – Drop the `Employees` table and the `employee` database.

### Constraints

The database is recreated with:

- **PRIMARY KEY** for unique identifiers.
- **NOT NULL** for required values.
- **UNIQUE** to prevent duplicate department names and locations.
- **AUTO_INCREMENT** for sequential location IDs.
- **ENUM** to restrict gender values to `M` or `F`.
- **CHECK** to ensure employee age is 18 or above.
- **DEFAULT** to automatically assign the current date to `hire_date`.
- **FOREIGN KEY** relationships between employees, departments, and locations.

## Database Schema

### Departments

| Column | Data Type | Constraint |
|---|---|---|
| `department_id` | INT | PRIMARY KEY |
| `department_name` | VARCHAR(100) | NOT NULL, UNIQUE |

### Location

| Column | Data Type | Constraint |
|---|---|---|
| `location_id` | INT | PRIMARY KEY, AUTO_INCREMENT |
| `location` | VARCHAR(30) | NOT NULL, UNIQUE |

### Employees

| Column | Data Type | Constraint |
|---|---|---|
| `employee_id` | INT | PRIMARY KEY |
| `employee_name` | VARCHAR(50) | NOT NULL |
| `gender` | ENUM('M','F') | Restricted values |
| `age` | INT | CHECK (age >= 18) |
| `hire_date` | DATE | DEFAULT (CURRENT_DATE) |
| `designation` | VARCHAR(100) | — |
| `department_id` | INT | FOREIGN KEY |
| `location_id` | INT | FOREIGN KEY |
| `salary` | DECIMAL(10,2) | — |

## File Included

- `Assignment 1.sql` – SQL statements for the DDL commands and constraints.

## Skills Demonstrated

- MySQL database creation
- Table creation and alteration
- Table renaming
- TRUNCATE and DROP operations
- Primary and foreign keys
- NOT NULL and UNIQUE constraints
- ENUM and CHECK constraints
- AUTO_INCREMENT
- DEFAULT values
- Relationships between tables
