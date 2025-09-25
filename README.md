# SQL Server Hints

A collection of useful SQL Server utilities and stored procedures.

## Contents

### Stored Procedures

- `SearchAllTables.sql` - Searches for a specific string across all tables and columns in a SQL Server database

## SearchAllTables Stored Procedure

This stored procedure allows you to search for a specific string value across all tables and text-based columns in your SQL Server database.

### Features

- Searches through all user tables (excludes system tables)
- Only searches text-based columns (char, varchar, nchar, nvarchar)
- Returns the table/column name and matching value for each result
- Uses NOLOCK hints for better performance

### Usage

```sql
EXEC SearchAllTables @SearchStr = 'your_search_term'
```

### Parameters

- `@SearchStr` - The string to search for across all tables

### Author

Originally written by Narayana Vyas Kondreddi
Compatible with SQL Server 7.0 and later versions
