
<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Grouping Sets and Pivoting Data


1. Which type of grouping set does a ROLLUP apply to?
- [ ] A. 	a grouping that forms a hierarchy
- [ ] B. 	an ordered grouping
- [ ] C. 	an unfiltered grouping
- [ ] D. 	a common table expression
	
	
 	

2. You write a query to summarize sales revenue by country/region and state/province. The results from your query should match the following rowset structure:

    | CountryRegion  		|	StateProvince    	|	Revenue |
    |  --- | --- | --- |
    |NULL				|	NULL				|	Total Revenue |
    | Country/Region 1	|	NULL				|	Subtotal for Country/Region 1 |
    | Country/Region 1	|	State/Province A	|	Subtotal for State/Province A in Country/Region 1  |
    | Country/Region 1	|	State/Province B	|	Subtotal for State/Province B in Country/Region 1 |
    | Country/Region 2	|	NULL				|	Subtotal for Country/Region 2 |
    | Country/Region 2	|	State/Province C	|	Subtotal for State/Province C in Country/Region 2 |
    | Country/Region 2	|	State/Province D	|	Subtotal for State/Province D in Country/Region 2 |

You write the following Transact-SQL code:

    ```sql
    SELECT c.CountryRegion, c.StateProvince, SUM(o.TotalDue) AS Revenue
    FROM Sales.Customers AS c
    JOIN Sales.SalesOrder AS o ON o.CustomerID = c.CustomerID
    -- GROUP BY clause goes here
    ORDER BY c.CountryRegion, c.StateProvince;

    ```

Which two of the following GROUP BY clauses will produce the required results?

- [ ] A. 	```sql GROUPING SETS(a.CountryRegion, a.StateProvince)) ```
- [ ] B. 	```sql GROUPING SETS(a.CountryRegion, (a.CountryRegion, a.StateProvince),()) ```
- [ ] C. 	```sql GROUP BY CUBE ```
- [ ] D. 	```sql GROUP BY ROLLUP ```
- [ ] E. 	```sql GROUPING SETS(a.CountryRegion, a.StateProvince),()) ```
- [ ] F. 	```sql GROUP BY c.CountryRegion, c.StateProvince ```

	
3. The Sales.SalesOrder header contains a CustomerID column, an OrderDate column, and a SalesAmount column. You want to query this table and generate a rowset that shows the total revenue per customer for each month using the following format:

| CustomerID	|	1		|	2		|	3		|	4		|	5		|	6		|	…  | 12 | 
|  ----         | ---        | ---      | ----      | ----      | ----      | ----      | ---- | ----     | 
| Customer 1	| January Revenue | February Revenue	| March Revenue	| April	Revenue	| MayRevenue | June	Revenue	| …  | December Revenue |
| Customer 2	| January Revenue	| February Revenue	| March Revenue	| April	Revenue	| May Revenue  | JuneRevenue	| …  | December Revenue |		
|	...		    | 	...		        |	...		        |	...		    |	...		   |	...		    |	...		    |	... |	... | 

You write the following Transact-SQL query:

    ```sql
    SELECT * FROM
    (SELECT CustomerID, SalesAmount, MONTH(OrderDate) AS OrderMonth
    FROM Sales.SalesOrder) AS SalesByMonth
    ________________________________________________________________
    ORDER BY CustomerID;
    ```
 
Select the appropriate code to complete the query.

- [ ] A. 	```sql UNPIVOT (SalesAmount FOR OrderMonth IN ([1],[2],[3],[4],[5],[6],[7],[8],[9],[10],[11],[12])) AS unpvt') ```
- [ ] B. 	```sql GROUP BY CUBE ```
- [ ] C. 	```sql PIVOT(SUM(SalesAmount) FOR OrderMonth IN([1],[2],[3],[4],[5],[6],[7],[8],[9],[10],[11],[12])) AS pvt ```
- [ ] D. 	```sql GROUP BY CustomerID ```
- [ ] E. 	```sql GROUP BY GROUPING SETS (MONTH(OrderDate)) ```

	
	
	
4. What is the syntax for a grouping set that applies to all rows?
- [ ] A. 	<>
- [ ] B. 	_
- [ ] C. 	()
- [ ] D. 	%


5. You write a query that uses a GROUP BY clause with a GROUPING SETS expression to summarize sales revenue by state, city, and store. The results contain many NULL values and it is difficult to determine which revenue totals are generated by which groupings.
What should you do to resolve this problem?
- [ ] A. 	Use the ISNULL function in the Revenue column to display 0.00 if the figure is NULL.
- [ ] B. 	Create a new column that uses the GROUPING_ID column to determine which groupings are being used for each row.
- [ ] C. 	Create a new column that uses the ISNULL function to display the text 'Total' if the Revenue column is NULL.
- [ ] D. 	Add a WHERE clause to the query that filters the results using an IS NOT NULL predicate on the aggregation expression for the Revenue column.
	

6. Which function can assist in identifying to which grouping a particular row applies?
- [ ] A. 	GROUPING_NAME
- [ ] B. 	GROUPING_COLUMN
- [ ] C. 	GROUPING_ID
- [ ] D. 	GROUPING_STATE
	
7. What do grouping sets allow you to do?
- [ ] A. 	have multiple levels of grouping
- [ ] B. 	group on more than one table
- [ ] C. 	filter groups based on a predicate
- [ ] D. 	order a group
	

8. What does pivoting data do?
- [ ] A. 	It defines an output format that is readable by Microsoft Excel.
- [ ] B. 	It groups based on numeric distribution of the data.
- [ ] C. 	It arranges the results in order of the group size.
- [ ] D. 	It changes a row-based result to a column-based result.



<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 