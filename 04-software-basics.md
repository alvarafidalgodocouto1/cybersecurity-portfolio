# Pre Security — Software Basics

## Module overview

This module introduces data representation and encoding, basic programming examples, and database/SQL concepts.

## 1. Data representation

Computers represent data using binary digits. A byte is typically eight bits. Text, numbers, images, and audio are represented through defined formats.

Do not confuse:
- **Encoding:** changes representation into a defined format.
- **Encryption:** transforms data using a key to protect confidentiality.
- **Hashing:** produces a digest used for integrity checks and other applications.
- **Compression:** reduces the size of data.

These serve different purposes.

## 2. Python

Python is a general-purpose language used for automation, data processing, scripting, and security tooling.

Example:

```python
status_code = 200

if status_code == 200:
    print("Request succeeded")
```

This is an illustrative example showing a conditional; it is not a record of a specific lab result.

## 3. JavaScript

JavaScript is widely used to add behaviour to web pages and is also used on servers. Understanding basic syntax helps explain client-side application behaviour and web security issues.

## 4. SQL and databases

Relational databases organise data in tables. SQL retrieves and modifies records.

Example read-only query:

```sql
SELECT username, last_login
FROM users
WHERE last_login IS NOT NULL;
```

Actual table and column names depend on the database schema.

Security concerns include access control, least privilege, input validation, safe query construction, and avoiding excessive database permissions.

## Security relevance

Security analysts may parse logs, automate repetitive tasks, query structured data, or investigate how an application handles input. Understanding the difference between encoding, encryption, and hashing prevents incorrect security assumptions.

## Key takeaways

- Data must be represented in formats software can interpret.
- Encoding, encryption, hashing, and compression are different concepts.
- Python and JavaScript support different types of automation and application behaviour.
- SQL is used to work with relational data; unsafe query construction can create vulnerabilities.

## Rooms covered by this module

- Data Representation
- Data Encoding
- Python: Simple Demo
- JavaScript: Simple Demo
- Database SQL Basics

## Official reference

[TryHackMe Pre Security](https://tryhackme.com/path/outline/presecurity)
