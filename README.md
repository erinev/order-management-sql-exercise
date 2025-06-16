# Order Management SQL Exercise

## Problem Statement

A retailer company is looking to develop an order management system to streamline their order processing and products management.

Your task is to build a database that stores information related to customers, products and their orders. Additionally, the system should provide capabilities to generate reports about ordered products.

## Requirements

*Hint*: Some requirements are open-ended so you can implement them in a way that you think would be most convenient for the database user.

### Functional

* As a retailer I need a **database table** so I could manage **customers**. Each customer must have the following info: `first name`, `last name`, `email` and `details`;
    * `details` column contains data about customer location and must be stored using **JavaScript Object Notation** (JSON) e.g.: ``` { "country": "Lithuania", "city": "Kaunas" } ```
* As a retailer I need a **database table** so I could manage **products**. Each product must have the following info: `name`, `category` and `price`;
* As a retailer I need a **database table** so I could manage **orders**. Each order must contain the following info: `customer who made order`, `list of ordered products with quantity of each ordered item`;
* As a retailer I need an **SQL query** so I could retrieve an **order's invoice**. The invoice should contain a list of products where **each product** has `name`, `category`, `quantity`, `amount ($)` and additionally show `total amount ($)` to pay for all products.
    * It should be possible to perform **partial text search** by product `name` and `category` columns;
* As a retailer I need an **SQL query** so I could retrieve a **report about orders distribution by customer location**. The report should show the `customer city`, `number of orders` that were made from this city and `total amount ($)` of ordered products from this city;
    * It should be possible to **filter** by `customer city` column;
    * It should be possible to **order** by `number of orders` column;

### Non-Functional

* The solution code must be in a **Git repository**;
* Use **PostgreSQL** database;
* Include prerequisites, steps to launch and provide SQL query examples in **README**;
* **Mock** data in the main input tables:
    * `customers` table: 10,000 rows;
    * `products` table: 8,000 rows; 
    * `orders` table: 100,000 rows;
        * Number of different products in a single order should vary from 1 to 100;
        * Amount of a single product inside a single order should vary from 1 to 50;
        * Make sure data integrity is not violated (e.g., an order should contain only existing products);
* **Performance optimization**;
    * Any type of optimization which would make queries (**reads**) complete faster;
    * Also think about implications for **writes** performance;

### Bonus Points

* **Docker-Compose** for easy local testing;
    * meaning that DB tables and mocks would be applied automatically and we could test queries without needing to install PostgreSQL server on our machine;
* **Performance tests**;
* **Simple .NET API** which allows executing SQL queries for **order's invoice** and **report about orders distribution**;
    * Use `Swagger` for easier API request testing;

## Time for Solution

Take as long as you need on the solution, but we suggest limiting yourself to 8 hours or less. Do let us know how much time it took you! 

The task is not made to be completed in the period of 8 hours and no one expects you to! 
However, knowing how much time you spent and seeing the solution you came up with allows for seeing what you prioritize and where you would consider cutting corners on a sharp deadline.
