
## Syntax

```sql
-- Begin a new transaction
BEGIN TRANSACTION;

-- Insert a new record into the second_table
INSERT INTO second_table (id, fname, age) VALUES (9, 'John', 30);

-- Update an existing record in the second_table
UPDATE second_table SET age = 40 WHERE id = 8;

-- Commit the transaction to save the changes
COMMIT;
```


### RollBack Syntax'

```sql
-- Begin a new transaction
BEGIN TRANSACTION;

-- Make some changes within the transaction
INSERT INTO second_table (id, fname, age) VALUES (9, 'John', 30);

-- Update an existing record in the second_table
UPDATE second_table SET age = 40 WHERE id = 8;

-- Roll back the transaction to discard the changes
ROLLBACK;
```

