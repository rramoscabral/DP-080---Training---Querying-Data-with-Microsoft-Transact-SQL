<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Using Table Expressions


1. What is an advantage of table variables over temporary tables?

    - [ ] A. 	They have a larger capacity.
    - [ ] B. 	They are serializable.
    - [ ] C. 	They cause fewer recompilations.
    - [ ] D. 	They can be persisted to disk. 
	

2. Which keyword is used to start the definition of a common table expression?

    - [ ] A. 	CREATE
    - [ ] B. 	BEGIN
    - [ ] C. 	APPLY
    - [ ] D. 	WITH
	
3. Which statement are derived tables created within?

    - [ ] A. 	DROP
    - [ ] B. 	BEGIN
    - [ ] C. 	SELECT
    - [ ] D. 	CREATE
	

4. You write the following query, which uses a common table expression:
    ```sql
    ____________________________________
    AS
    (
    SELECT MONTH(OrderDate), SalesOrderID
    FROM Sales.SalesOrder
    WHERE YEAR(OrderDate) = YEAR(GETDATE())
    )
    SELECT OrderMonth, COUNT(SalesOrderID) AS Orders
    FROM YTD_Orders
    GROUP BY OrderMonth;
    ```

    Which line of code is the correct first line for the above query?

    - [ ] A. 	WITH YTD_Orders
    - [ ] B. 	WITH YTD_Orders (OrderMonth AS int, SalesOrderID AS int)
    - [ ] C. 	DECLARE @YTD_Order
    - [ ] D. 	SELECT YTD_Orders =
    - [ ] E. 	WITH YTD_Orders (OrderMonth, SalesOrderID)
	


5. What is the lifetime of a table variable scoped to?

    - [ ] A. 	batch
    - [ ] B. 	instance
    - [ ] C. 	connection
    - [ ] D. 	session
        


6. What is the main characteristic of table-valued functions?

    - [ ] A. 	They are defined as part of a table.
    - [ ] B. 	They accept a table as a parameter.
    - [ ] C. 	 They return a virtual table when run.
    - [ ] D. 	They can participate in transactions.
	
 	

	
7. You write a Transact-SQL script and want to store a rowset in a temporary object that will be automatically deleted. The script will reference the temporary rowset from mulitple queries in the same batch.

    Which two types of object can you use to achieve your goals?
    - [ ] A. 	View
    - [ ] B. 	Table-valued function
    - [ ] C. 	Common table expression
    - [ ] D. 	Temporary table
    - [ ] E. 	Derived table
    - [ ] F. 	Table variable
	
	
 	

8. You write a query that contains a derived table. The derived table should retrieve each product category ID and the count of products in those categories from the Production.Product table. The outer query then joins the derived table to the Production.ProductCategory table to display the product category names and their product counts.

    Your outer query looks like this:

    ```sql
    SELECT cat.Name AS Category, prd_cnts.ProductCount
    FROM Production.ProductCategory AS cat
    JOIN
    -- (derived table goes here ) --
    ON cat.ProductCategoryID = prd_cnts.CategoryID;
    ```

    Which two of the following derived table definitions can you use to complete the query?

    - [ ] A. 
        ```sql 	(SELECT ProductCategoryID AS CategoryID, COUNT(ProductID) AS ProductCount
        FROM Production.Product
        GROUP BY ProductCategoryID) AS prd_cnts
        ```
    - [ ] B. 
        ```sql	(SELECT ProductCategoryID, COUNT(ProductID)
        FROM Production.Product
        GROUP BY ProductCategoryID) AS prd_cnts(CategoryID, ProductCount)
        ```
    - [ ] C. 
        ```sql	(SELECT ProductCategoryID, COUNT(ProductID)
        FROM Production.Product AS prd_cnts (CategoryID, ProductCount)
        GROUP BY ProductCategoryID)
        ```
    - [ ] D. 
        ```sql	(SELECT ProductCategoryID AS CategoryID, COUNT(ProductID) AS ProductCount
        FROM Production.Product AS prd_cnts
        GROUP BY ProductCategoryID)
        ```
	

9. You write a Transact-SQL script and want to store a rowset in a temporary object that will be automatically deleted. The script will reference the temporary rowset from mulitple queries in the same batch.

    Which two types of object can you use to achieve your goals?
    - [ ] A. 	Temporary table
    - [ ] B. 	Table variable
    - [ ] C. 	Table-valued function
    - [ ] D. 	Derived table
    - [ ] E. 	Common table expression
    - [ ] F. 	View
	
	

10. How many different types of temporary tables are there?

    - [ ] A. 	3
    - [ ] B. 	2
    - [ ] C. 	4
    - [ ] D. 	1



<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 