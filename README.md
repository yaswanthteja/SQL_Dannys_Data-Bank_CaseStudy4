## Case Study #4: Data Bank

<img src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/Readme/DataBank.png" alt="Image" width="500" height="520">

## 📚 Table of Contents
- [Business Task](#business-task)
- [Entity Relationship Diagram](#entity-relationship-diagram)
- [Case Study Questions](#case-study-questions)
- Solution
  - [A. Customer Nodes Exploration](https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/A.%20Customer%20Nodes%20Exploration.md)
  - [B. Customer Transactions](https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/B.Customer_Transactions.md)
  - [Complete SQL Syntax](https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/SQL%20Syntax/Complete%20SQL%20solution.sql)

***

## Business Task
Danny launched a new initiative, Data Bank which runs **banking activities** and also acts as the world’s most secure distributed **data storage platform**!

Customers are allocated cloud data storage limits which are directly linked to how much money they have in their accounts. 

The management team at Data Bank want to increase their total customer base - but also need some help tracking just how much data storage their customers will need.

This case study is all about calculating metrics, growth and helping the business analyse their data in a smart way to better forecast and plan for their future developments!

## Entity Relationship Diagram

<img width="631" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/Readme/Entity%20Relationship%20Diagram.png">

**Table 1: Regions**

This regions table contains the region_id and their respective region_name values.

<img width="176" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/Readme/Table1-%20Regions.png">

**Table 2: Customer Nodes**

Customers are randomly distributed across the nodes according to their region. This random distribution changes frequently to reduce the risk of hackers getting into Data Bank’s system and stealing customer’s money and data!

<img width="412" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/Readme/Table%202-customerNodes.png">

**Table 3: Customer Transactions**

This table stores all customer deposits, withdrawals and purchases made using their Data Bank debit card.

<img width="343" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/Readme/Table%203-%20CustomerTransactions.png">

***

## Case Study Questions

### A. Customer Nodes Exploration

View my solution [here](https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/A.%20Customer%20Nodes%20Exploration.md).

1. How many unique nodes are there on the Data Bank system?
2. What is the number of nodes per region?
3. How many customers are allocated to each region?
4. How many days on average are customers reallocated to a different node?
5. What is the median, 80th and 95th percentile for this same reallocation days metric for each region?

### B. Customer Transactions

View my solution [here](https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/B.Customer_Transactions.md).
  
1. What is the unique count and total amount for each transaction type?
2. What is the average total historical deposit counts and amounts for all customers?
3. For each month - how many Data Bank customers make more than 1 deposit and either 1 purchase or 1 withdrawal in a single month?
4. What is the closing balance for each customer at the end of the month?
5. Comparing the closing balance of a customer’s first month and the closing balance from their second nth, what percentage of customers:
  - Have a negative first month balance?
  - Have a positive first month balance?
  - Increase their opening month’s positive closing balance by more than 5% in the following month?
  - Reduce their opening month’s positive closing balance by more than 5% in the following month?
  - Move from a positive balance in the first month to a negative balance in the second month?
  
***

Do give me a 🌟 if you like what you're reading. Thank you! 🙆🏻‍♀️




- [SQL_Dannys_Diner_CaseStudy1](https://github.com/yaswanthteja/SQL_Dannys_Diner_CaseStudy1)


- [SQL_Dannys_Pizza_Runner_CaseStudy2-](https://github.com/yaswanthteja/SQL_Dannys_Pizza_Runner_CaseStudy2-)

- [SQL_Dannys_Foodiee-Fi_CaseStudy3](https://github.com/yaswanthteja/SQL_Dannys_Foodiee-Fi_CaseStudy3)

- [SQL_Dannys_Data-Bank_CaseStudy4](https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4)

