<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Querying Tables with SELECT

1. 	You write a query to return the Name and Price of all products that have a Category value of 2 or 4. You have used the following SELECT clause:

    ```sql
    SELECT Name, Price
    FROM Production.Product
    ```

    Which two of the following WHERE clauses can you use to complete the query correctly?
    - [ ] A. 	``` WHERE Category IN (2, 4); ```
    - [ ] B. 	``` WHERE CATEGORY = 2 AND Category = 4; ```
    - [ ] C. 	``` WHERE Category BETWEEN 2 AND 4; ```
    - [ ] D. 	``` WHERE Category = 2 OR Category = 4; ```
    - [ ] E. 	``` WHERE Category = 2 OR 4; ```


2.  Which character acts as a wildcard when used in the LIKE predicate?

    - [ ] A. 	``` & ```
    - [ ] B. 	``` + ```
    - [ ] C. 	``` * ```
    - [ ] D. 	``` _ ```

    <br>

    <details>
    <summary>Show answer</summary>
    _ (underscore)
    </details>

    <br>
	
3. 	Which character in a LIKE statement matches exactly one alpha-numeric character?

    - [ ] A. 	``` _ ```
    - [ ] B. 	``` & ```
    - [ ] C. 	``` + ```
    - [ ] D. 	``` * ```


    <br>

    <details>
    <summary>Show answer</summary>
    _ (underscore) Any single character
    </details>

    <br>



4. 	Which T-SQL keyword should you use to remove duplicate rows?

    - [ ] A. 	``` DISTINCT ```
    - [ ] B. 	``` UNION ALL ```
    - [ ] C. 	``` WHERE ```
    - [ ] D. 	``` JOIN ```

    <br>

    <details>
    <summary>Show answer</summary>
    DISTINCT
    </details>

    <br>


5. 	Which SQL keyword matches a value in a collection when used in a predicate?

    - [ ] A. 	``` IN ```
    - [ ] B. 	``` LIKE ```
    - [ ] C. 	``` OR ```
    - [ ] D. 	``` BETWEEN ```

    <br>

    <details>
    <summary>Show answer</summary>
    IN (Transact-SQL) determines whether a specified value matches any value in a subquery or a list.
    </details>

    <br>
	
6. 	You write a Transact-SQL query to list the available sizes for products. Each individual size should be listed only once.

    Which query should you use?
    - [ ] A. 	``` SELECT TOP 1 Size FROM Production.Product ORDER BY Size; ```
    - [ ] B. 	``` SELECT DISTINCT Size FROM Production.Product; ```
    - [ ] C. 	``` SELECT ALL Size FROM Production.Product; ```
    - [ ] D. 	``` SELECT Size FROM Production.Product; ```

    <br>

    <details>
    <summary>Show answer</summary>
    SELECT DISTINCT Size FROM Production.Product; 
    </details>

    <br>



7. 	You write a Transact-SQL query to return the SalesOrderID, OrderDate, and Amount fields for the first 10 sales orders in order of SalesOrderID.  Which three of the following queries returns the required results?

    - [ ] A.
        ```sql
        SELECT SalesOrderID, OrderDate, Amount
        FROM Sales.SalesOrder
        ORDER BY SalesOrderID
        OFFSET 0 ROW FETCH NEXT 10 ROW ONLY;
        ```
    - [ ] B.
        ```sql
        SELECT TOP 10 SalesOrderID, OrderDate, Amount
        FROM Sales.SalesOrder
        ORDER BY SalesOrderID;
        ```
    - [ ] C.
        ```sql 	
        SELECT TOP 10 PERCENT SalesOrderID, OrderDate, Amount
        FROM Sales.SalesOrder
        ORDER BY SalesOrderID;
        ```
    - [ ] D.
        ```sql
        SELECT SalesOrderID, OrderDate, Amount
        FROM Sales.SalesOrder
        ORDER BY SalesOrderID ASC;
        ```
    - [ ] E. 
        ```sql SELECT SalesOrderID, OrderDate, Amount
        FROM Sales.SalesOrder
        ORDER BY SalesOrderID
        OFFSET 0 ROWS FETCH FIRST 10 ROWS ONLY;
        ```

	
8. 	What are two ways that the results of a sorted query can be limited?

    - [ ] A. 	``` BOTTOM N PERCENT ```
    - [ ] B. 	``` TOP N PERCENT ```
    - [ ] C. 	``` TOP N ```
    - [ ] D. 	``` BOTTOM N ```




<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 