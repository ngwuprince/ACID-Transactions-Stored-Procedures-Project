**Project Overview**

This project focuses on the implementation of ACID (Atomicity, Consistency, Isolation, Durability) transactions and the creation of stored procedures within a relational database environment. The goal is to ensure that complex transactions either complete successfully in their entirety or have no impact on the database, maintaining data integrity and consistency.

**Key Concepts:**
ACID Transactions: A set of properties ensuring that database transactions are processed reliably. If any part of the transaction fails, the entire transaction is rolled back to its previous state.
Stored Procedures: Predefined SQL code that can be saved and reused. They help in executing a series of tasks, managing transactions, and maintaining the integrity of data operations.

**Project Objectives**

**Ensure Data Consistency and Reliability**: Implement ACID transactions to safeguard data integrity during multiple, interdependent database operations.

**Develop and Implement Stored Procedures**: Create stored procedures to handle complex transaction logic, enabling automated and repeatable database operations.

**Optimize Server Queries and Transaction Control**: Utilize Transaction Control Language (TCL) commands such as COMMIT and ROLLBACK to manage transaction flows effectively.

**Case Studies**
1. TRANSACTION_ROSE Stored Procedure

Scenario: Buying a pair of Boots for Rose from ShoeShop.

**Operations:**
- Update Rose’s bank balance.
- Update ShoeShop’s bank balance.
- Update the inventory of Boots at ShoeShop.
- Attempt to purchase Trainers for Rose.

**Outcome:**
The transaction was rolled back due to insufficient funds when attempting to buy Trainers, demonstrating the effectiveness of ACID transactions in preventing partial data updates.

2. TRANSACTION_JAMES Stored Procedure

Scenario: Purchasing four pairs of Trainers for James from ShoeShop.

**Operations:**
- Update James’s bank balance.
- Update ShoeShop’s bank balance.
- Update the inventory of Trainers at ShoeShop.
- Attempt to buy Brogues for James.

**Outcome:**
The transaction was rolled back because of insufficient funds when attempting to buy Brogues, ensuring the integrity of the entire transaction process.

**Skills Utilized**
- SQL: Structured Query Language for managing and manipulating relational databases.
- Database Management: Ensuring data integrity, performance optimization, and transaction control.
- Cloud Computing: Utilizing IBM Db2 cloud database for implementation.

**Technology Stack**
- IBM Db2 Cloud Database: A scalable and robust cloud database solution used for implementing the transactions and stored procedures.

**Project Impact**
- Data Integrity: Ensured by implementing ACID properties, critical for applications handling financial transactions or other sensitive operations.
- Transaction Reliability: Stored procedures automate and safeguard complex operations, reducing the risk of errors during data manipulation.
- Operational Efficiency: Streamlined database operations through reusable stored procedures, allowing for efficient transaction management.

**Conclusion**

This project highlights the importance of ACID transactions in maintaining the reliability and consistency of data within a database. By implementing stored procedures with transaction control, businesses can ensure that their operations are secure, efficient, and resistant to errors that could compromise data integrity.
