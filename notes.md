<a id="top" />

[**Back to main**](./README.md) 

<br/>

# Notes 


# SQL Standart

The first SQL standard was released by the American National Standards Institute (ANSI) in 1986.
Is held by ANSI and the International Standards Organization (ISO) as the ISO/IEC 9075 standard.

- 1986, ANSI X3.135-1986, ISO/IEC 9075:1986, SQL-86
    * [This standard is available on archive.org](https://archive.org/details/federalinformati127nati/)
- 1997, ISO/IEC 9075:1987 SQL: 1987 
    * Transactions
    * Create
    * Read
    * Update
    * Delete 
- 1989, ANSI ISO/IEC 9075:1992, SQL-92 (SQL2)
    * Added foreign and primary key constraints. 
- 1992, ISO/IEC 9075:1992, SQL:1992
    * Subqueries in place of named tables.
    * Internationalization.
    * Embedded SQL in programming languages 
- 1999, ISO/IEC 9075:1999, SQL:1999 (SQL3)
    * Arrays collection types that contains an ordered set of elements.
- 2003, ISO/IEC 9075:2003, SQL:2003
    * Multiset collection types that stores an unordered set of elements.
    * Data types
    * Identity columns, and  generated columns 
- 2008, ISO/IEC 9075:2008, SQL:2008
- 2011, ISO/IEC 9075:2011, SQL:2011
    * New features
    * Database languages SQL
- 2016, ISO/IEC 9075:2016, SQL:2016
    * Support for JSON data
    * Polymorphic table functions (PTF)
    * Regular expressions 
    * Trigonometric and logarithmic functions
    * Framework (SQL/Framework)
    * Persistent Stored Modules (SQL/PSM)
    * Information technology Database languages SQL
- 2019, ISO/IEC 9075:2019, SQL:2019
    * Multidimensional arrays (MDA)
- 2023, ISO/IEC 9075:2023, SQL:2023
    - Foundation (SQL/Foundation)
    - Call Level Interface (SQL/CLI)
    - Object language bindings (SQL/OLB)
    - XML-Related Specifications (SQL/XML)


<br>

# SQL Schema

A schema is a collection of database objects.

* `[server_name.][database_name.][schema_name.]object_name`

Every object has a unique name.

Every object belongs to one schema.

So, each schema will have its own tables, views, relationships and other objects and for the user who accesses them they will be, in practice, like separate databases.

The following schemas cannot be dropped deleted because they are built-in logical schemas:
* dbo (default schema of every database)
* guest
* sys (reserved for system objects)
* INFORMATION_SCHEMA (reserved for system objects)

Documentation:
- [OBJECT_SCHEMA_NAME (Transact-SQL)](https://learn.microsoft.com/en-us/sql/t-sql/functions/object-schema-name-transact-sql)
- [Create a database schema](https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/create-a-database-schema)
- [Ownership and user-schema separation in SQL Server](https://learn.microsoft.com/en-us/sql/relational-databases/security/authentication-access/ownership-and-user-schema-separation)


<br/>

[**Back to main**](./README.md) 