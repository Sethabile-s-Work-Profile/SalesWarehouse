# Sales Data Warehouse

## Overview

This project is a **SQL Server Sales Data Warehouse** created to strengthen my understanding of relational database design, SQL development, and data engineering fundamentals.

The database models a simple sales system consisting of customers, products, orders, and order details. It serves as a practice environment for writing SQL queries, performing data analysis, and exploring data warehouse concepts.

## Objectives

* Design a relational database using SQL Server
* Create tables with primary and foreign key relationships
* Populate tables with realistic sample data
* Practice SQL queries ranging from beginner to advanced
* Explore data warehouse and reporting concepts

## Database Schema

The project consists of four main tables:

### Customers

Stores customer information.

| Column     | Description                  |
| ---------- | ---------------------------- |
| CustomerId | Unique customer identifier   |
| FirstName  | Customer's first name        |
| LastName   | Customer's last name         |
| Email      | Customer email address       |
| City       | Customer city                |
| SignupDate | Date the customer registered |

### Products

Stores product information.

| Column      | Description               |
| ----------- | ------------------------- |
| ProductId   | Unique product identifier |
| ProductName | Product name              |
| Category    | Product category          |
| Price       | Product price             |

### Orders

Stores customer orders.

| Column     | Description                   |
| ---------- | ----------------------------- |
| OrderId    | Unique order identifier       |
| CustomerId | Customer who placed the order |
| OrderDate  | Date the order was placed     |

### OrderDetailId

Stores the products contained within each order.

| Column        | Description                    |
| ------------- | ------------------------------ |
| OrderDetailId | Unique order detail identifier |
| OrderId       | Related order                  |
| ProductId     | Purchased product              |
| Quality       | Quantity purchased             |
| UnitPrice     | Price at the time of purchase  |

## Entity Relationships

```text
Customers
    │
    │ CustomerId
    ▼
Orders
    │
    │ OrderId
    ▼
OrderDetailId
    │
    │ ProductId
    ▼
Products
```

## Skills Demonstrated

* SQL Server
* Database Design
* Primary & Foreign Keys
* Relational Data Modeling
* Data Warehousing Fundamentals
* Data Analysis with SQL
* Query Optimization
* Joins
* Aggregate Functions
* Grouping and Filtering
* Subqueries
* Window Functions (planned)

## Example SQL Queries

Examples of analyses that can be performed using this database include:

* Total sales revenue
* Best-selling products
* Top spending customers
* Sales by city
* Monthly sales trends
* Average order value
* Product category performance

## Technologies Used

* Microsoft SQL Server
* SQL Server Management Studio (SSMS)

## Future Improvements

* Add Date, Customer, and Product dimension tables
* Build a Star Schema
* Create ETL pipelines
* Integrate with Power BI dashboards
* Add stored procedures, views, and indexes
* Expand the dataset with additional sales records

## Author

**Likhona Dlamini**

Aspiring Data Engineer | Cloud Enthusiast | SQL & Data Analytics Learner
