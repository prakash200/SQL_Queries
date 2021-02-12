# SQL_Queries
Here are SQL Queries on HR and NORTHWIND database . These Queries are written in #MYSQL_WORKBENCH# using SQL . These two Databases are RELATIONAL_DATABASES .
A relational database is a collection of data items with pre-defined relationships between them. These items are organized as a set of tables with columns and rows.

USE hr ;

----- 1. Write a query to display the names (first_name, last_name) using alias name “First Name", "Last Name

SELECT first_name FirstName ,last_name LastName
FROM employees;

-----  2. Write a query to get unique department ID from employee table
SELECT DISTINCT department_id
FROM employees ;

--------- 3. Write a query to get all employee details from the employee table order by first name, descending

select *
from employees
order by first_name desc ;

-----  4. Write a query to get the names (first_name, last_name), salary, PF of all the employees (PF is calculated as 15% of salary)

select first_name , last_name , salary , (salary*15)/100 PF
from employees; 

----- 5. Write a query to get the employee ID, names (first_name, last_name), salary in ascending order of salary

select employee_id ,first_name , last_name , salary 
from employees 
order by salary;

----- 6. Write a query to get the total salaries payable to employees

select sum(salary) Total_salaries
from employees ;
