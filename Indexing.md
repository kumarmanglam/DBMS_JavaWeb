
indexing is a database feature that enhances the speed of data retrieval operations on a database table. It ==involves creating a data structure, known as an index==, which is a ==copy of a portion of the data== in the table. This index allows the database management system (DBMS) to locate and access the rows in the table more quickly and efficiently, reducing the time it takes to execute queries.

Indexes are ==created on one or more columns of a table==, and they **work like an organized reference** to the actual data. When a query is executed that involves the indexed columns, the database engine can use the ==index to quickly locate the relevant rows==, rather t==han scanning the entire table.==

There are different types of indexes in SQL, including:

1. **Single-Column Index:** Created on a single column.
2. **Composite Index:** Created on multiple columns.
3. **Unique Index:** Ensures that the indexed columns ==do not contain duplicate values.==
4. **Clustered Index:** Determines the physical order of the data rows in the table, and the table itself is stored in the order of the clustered index.
5. **Non-Clustered Index:** Creates a separate structure for the index, and the data rows are not sorted in the order of the index.

**Single-Column Index:**
`CREATE INDEX idx_single_column ON your_table_name (column_name);
`
**Composite Index:**
`CREATE INDEX idx_composite ON your_table_name (column1, column2, ...);
`
**Unique Index:**
`CREATE UNIQUE INDEX idx_unique ON your_table_name (column_name);
`
**Clustered Index:**
`CREATE CLUSTERED INDEX idx_clustered ON your_table_name (column_name);`

**Non-Clustered Index:**
`CREATE NONCLUSTERED INDEX idx_non_clustered ON your_table_name (column_name);
`

