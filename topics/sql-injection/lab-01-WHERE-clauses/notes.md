# SQL injection vulnerability in WHERE clause allowing retrieval of hidden data

- Topic: SQL Injection
- Difficulty: Apprentice
- Status: ✅ Solved
- Lab URL: https://portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data
- Tags: #SQLI

## Objectives
Display non-released products

## Summary
SQL injection to filter categories out and get unreleased items.

```sql
SELECT * FROM products WHERE category = 'Gifts' AND released = 1
```
## Payload


## Takeaways
Note that within SQL statements quotes are used to indicate a **string literal**. 
Without quotes it identifies `database objects` such as tables, columns, or even roles.

SQL expects the comparison to be written as `category = 'Gifts'`, with the text wrapped in single quotes. Without quotes, Gifts is no longer parsed as a string literal, so the database tries to interpret it as something else, typically an identifier such as a column name, which is why `category = Gifts` often fails.

```SQL
SELECT * FROM products WHERE category = 'Gifts' AND released = 1
SELECT * FROM products WHERE category = Gifts AND released = 1 -- Fails
```

### Resources

[Understanding 'Single' vs "Double" Quotation Marks in PostgreSQL - DEV Community](https://dev.to/appsmith/understanding-single-vs-double-quotation-marks-in-postgresql-dk0)






