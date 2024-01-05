<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Using Functions and Aggregating Data

1. Which kind of function is RANK?
- [ ] A. 	window
- [ ] B. 	aggregate
- [ ] C. 	logical
- [ ] D. 	numeric

	
2. The Sales.SalesOrderDetail table contains a row for each line item that has been ordered. Each row includes the following columns:
* ProductID: The unique ID of the product that was ordered.
* Quantity: How many units of the product were ordered.
* UnitPrice: The price per unit charged for the product.
You run the following query:
    ```sql
    SELECT COUNT(ProductID) AS ProductIDCount, COUNT(Quantity) AS QuantityCount, SUM(UnitPrice) AS PriceSum
    FROM Sales.SalesOrderDetail;
    ```
What does the value returned by the query for the QuantityCount column represent?
 - [ ] A. 	The number of distinct products that have been ordered
 - [ ] B. 	The total number of product units that have been ordered
 - [ ] C. 	The number of rows containing a Quantity value
 - [ ] D. 	The number of orders


3. Which clause is required in order for an aggregate query to return more than one value?
- [ ] A. 	GROUP BY
- [ ] B. 	ORDER BY
- [ ] C. 	WHERE
- [ ] D. 	DISTINCT
	

4. You write a query that counts customers. The results should show the count of customers in each city in every state.
Select the code required to complete the query:
    ```sql
    SELECT COUNT(CustomerID) AS CustomerCount, City AS CustomerCity, State AS CustomerState
    FROM Sales.Customer
    ______________________ ;
    ```
- [ ] A. 	GROUP BY CustomerState, CustomerCity
- [ ] B. 	GROUP BY City, State
- [ ] C. 	GROUP BY CustomerCount
- [ ] D. 	GROUP BY State, City, CustomerID
- [ ] E. 	GROUP BY State, City
	

5. Which should you use to filter the aggregated values in an aggregate query?
- [ ] A. 	IN
- [ ] B. 	WHERE
- [ ] C. 	GROUP BY
- [ ] D. 	HAVING
	
	
	

6. What value will the following query return in the OrderStatus column for rows with a Status value of 2?
    ```sql
    SELECT OrderNumber, CHOOSE(Status, 'Ordered', 'Shipped', 'Delivered') AS OrderStatus
    FROM Sales.SalesOrderHeader
    ```
- [ ] A. 	NULL
- [ ] B. 	Delivered
- [ ] C. 	Ordered
- [ ] D. 	Shipped
	
	
	
<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 