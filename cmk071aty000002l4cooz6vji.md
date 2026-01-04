---
title: "100 Essential SQL Commands Every Data Analyst Should Know"
seoTitle: "100 Essential SQL Commands Every Data Analyst Should Know"
seoDescription: "Explore 100 essential SQL commands for data analysts to optimize querying, data manipulation, and reporting tasks in business environments"
datePublished: Sun Jan 04 2026 20:37:54 GMT+0000 (Coordinated Universal Time)
cuid: cmk071aty000002l4cooz6vji
slug: 100-essential-sql-commands-every-data-analyst-should-know
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1767558662324/8b59809e-a620-4a7c-b5c7-d677d8b32944.png
tags: data-analysis, sql, data-analyst

---

As a seasoned data analyst working in business environments, I use SQL every day to extract actionable insights, support decision-making, and drive operational efficiency. Structured Query Language (SQL) remains the cornerstone of relational database management, enabling analysts to query large datasets, transform raw data into meaningful metrics, and deliver timely reports to stakeholders. This guide consolidates 100 key SQL commands drawn from a widely referenced cheat sheet, organized into logical sections for quick navigation. Each command includes a concise description and practical insights relevant to real-world business applications. Whether you are optimizing sales reports, analyzing customer behavior, or building dashboards, this reference will strengthen your SQL toolkit and help you work more effectively with enterprise data systems.

---

## Core Data Retrieval and Manipulation Commands

These form the foundation of SQL, covering data querying, insertion, updates, and structural changes.

* **SELECT**: Retrieves data from a database. The starting point for most queries; use with clauses like WHERE for filtering.
    
* **INSERT**: Inserts new data into a database.
    
* **UPDATE**: Updates existing data in a database.
    
* **DELETE**: Deletes data from a database.
    
* **CREATE DATABASE**: Creates a new database.
    
* **CREATE TABLE**: Creates a new table in a database.
    
* **ALTER TABLE**: Modifies an existing table structure.
    
* **DROP TABLE**: Deletes a table from a database.
    
* **TRUNCATE TABLE**: Removes all records from a table. Faster than DELETE as it does not log individual row deletions.
    
* **CREATE INDEX**: Creates an index on a table. Improves query performance on large datasets.
    
* **DROP INDEX**: Deletes an index from a table.
    
* **JOIN**: Combines rows from two or more tables based on a related column.
    
* **INNER JOIN**: Returns rows when there is a match in both tables. The default JOIN type for matched records.
    
* **LEFT JOIN**: Returns all rows from the left table, and the matched rows from the right table.
    
* **RIGHT JOIN**: Returns all rows from the right table, and the matched rows from the left table.
    

## Joins, Set Operations, and Aggregation

Building on basics, these handle complex data combinations and summaries.

* **FULL JOIN**: Returns rows when there is a match in one of the tables. Also known as FULL OUTER JOIN; includes unmatched rows from both sides.
    
* **UNION**: Combines the results of two or more SELECT statements. Removes duplicates by default.
    
* **UNION ALL**: Combines the results of two or more SELECT statements, including duplicates.
    
* **GROUP BY**: Groups rows that have the same values into summary rows. Often used with aggregates like COUNT or SUM.
    
* **HAVING**: Filters records based on a specified condition. Applied after GROUP BY, unlike WHERE.
    
* **ORDER BY**: Sorts the result set in ascending or descending order.
    
* **COUNT**: Returns the number of rows that satisfy the condition.
    
* **SUM**: Calculates the sum of a set of values.
    
* **AVG**: Calculates the average of a set of values.
    
* **MIN**: Returns the smallest value in a set of values.
    
* **MAX**: Returns the largest value in a set of values.
    
* **DISTINCT**: Selects unique values from a column.
    
* **WHERE**: Filters records based on specified conditions.
    

## Conditional Logic and Operators

These enable precise filtering and decision-making in queries.

* **AND**: Combines multiple conditions in a WHERE clause. All must be true.
    
* **OR**: Specifies multiple alternative conditions in a WHERE clause. Any one can be true.
    
* **NOT**: Negates a condition in a WHERE clause.
    
* **BETWEEN**: Selects values within a specified range.
    
* **IN**: Specifies multiple values for a column.
    
* **LIKE**: Selects rows that match a specified pattern. Uses wildcards like % or \_.
    
* **IS NULL**: Checks for NULL values in a column.
    
* **IS NOT NULL**: Checks for non-NULL values in a column.
    
* **EXISTS**: Tests for the existence of any record in a subquery.
    
* **CASE**: Performs conditional logic in SQL statements. Like an if-then-else structure.
    
* **WHEN**: Specifies conditions in a CASE statement.
    
* **THEN**: Specifies the result if a condition is true in a CASE statement.
    
* **ELSE**: Specifies the result if no condition is true in a CASE statement.
    
* **END**: Ends the CASE statement.
    

## Constraints and Referential Integrity

Essential for maintaining data integrity in database design.

* **PRIMARY KEY**: Uniquely identifies each record in a table.
    
* **FOREIGN KEY**: Establishes a relationship between tables. Links to a PRIMARY KEY in another table.
    
* **CONSTRAINT**: Enforces rules for data in a table.
    
* **DEFAULT**: Specifies a default value for a column.
    
* **NOT NULL**: Ensures that a column cannot contain NULL values.
    
* **UNIQUE**: Ensures that all values in a column are unique.
    
* **CHECK**: Enforces a condition on the values in a column.
    
* **CASCADE**: Automatically performs a specified action on related records. For example, deletes child records when parent is deleted.
    
* **SET NULL**: Sets the value of foreign key columns to NULL when a referenced record is deleted.
    
* **SET DEFAULT**: Sets the value of foreign key columns to their default value when a referenced record is deleted.
    
* **NO ACTION**: Specifies that no action should be taken on related records when a referenced record is deleted. Often the default behavior.
    

## Advanced Querying and Pagination

Tools for limiting results, ranking, and conditional expressions.

* **RESTRICT**: Restricts the deletion of a referenced record if there are related records.
    
* **CASE WHEN**: Conditional expression in SELECT statements. Combines CASE with WHEN for inline logic.
    
* **WITH**: Defines a common table expression (CTE). Temporary result set for cleaner queries.
    
* **INTO**: Specifies a target table for the result set of a SELECT statement.
    
* **TOP**: Limits the number of rows returned by a query. Common in SQL Server.
    
* **LIMIT**: Limits the number of rows returned by a query (used in some SQL dialects like MySQL/PostgreSQL).
    
* **OFFSET**: Specifies the number of rows to skip before starting to return rows.
    
* **FETCH**: Retrieves rows from a result set one at a time. Often used with OFFSET for pagination.
    
* **ROW\_NUMBER()**: Assigns a unique sequential integer to each row in a result set.
    
* **RANK()**: Assigns a unique rank to each row in a result set, with gaps in the ranking sequence.
    
* **DENSE\_RANK()**: Assigns a unique rank to each row in a result set, with no gaps in the ranking sequence.
    

## Window Functions and Date Handling

For analytical queries over partitions and time-based operations.

* **NTILE()**: Divides the result set into a specified number of equally sized groups.
    
* **LEAD()**: Retrieves the value from the next row in a result set.
    
* **LAG()**: Retrieves the value from the previous row in a result set.
    
* **PARTITION BY**: Divides the result set into partitions to which the window function is applied separately.
    
* **ORDER BY**: Specifies the order of rows within each partition for window functions.
    
* **ROWS**: Specifies the window frame for window functions.
    
* **RANGE**: Specifies the window frame based on values rather than rows for window functions.
    
* **CURRENT\_TIMESTAMP**: Returns the current date and time.
    
* **CURRENT\_DATE**: Returns the current date.
    
* **CURRENT\_TIME**: Returns the current time.
    
* **DATEADD**: Adds a specified time interval to a date.
    
* **DATEDIFF**: Calculates the difference between two dates.
    

## Advanced Aggregation and Set Operations

For multi-level grouping, intersections, and dynamic operations.

* **DATEPART**: Extracts a specific part of a date.
    
* **GETDATE**: Returns the current date and time (similar to CURRENT\_TIMESTAMP).
    
* **GROUPING SETS**: Specifies multiple groupings for aggregation.
    
* **CUBE**: Generates all possible combinations of grouping sets for aggregation. Useful for OLAP-style reporting.
    
* **ROLLUP**: Generates subtotal values for a hierarchy of values.
    
* **INTERSECT**: Returns the intersection of two result sets.
    
* **EXCEPT**: Returns the difference between two result sets.
    
* **MERGE**: Performs insert, update, or delete operations on a target table based on the results of a join with a source table. Efficient for upserts.
    
* **CROSS APPLY**: Performs a correlated subquery against each row of the outer table.
    
* **OUTER APPLY**: Similar to CROSS APPLY, but also returns rows from the outer table that have no matching rows in the inner table.
    
* **PIVOT**: Rotates a table-valued expression by turning the unique values from one column into multiple columns in the output.
    

## Pivoting, Null Handling, and String/Numeric Functions

Finishing with transformations and manipulations for data cleaning.

* **UNPIVOT**: Rotates a table-valued expression by turning multiple columns into unique rows in the output.
    
* **COALESCE**: Returns the first non-NULL expression in a list. Great for handling nulls in reports.
    
* **NULLIF**: Returns NULL if the two specified expressions are equal, otherwise returns the first expression.
    
* **IIF**: Returns one of two values based on a Boolean expression. Shorthand for simple CASE.
    
* **CONCAT**: Concatenates two or more strings.
    
* **SUBSTRING**: Extracts a substring from a string.
    
* **CHARINDEX**: Finds the position of a substring within a string.
    
* **REPLACE**: Replaces all occurrences of a specified substring within a string with another substring.
    
* **LEN**: Returns the length of a string.
    
* **UPPER**: Converts a string to uppercase.
    
* **LOWER**: Converts a string to lowercase.
    
* **TRIM**: Removes leading and trailing spaces from a string.
    
* **ROUND**: Rounds a numeric value to a specified number of decimal places.
    

This comprehensive collection of 100 SQL commands covers foundational CRUD operations through to advanced window functions, pivoting techniques, and data transformation tools frequently used in large-scale business data analysis. Note that syntax and feature availability may vary across database systems (for example, MySQL, PostgreSQL, SQL Server, or Oracle), so always refer to your specific DBMS documentation for accurate details. Consistent practice in a development or sandbox environment will enhance your proficiency and enable more precise, impactful insights from organizational data.