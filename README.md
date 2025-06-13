# order-management-sql-exercise

# Problem statement

TBA

# Requirements

## Functional
* TBA

## Non-Functional
* **Mock** data to main input tables:
  * `users` table: 10 000 rows;
  * `products` table: 8 000 rows; 
  * `orders` table: 100 000 rows;
    * Order should contain amount of each product that was ordered;
    * Orders should contain only existing products;
    * Number of different products in single order should vary from 1 to 100;
    * Amount of single product ordered should vary from 1 to 50;
* Include prerequisites, steps to launch and provide SQL query examples in **README**;
* The solution code must be in a **Git repository**;

## Bonus points stuff
* Performance optimization; 
* `Docker-Compose` for easy local testing;
  * meaning that DB tables and mocks would be applied automatically and we could test queries without need to instal PostgreSQL server on our machine;
* Performance tests;
* Simple .NET API which allows to execute SQL queries on output data;
  * We recommend to use `Swagger` for easier API request testing;

# Time for solution

Take as long as you need on the solution but we suggest to limit yourself at 8 hours. Do let us know how much time it took you!

The task is not made to be completed in the period of 8 hours and no one expects you to! 
However, knowing how much time you spent and seeing the solution you came up with allows for seeing what you prioritize and where you would consider cutting corners on a sharp deadline.
