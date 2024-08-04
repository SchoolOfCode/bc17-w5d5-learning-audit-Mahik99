## Environment variables

- Contain sensitive data like API keys, database connection strings, and configuration settings.
- They're useful for setting different configurations for different environments (development, testing, production).
- Can create a .env file which contains key-value pairs for example: `PORT = "3000"`
- You shouldn't hardcode sensitive information for security purposes and you should never commit your .env file, list it under gitignore.

## pg Package in Node.js

- The purpose of a pg package is that it's a PostgreSQL client for Node.js. It allows you to interact with a PostgreSQL database.
- You need to intsall the package, import it, connect to the database and then query the database.
- Pooling is useful to manage multiple database connections efficiently and when making a query you should always use parameterized queries to prevent SQL injection attacks. SQL Injection is a security vulnerability that allows an attacker to interfere with the queries that an application makes to its database. It can lead to unauthorized access, data theft, or data manipulation.
