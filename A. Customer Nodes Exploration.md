# 💵 Case Study #4 - Data Bank

## 🏦 Solution - A. Customer Nodes Exploration

**1. How many unique nodes are there on the Data Bank system?**

````sql
SELECT 
  COUNT(DISTINCT node_id)
FROM data_bank.customer_nodes;
````

**Answer:**

<img width="97" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/A.%20Customer%20Nodes%20Exploration/1.png">

- There are 5 unique nodes on Data Bank system.

***

**2. What is the number of nodes per region?**

````sql
SELECT 
  r.region_id, 
  r.region_name, 
  COUNT(*) AS node_count
FROM data_bank.regions r
JOIN data_bank.customer_nodes n
  ON r.region_id = n.region_id
GROUP BY r.region_id, r.region_name
ORDER BY region_id;
````

**Answer:**

<img width="391" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/A.%20Customer%20Nodes%20Exploration/2.png">

***

**3. How many customers are allocated to each region?**

````sql
SELECT 
  region_id, 
  COUNT(customer_id) AS customer_count
FROM data_bank.customer_nodes
GROUP BY region_id
ORDER BY region_id;
````

**Answer:**

<img width="296" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/A.%20Customer%20Nodes%20Exploration/3.png">

***

**4. How many days on average are customers reallocated to a different node?**

````sql
WITH node_diff AS (
  SELECT 
    customer_id, node_id, start_date, end_date,
    end_date - start_date AS diff
  FROM data_bank.customer_nodes
  WHERE end_date != '9999-12-31'
  GROUP BY customer_id, node_id, start_date, end_date
  ORDER BY customer_id, node_id
  ),
sum_diff_cte AS (
  SELECT 
    customer_id, node_id, SUM(diff) AS sum_diff
  FROM node_diff
  GROUP BY customer_id, node_id)

SELECT 
  ROUND(AVG(sum_diff),2) AS avg_reallocation_days
FROM sum_diff_cte;
````

**Answer:**

<img width="178" alt="image" src="https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/images/A.%20Customer%20Nodes%20Exploration/4.png">

- On average, customers are reallocated to a different node every 24 days.

***


***

Click [here](https://github.com/yaswanthteja/SQL_Dannys_Data-Bank_CaseStudy4/blob/master/B.Customer_Transactions.md) for **B. Customer Transactions** solution!
