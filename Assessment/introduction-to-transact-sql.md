<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Introduction to Transact-SQL

1. In a normalized database, which two artifacts define relationships between tables?

    - [ ] A. column map
    - [ ] B. primary key
    - [ ] C. table map
    - [ ] D. foreign key

    <br>

    <details>
    <summary>Show answer</summary>
    primary key & foreign key
    </details>

    <br>
	
2. True or false: When using an alias, you must include the AS keyword.

    - [ ] A. True
    - [ ] B. False
	
    <br>

    <details>
    <summary>Show answer</summary>
    False, the AS keyword is optional
    </details>

    <br>

3. 	You write a query that returns the Name and Price columns from a table named Product in the Production schema. In the resulting rowset, you want the Name column to be named ProductName.

    Which of the following Transact-SQL statements should you use?
    - [ ] A. 	 ```sql SELECT * FROM Product;  ```
    - [ ] B. 	 ```sql SELECT Name AS ProductName, Price FROM Production.Product;  ```
    - [ ] C. 	 ```sql SELECT ProductName, Price FROM Production.Product;  ```
    - [ ] D. 	 ```sql SELECT Name, Price FROM dbo.Product;  ```
	

    <br>

    <details>
    <summary>Show answer</summary>
    SELECT Name AS ProductName, Price FROM Production.Product;  
    </details>

    <br>


4. 	You need to retrieve data from a column that is defined as char(1). If the value in the column is a digit between 0 and 9, the query should return it as an integer value. Otherwise, the query should return NULL.

    Which two functions can you use to accomplish this?
    - [ ] A. 	TRY_CAST
    - [ ] B. 	CAST
    - [ ] C. 	STR
    - [ ] D. 	TRY_CONVERT
    - [ ] E. 	CONVERT

    <br>

    <details>
    <summary>Show answer</summary>
    TRY_CAST & TRY_CONVERT
    </details>

    <br>

5. 	What are two statement types in SQL?

    - [ ] A. 	Data Manipulation Language (DML)
    - [ ] B. 	Data Query Language (DQL)
    - [ ] C. 	Data Definition Language (DDL)
    - [ ] D. 	Data Relational Language (DRL)
	

    <br>

    <details>
    <summary>Show answer</summary>
    Data Manipulation Language (DML) & Data Definition Language (DDL)
    </details>

    <br>


6. 	What does the HAVING keyword do?

    - [ ] A. 	It filters groups using a predicate.
    - [ ] B. 	It applies a calculation to a row.
    - [ ] C. 	It applies a grouping to the query.
    - [ ] D. 	It filters rows using a predicate.
	
    
     <br>

    <details>
    <summary>Show answer</summary>
    It filters groups using a predicate.
    </details>

    <br>


7. 	Which purpose does an alias serve in a select query?

    - [ ] A. 	It provides a hint to the query engine.
    - [ ] B. 	It behaves as a calculated value when performing updates.
    - [ ] C. 	It allows a query to return values from another database.
    - [ ] D. 	It changes the name of a returned column.
 
    <br>

    <details>
    <summary>Show answer</summary>
    It changes the name of a returned column.
    </details>

    <br>


 
8. You write a Transact-SQL query that returns the Cellphone column from the Sales.Customer table. Cellphone is a varchar column that permits NULL values. For rows where the Cellphone value is NULL, your query should return the text 'None'. Select the correct function to complete the following query:
    ```sql
    SELECT FirstName, LastName, __________(Cellphone, 'None') AS Cellphone
    FROM Sales.Customer;
    ```
    - [ ] A. 	COALESCE
    - [ ] B. 	NULLIF
    - [ ] C. 	ISNULL

    <br>

    <details>
    <summary>Show answer</summary>
    ISNULL
    </details>

    <br>


	
9. 	What does the * keyword do in a query?

    - [ ] A. 	It groups the results by their numeric value.
    - [ ] B. 	It returns all columns from the source table.
    - [ ] C. 	It joins multiple tables based on their relationship.
    - [ ] D. 	It filters the results to include only rows with values.


    <br>

    <details>
    <summary>Show answer</summary>
    It returns all columns from the source table.
    </details>

    <br>


10. Which style of language is SQL?

    - [ ] A. 	object-oriented
    - [ ] B. 	procedural
    - [ ] C. 	declarative
    - [ ] D. 	functional

    <br>

    <details>
    <summary>Show answer</summary>
    Structured Query Language (SQL) is is a set-based, declarative programming language, not an imperative programming language like C or BASIC.
    </details>

    <br>

<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 