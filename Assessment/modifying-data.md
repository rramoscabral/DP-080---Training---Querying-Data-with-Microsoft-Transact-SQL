<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Modifying Data


1. You use an INSERT statement to insert specific values into a table.

    For which of the following columns do you not need to provide values?
    - [ ] A. 	Non-Nullable columns that have a default value
    - [ ] B. 	Nullable columns that have no default value
    - [ ] C. 	IDENTITY columns
    - [ ] D. 	Nullable columns that have a default value
    - [ ] E. 	Non-Nullable columns that have no default value


	

2. You need to determine the most recently inserted IDENTITY column in a specific table.

    Which statement should you use?
    - [ ] A. 	``` SELECT IDENT_CURRENT('table_name') ```
    - [ ] B. 	``` SELECT SCOPE_IDENTITY() ```
    - [ ] C. 	``` SELECT NEXT VALUE FOR table_name ```
    - [ ] D. 	``` SELECT @@IDENTITY ```
	

    <br>

    <details>
    <summary>Show answer</summary>
    SELECT IDENT_CURRENT('table_name') 
    </details>

    <br>


3. You want to load new product catalog data from a staging table into the Production.Products table. Products are uniquely identified by a ProductID value. You want to apply the following logic:

    * If the ProductID exists in the staging table but not the Production.Products table, insert a new row into the Production.Products table.
    * If the ProductID exists in the Production.Products table but not the staging table, update the row for that product in the Production.Products table to set its Discontinued column to 1.
    * If the ProductID exists in both tables, update the row in the Production.Products table and set all column values to match the values in the staging table.

    What type of statement should you use?
    - [ ] A. 	A SELECT INTO statement
    - [ ] B. 	An UPDATE statement with a FROM clause
    - [ ] C. 	An INSERT statement with a FROM clause
    - [ ] D. 	A MERGE statement

    <br>

    <details>
    <summary>Show answer</summary>
    A MERGE statement
    </details>

    <br>


4. What does the MERGE statement do?

    - [ ] A. 	It inserts rows that don’t match the predicate, and updates rows that do match.
    - [ ] B. 	It deletes rows that don’t match the predicate, and updates rows that do match.
    - [ ] C. 	It updates if there is a match, and runs a statement if there is not a match.
    - [ ] D. 	It runs one statement if there is a match, and runs another statement if there is not a match. 

    <br>

    <details>
    <summary>Show answer</summary>
    The MERGE statement allows you to check a set of data for a condition, and UPDATE a record if it exists or INSERT a record if it doesn't exist.
    </details>

    <br>

5. What are two ways to insert data from a query or stored procedure?

    - [ ] A. 	INSERT…SELECT
    - [ ] B. 	INSERT…MANY
    - [ ] C. 	INSERT…EXEC
    - [ ] D. 	INSERT…SOURCE
	

6. What is the first version of SQL Server that supports sequences for identifiers?

    - [ ] A. 	2008 R2
    - [ ] B. 	2008
    - [ ] C. 	2014
    - [ ] D. 	2012

    <br>

    <details>
    <summary>Show answer</summary>
    Sequence objects are used to sequentially generate numeric values. They were introduced in SQL Server 2012. 
    </details>

    <br>

	

7. Which function is used to find the last identity value for a specific table?

    - [ ] A. 	LAST_IDENT
    - [ ] B. 	ROW_TIP
    - [ ] C. 	TABLE_MAX
    - [ ] D. 	IDENT_CURRENT


    <br>

    <details>
    <summary>Show answer</summary>
    IDENT_CURRENT returns the last identity value generated for a specific table in any session and any scope.
    </details>

    <br>


<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 