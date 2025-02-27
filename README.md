# SQL

📌 **Tables Included**
1. customers Table
Stores customer details such as:

```sql
Name (VARCHAR) – First name of the customer
Surname (VARCHAR) – Last name of the customer
Age (INT) – Age of the customer
```

2. AGENTS Table
Stores agent details such as:
```sql
AGENT_CODE (VARCHAR) – Unique identifier (Primary Key)
AGENT_NAME (VARCHAR) – Name of the agent
WORKING_AREA (VARCHAR) – Location where the agent operates
COMMISSION (FLOAT) – Commission percentage
PHONE_NO (VARCHAR) – Contact number
COUNTRY (VARCHAR) – Country of operation
```

📌 **SQL Operations**

🟢 **Creating Tables**
```sql

CREATE TABLE customers (
  Name VARCHAR,
  Surname VARCHAR,
  Age INT
);
```
```sql
CREATE TABLE AGENTS (
  AGENT_CODE VARCHAR NOT NULL PRIMARY KEY,
  AGENT_NAME VARCHAR,
  WORKING_AREA VARCHAR,
  COMMISSION FLOAT,
  PHONE_NO VARCHAR,
  COUNTRY VARCHAR
);
```

🟢 **Inserting Data**
```sql
INSERT INTO customers VALUES ('Asim', 'Pardeshi', 25);
INSERT INTO AGENTS VALUES ('A001', 'Asim', 'Hyderabad', '0.15', '+91 789456123', 'India');
```

🟢 **Selecting Data**
```sql
SELECT * FROM customers;
SELECT * FROM AGENTS WHERE COUNTRY = 'India';
SELECT * FROM AGENTS WHERE agent_name LIKE 'Ra%';
```
🟢 **Sorting Data**
```sql
SELECT * FROM AGENTS ORDER BY COMMISSION DESC;
```
🟢 **Updating Records**
```sql
UPDATE AGENTS SET agent_name = 'Asim', COUNTRY = 'Germany' WHERE agent_code = 'A006';
```
🟢 **Deleting Records**
```sql
DELETE FROM AGENTS WHERE agent_code = 'A006';
```

📌 **How to Use**

*Clone the repository:*

*Git clone* https://github.com/Analyzewithasim/SQL_Queries.git

**Import the SQL script into your database management system (MySQL, PostgreSQL, etc.).**

**Execute the queries in the order provided.**
