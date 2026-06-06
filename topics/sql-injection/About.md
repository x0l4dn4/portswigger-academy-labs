# What is SQL injection

**SQL injection** (**SQLi**) is a type of vulnerability in which an attacker can inject malicious SQL statements, also known as **payloads**, enabling the user to perform other unintended SQL queries directly against the database.

> It occurs when *user input* is inserted into queries and subsequently passed to a database for execution.

## Process

First, the attacker has to **inject code outside the expected user input limits**. 

In the most basic case, this is done by injecting a single quote (') to escape the limits of user input and inject data directly into the SQL query.

## Resources

[What is SQL Injection? Tutorial & Examples | Web Security Academy](https://portswigger.net/web-security/sql-injection)

[SQL Injection | OWASP Foundation](https://owasp.org/www-community/attacks/SQL_Injection)

