<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Using Set Operators


1. INTERSECT is similar to what type of join?
    - [ ] A. 	inner
    - [ ] B. 	cross
    - [ ] C. 	outer
    - [ ] D. 	full
        

2. The Sales.SalesOrderDetail table contains a row for every line item sold, and includes a ProductID column to identify the product that was ordered.
    The Production.Product table contains a row for every product, and includes a Discontinued column where the value 1 indicates that the product has been discontinued.

    What result does the following query return?

    ```sql
    SELECT DISTINCT ProductID
    FROM Sales.SalesOrderDetail
    EXCEPT
    SELECT ProductID
    FROM Production.Product
    WHERE Discontinued = 1;
    ```

    - [ ] A. 	All products that have been sold and all products that have been discontinued.
    - [ ] B. 	All non-discontinued products that have been sold.
    - [ ] C. 	All non-discontinued products that have never been sold.
    - [ ] D. 	All discontinued products that have been sold.
	
    <br>

    <details>
    <summary>Show answer</summary>
    All non-discontinued products that have been sold. 
    </details>

    <br>


3. You write a query that returns the set of products that are available in the color 'Red' or the size 'XL' by combining the results of two queries. Any products that are available in both red and size XL should be included as a duplicate row in the resultset.

    Select the appropriate missing keyword.

    ```sql
    SELECT ProductID, Name, Color, Size
    FROM Production.Product
    WHERE Color = 'Red'
    __________
    SELECT ProductID, Name, Color, Size
    FROM Production.Product
    WHERE Size = 'XL'
    ORDER BY ProductID;
    ```

    - [ ] A. 	UNION
    - [ ] B. 	UNION ALL
    - [ ] C. 	EXCEPT
    - [ ] D. 	INTERSECT
	

    <br>

    <details>
    <summary>Show answer</summary>
    UNION ALL
    </details>

    <br>
	

4. You write the following Transact-SQL query that returns the CustomerName, StreetAddress, City, and PostalCode columns from the Sales.BillingAddress table:

    ```sql
    SELECT CustomerName, StreetAddress, City, PostalCode
    FROM Sales.BillingAddress;
    ```

    You have also written the following query to retrieve the same fields from the Sales.ShippingAddress table:

    ```sql
    SELECT CustomerName, StreetAddress, City, PostalCode
    FROM Sales.ShippingAddress;
    ```

    What set operator can you use to combine the results of these queries and return only rows for customers whose billing address is the same as their shipping address?
    - [ ] A. 	UNION ALL
    - [ ] B. 	UNION
    - [ ] C. 	INTERSECT
    - [ ] D. 	EXCEPT
	

    <br>

    <details>
    <summary>Show answer</summary>
    INTERSECT
    </details>

    <br>


5. What does an EXCEPT query return?

    - [ ] A. 	all distinct rows that appear in the first result set but not in the second result set
    - [ ] B. 	all rows that appear in the first result set but not in the second result set
    - [ ] C. 	all distinct rows that appear in the second result set but not in the first result set
    - [ ] D. 	all rows that appear in the second result set but not in the first result set


<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>
------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 