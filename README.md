# Task 4: E-commerce Database Aggregate Functions and Grouping

This repository contains an SQL script (`e_commerce_db_task4.sql`) focused on summarizing and analyzing data using 
aggregate functions and grouping within your E-commerce PostgreSQL database.

---

## Objective

The main goal of this task is to gain a clear understanding and hands-on experience in summarizing and analyzing tabular data effectively by:
* Applying **aggregate functions** such as `SUM()`, `COUNT()`, `AVG()` on numeric and other relevant columns.
* Using the **`GROUP BY`** clause to categorize data and apply aggregate functions to each distinct group.
* Filtering grouped data using the **`HAVING`** clause, which is specifically designed for conditions on aggregate results.
* Utilizing **`CASE`** statements within `SELECT` and `GROUP BY` for conditional categorization.
* Employing **subqueries** to perform calculations that can then be used in outer queries.

---

## Contents

* `e_commerce_db_task4.sql`: The primary SQL script containing various aggregate function and grouping query examples.

---

## Key Demonstrations

The script illustrates a range of queries involving aggregate functions and grouping, including:

* **Basic Aggregation**: Examples of calculating total counts (`COUNT()`), sums (`SUM()`), and averages (`AVG()`) across entire tables.
* **Grouping Data (`GROUP BY`)**:
    * Counting records per category (e.g., customers per city).
    * Calculating sums and averages for each distinct group (e.g., total stock per product category, average price per category).
* **Filtering Groups (`HAVING`)**: Applying conditions to the results of aggregate functions
* (e.g., finding categories with more than a certain number of items, or products with average order quantities above a threshold).
* **Conditional Aggregation (`CASE`)**: Categorizing data dynamically within the query and then aggregating based on these categories
* (e.g., counting products within specific price ranges).
* **Subqueries with Aggregation**: Using an aggregate result from a subquery to filter an outer query
* (e.g., selecting orders with amounts greater than the overall average order amount).

---

## How to Use

1.  **Prerequisite**: Ensure your E-commerce database schema and sample data are already set up and
2.   populated in your PostgreSQL environment. You should have completed:
    * [Task 1 - Database Setup and Schema Design](https://github.com/sanjay-it-is/e-commerce-db)
    * [Task 2 - Data Insertion and Handling Nulls](https://github.com/sanjay-it-is/e-commerce-db_task2)
    * [Task 3 - Basic SELECT Queries](https://github.com/sanjay-it-is/e-commerce-db_task3)
3.  **Connect to your Database**: Open your preferred PostgreSQL client (e.g., `psql` command line, pgAdmin, DBeaver).
4.  **Execute the Script**: You can run the `e_commerce_db_task4.sql` file against your `e_commerce_db` database.

    ```bash
    -- Example using psql:
    psql -U your_username -d e_commerce_db -f e_commerce_db_task4.sql
    ```
    Alternatively, you can copy and paste individual queries or the entire script into your client and execute them to see the results.

---

## 📝 Outcome

By working through this script, you will gain a clear understanding of how to effectively 
summarize, categorize, and analyze data within a relational database using SQL's powerful 
aggregate functions and grouping capabilities, forming the foundation for more advanced business intelligence and reporting.
