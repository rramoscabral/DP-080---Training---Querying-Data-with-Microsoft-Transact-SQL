<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Using Subqueries and APPLY


1. Which two types of results can subqueries return?
- [ ] A. 	inverted
- [ ] B. 	pivot-table
- [ ] C. 	multi-valued
- [ ] D. 	scalar
	

2. Select the appropriate subquery WHERE predicate to complete the following query so that the OrderCount column contains a count of the orders placed by each customer.
    ```sql
    SELECT CustomerID, CompanyName,
    (SELECT COUNT(*) FROM Sales.SalesOrder AS o
    WHERE _____________________) AS OrderCount

    FROM Sales.Customer AS c;
    ```

- [ ] A. 	o.CustomerID = c.CustomerID
- [ ] B. 	o.SalesOrderID = c.SalesOrderID
- [ ] C. - [ ] C.CustomerID IN (SELECT CustomerID FROM Sales.SalesOrder AS o)
- [ ] D. 	SalesOrderID = CustomerID
	

3. What is one of the categories of subqueries?
- [ ] A. 	self-contained
- [ ] B. 	justified
- [ ] C. 	optimized
- [ ] D. 	interdependent
	
	
 	

4. What is an OUTER APPLY query similar to?
- [ ] A. 	CROSS JOIN
- [ ] B. 	FULL JOIN
- [ ] C. 	INNER JOIN
- [ ] D. 	LEFT OUTER JOIN
	
	

5. What is a CROSS APPLY query similar to?
- [ ] A. 	CROSS JOIN
- [ ] B. 	LEFT OUTER JOIN
- [ ] C. 	FULL JOIN
- [ ] D. 	INNER JOIN

6. Your database contains a table-valued function named dbo.fn_CurrentYearOrders that returns the SalesOrderID, OrderDate, and SalesAmount for each order placed in the current year by the customer specified in a CustomerID parameter.
You write the following query to return the CompanyName column from the Sales.Customer table and the sum of revenue for each customer in the current year, and you plan to use the dbo.fn_CurrentYearOrders function to accomplish this. Only data for customers who have placed orders in the current year should be included in the results.
    ```sql
    SELECT c.CompanyName, SUM(cyo.SalesAmount) AS Revenue
    FROM SalesLT.Customer AS c
    _____________________________________________________
    GROUP BY c.CompanyName;
    ```
- [ ] A. 	CROSS JOIN dbo.CurrentYearOrders(c.CustomerID) AS cyo
- [ ] B. 	CROSS APPLY dbo.CurrentYearOrders(c.CustomerID) AS cyo
- [ ] C. 	OUTER JOIN dbo.CurrentYearOrders(c.CustomerID) AS cyo
- [ ] D. 	OUTER APPLY dbo.CurrentYearOrders(c.CustomerID) AS cyo
 
 
 

7. The Sales.SalesOrder table contains details of sales orders made by customers. Customers are identified by a unique CustomerID column, which is the primary key of the Sales.Customer table. The Sales.Customer table also contains a City column that contains the name of the city in which the customer lives.
Select the appropriate WHERE clause for the following query so that it returns sales order data for all customers who live in New York:
    ```sql
    SELECT SalesOrderID, OrderDate, Amount
    FROM Sales.SalesOrder
    ______________________
    ```
- [ ] A. 	WHERE City = 'New York';
- [ ] B. 	WHERE CustomerID = (SELECT CustomerID FROM Sales.Customer WHERE City = 'New York');
- [ ] C. 	WHERE CustomerID IN (SELECT CustomerID FROM Sales.Customer WHERE City = 'New York');
- [ ] D. 	WHERE CustomerID IN (SELECT City FROM Sales.Customer WHERE City = 'New York');



<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 