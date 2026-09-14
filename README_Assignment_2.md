# MySQL Assignment 2 – Querying Data

## Overview

This assignment focuses on querying and analyzing data from the `employee` database.

The assignment continues from the previous assignment and uses the provided Employee Data to populate the tables before executing the queries.

## Topics Covered

- DISTINCT Values
- Column Aliases using AS
- WHERE Clause and Operators
- ORDER BY
- LIMIT
- Aggregate Functions
- GROUP BY
- HAVING
- INNER JOIN
- LEFT JOIN
- RIGHT JOIN

## Queries Performed

### 1. DISTINCT Values
Retrieve distinct salaries from the Employees table.

### 2. Alias (AS)
Display:
- `age` as `Employee_Age`
- `salary` as `Employee_Salary`

### 3. WHERE Clause & Operators
- Find employees with salary greater than ₹50,000 and hired before 2016-01-01.
- Find an employee with a missing designation and update it to `Data Scientist`.

### 4. ORDER BY
Sort employees by department ID in ascending order and salary in descending order.

### 5. LIMIT
Display the first 5 employees hired in 2018.

### 6. Aggregate Functions
- Calculate the total salary in the Finance department.
- Find the minimum age among employees.

### 7. GROUP BY
- Find the maximum salary for each location.
- Calculate the average salary for each designation containing `Analyst`.

### 8. HAVING
- Find departments with fewer than 3 employees.
- Find locations with female employees whose average age is below 30.

### 9. INNER JOIN
List employee names, designations, and department names for employees assigned to a department.

### 10. LEFT JOIN
List all departments with the total number of employees in each department, including departments with no employees.

### 11. RIGHT JOIN
List all locations with the names of employees assigned to each location. Locations without employees should display `NULL` for the employee name.

## Database Tables

- `Departments`
- `Location`
- `Employees`

## Skills Demonstrated

- SELECT
- DISTINCT
- AS / Aliases
- WHERE
- ORDER BY
- LIMIT
- SUM
- MIN
- MAX
- AVG
- COUNT
- GROUP BY
- HAVING
- INNER JOIN
- LEFT JOIN
- RIGHT JOIN
- UPDATE
