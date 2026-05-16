## Overview
This is a relational database project designed for a computer store utilizing MySQL Workbench. It stores information about the customers, employees, products, sales orders, and order details. This projects demonstrates the database design, table relationships, primary keys, foreign keys, sample data insertion, and SQL queries.

## Database Purpose
The purpose of this database is to enable a computer store to capture customer orders, employee sales activity, product inventory, and order details. This can be used to answer business queries such as the best-selling items, employees who handled orders, and customers with high-value orders.

## Database Tables
The database includes five main tables:

- **Customer**: Stores customer contact and registration information.
- **Employee**: Stores employee contact information, hire dates, and roles.
- **Product**: Stores product details such as SKU, brand, model, category, price, and inventory quantity.
- **SalesOrder**: Stores order information including order date, payment method, total amount, customer ID, and employee ID.
- **OrderDetail**: Stores individual items within each order, including quantity, sale price, line total, sales order ID, and product ID.

## Table Relationships
- Each customer can place multiple sales orders.
- Each employee can handle multiple sales orders.
- Each sales order can contain multiple order details.
- Each product can appear in multiple order details.

The `SalesOrder` table connects customers and employees, while the `OrderDetail` table connects sales orders and products.

## SQL Features Demonstrated
This project demonstrates the following SQL concepts:

- Creating databases and tables
- Primary keys
- Foreign keys
- Auto-incrementing IDs
- Data insertion with `INSERT INTO`
- Filtering with `WHERE`
- Sorting with `ORDER BY`
- Aggregate functions with `SUM`
- Grouping with `GROUP BY`
- Filtering grouped results with `HAVING`
- Wildcard searches using `LIKE`
- Subqueries
- Table joins using `JOIN`

## Queries

### Query 1: Product Filter Query
Finds products with a unit price greater than or equal to $50 and at least 20 units in stock.

![Product Filter Query](queries/product-filter-query.png)

### Query 2: Product Sales Summary Query
Groups order details by product and shows products that sold more than 2 total units.

![Product Sales Summary Query](queries/product-sales-summary-query.png)

### Query 3: Customer Phone Search Query
Finds customers whose phone number begins with `770`.

![Customer Phone Search Query](queries/customer-phone-search-query.png)

### Query 4: Employee Order Subquery
Finds employees who handled sales orders using a nested query.

![Employee Order Subquery](queries/employee-order-subquery.png)

### Query 5: High-Value Orders Join Query
Uses a join to display customer names for orders over $500.

![High Value Orders Join Query](queries/high-value-orders-join-query.png)

## Tables

### Customer Table
![Customer Table](tables/customer-table.png)

### Employee Table
![Employee Table](tables/employee-table.png)

### Product Table
![Product Table](tables/product-table.png)

### Sales Order Table
![Sales Order Table](tables/sales-order-table.png)

### Order Detail Table
![Order Detail Table](tables/order-detail-table.png)
