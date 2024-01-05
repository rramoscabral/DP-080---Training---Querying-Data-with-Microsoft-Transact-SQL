<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## 3 - Querying Multiple Tables with Joins



1. The HumanResources.Employee table contains the following columns:
* EmployeeID (a unique identifier for each employee)
* FirstName (the employee's first name)
* LastName (the employee's last name)
* ManagerID (the EmployeeID of the employee's manager)
You want to write a query that returns FirstName and LastName for each employee as well as FirstName and LastName for the employee’s manager.
Which type of join should you use?
- [ ] A. 	A cross join
- [ ] B. 	An equi-join
- [ ] C. 	An inner join
  [ ] D. 	A self-join

	
2. What are the two standards used to define the JOIN syntax?
- [ ] A. 	ANSI SQL-99
- [ ] B. 	ANSI SQL-80
- [ ] C. 	ANSI SQL-89
- [ ] D. 	ANSI SQL-92
	
	

3. What does a Cartesian product consist of?
- [ ] A. 	all unmatched values in the first table
- [ ] B. 	every possible combination of rows
- [ ] C. 	all rows in the first table that match a second table
- [ ] D. 	all rows from both tables in one result
	

4. You write a query to generate test data. You want to generate a list of sales orders in which every customer has ordered every product.
What kind of join should you use?
- [ ] A. 	An equi-join
- [ ] B. 	An inner join
- [ ] C. 	A self-join
- [ ] D. 	A full outer join
- [ ] E. 	A cross join
	

5. You write a query that returns a list of all sales employees that have taken sales orders. Employees who have not taken sales orders should not be included in the results.
  ```sql
  Select the appropriate join type to complete the following query.
  SELECT e.FirstName, e.LastName, s.Amount
  FROM HumanResources.Employee AS e
  ________________ Sales.SalesOrder AS s ON s.SalesPersonID = e.EmployeeID;
  ```
- [ ] A. 	RIGHT OUTER JOIN
- [ ] B. 	LEFT OUTER JOIN
- [ ] C. 	CROSS JOIN
- [ ] D. 	INNER JOIN
 
 

6. When a column is selected in a join where the value cannot be determined from the source table, what value is returned?
- [ ] A. 	the last value from the source table
- [ ] B. 	NULL
- [ ] C. 	the first value from the source table
- [ ] D. 	0



<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 