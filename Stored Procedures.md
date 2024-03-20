
Syntax 
```sql
CREATE PROCEDURE _procedure_name_  
AS  
_sql_statement_  
GO;
```

Execute syntax
```sql
EXEC _procedure_name_;
```

## First Example

```sql
CREATE PROCEDURE SelectAllCustomers  
AS  
SELECT * FROM Customers  
GO;

EXEC SelectAllCustomers;
```


## Second Example

```sql
CREATE PROCEDURE SelectAllCustomers @City nvarchar(30)  
AS  
SELECT * FROM Customers WHERE City = @City  
GO;

EXEC SelectAllCustomers @City = 'London';
```

## Third Example

```sql
CREATE PROCEDURE SelectAllCustomers @City nvarchar(30), @PostalCode nvarchar(10)  
AS  
SELECT * FROM Customers WHERE City = @City AND PostalCode = @PostalCode  
GO;

EXEC SelectAllCustomers @City = 'London', @PostalCode = 'WA1 1DP';
```

