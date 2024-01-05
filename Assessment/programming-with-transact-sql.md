<a id="top" />

<br/>


[**Back to assessment**](./assessment.md) |   [**Back to main**](../README.md) 

## Programming with Transact-SQL


1. Which two conditions will cause the ELSE block to be run?

    - [ ] A. 	The predicate evaluates to FALSE.
    - [ ] B. 	The predicate evaluates to TRUE.
    - [ ] C. 	The predicate evaluates to MAYBE.
    - [ ] D. 	The predicate evaluates to UNKNOWN.


    |<br>

    <details>
    <summary>Show answer</summary>
    The ELSE keyword introduces another Transact-SQL statement that is executed when the IF condition is not satisfied: the Boolean expression returns FALSE.
    </details>

    <br>


	
2. What are the two keywords that define a block?

    - [ ] A. 	FINISH
    - [ ] B. 	END
    - [ ] C. 	START
    - [ ] D. 	BEGIN

    |<br>

    <details>
    <summary>Show answer</summary>
    BEGIN and END are control-of-flow language keywords.
    </details>

    <br>

	
3. How many times will the loop in the following code be executed?

    ```sql
    DECLARE @i int = 1;
    WHILE @i < 10
    BEGIN
    PRINT @i;
    END
    ```
    - [ ] A. 	None
    - [ ] B. 	Infinitely
    - [ ] C. 	9
    - [ ] D. 	10

    <br>

    <details>
    <summary>Show answer</summary>
    Infinitely
    </details>

    <br>


	
	
4. The organization you work for has a fiscal year that runs from July to June. For example, FY 2015 covers the period from July 1st 2014 to June 30th 2015. The Sales.SalesOrder table contains records of financial transactions, and the table includes an FY column to indicate in which fiscal year each transaction occurred.

    You need to write a script that returns all transaction data for the current fiscal year. Which two of the following scripts accomplishes this?

    - [ ] A. 
        ```sql	DECLARE @fy int;
        SET @fy = YEAR(GETDATE()) ;
        SELECT * FROM Sales.SalesOrder WHERE FY = @fy
        ```
    - [ ] B. 
        ```sql	DECLARE @fy int;
        IF MONTH(GETDATE()) < =6
        SET @fy = YEAR(GETDATE()) ;
        ELSE
        SET @fy = YEAR(GETDATE())+1;
        SELECT * FROM Sales.SalesOrder WHERE FY = @fy
        ```
    - [ ] C. 
        ```sql 
        SELECT * FROM Sales.SalesOrder WHERE FY = YEAR(GETDATE()) + 1; 
        ```
    - [ ] D. 
        ```sql	DECLARE @fy int = YEAR(GETDATE()) ;
        IF MONTH(GETDATE()) > 6
        SET @fy = @fy + 1;
        SELECT * FROM Sales.SalesOrder WHERE FY = @fy 
        ```
    - [ ] E. 
        ```sql	DECLARE @fy int;
        SET @fy = YEAR(GETDATE()) ;
        IF @fy > 6
        SET @fy = YEAR(GETDATE()) + 1;
        SELECT * FROM Sales.SalesOrder WHERE FY = @fy
        ```

        <br>

        <details>
        <summary>Show answer</summary>
        Answer B & D.
        </details>

        <br>



	
5. Which keyword is used to run a stored procedure?

    - [ ] A. 	EXEC
    - [ ] B. 	INVOKE
    - [ ] C. 	RUN
    - [ ] D. 	START

    <br>

    <details>
    <summary>Show answer</summary>
    EXEC
    </details>

    <br>


<br/>

> Source: 'Transact-SQL' published on Microsoft Virtual Academy

<br/>

------

[**Back to top**](#top) | [**Back to assessment**](./assessment.md) | [**Back to main**](../README.md) 