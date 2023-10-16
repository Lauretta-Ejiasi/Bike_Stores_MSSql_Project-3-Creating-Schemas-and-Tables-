# Bike_Stores_MSSql_Project 3 (Creating Schemas and Tables)

This project demonstrates my ability to create schemas and tables on MSSql using Bike Stores Database.

The BikeStores database is a sample database that can be used for learning and practicing SQL queries. It consists of several tables representing different aspects of a bike store's operations, including categories, brands, products, customers, stores, staffs, orders, order items, and stocks. For more details about the BikeStores database and how to load it, you can visit the page on https://www.sqlservertutorial.net/load-sample-database/?locale=en

Below is the breakdown of each query:

- CREATE SCHEMA production;: Creates a new schema called "production".
- CREATE SCHEMA sales;: Creates a new schema called "sales".
- CREATE TABLE production.categories: Creates a new table called "categories" in the "production" schema. The table has two columns: category_id (primary key) and category_name.
- CREATE TABLE production.brands: Creates a new table called "brands" in the "production" schema. The table has two columns: brand_id (primary key) and brand_name.
- CREATE TABLE production.products: Creates a new table called "products" in the "production" schema. The table has six columns: product_id (primary key), product_name, brand_id, category_id, model_year, and list_price. The brand_id and category_id columns are foreign keys referencing the respective tables.
- CREATE TABLE sales.customers: Creates a new table called "customers" in the "sales" schema. The table has nine columns: customer_id (primary key), first_name, last_name, phone, email, street, city, state, and zip_code.
- CREATE TABLE sales.stores: Creates a new table called "stores" in the "sales" schema. The table has eight columns: store_id (primary key), store_name, phone, email, street, city, state, and zip_code.
- CREATE TABLE sales.staffs: Creates a new table called "staffs" in the "sales" schema. The table has eight columns: staff_id (primary key), first_name, last_name, email, phone, active, store_id, and manager_id. The store_id and manager_id columns are foreign keys referencing the respective tables.
- CREATE TABLE sales.orders: Creates a new table called "orders" in the "sales" schema. The table has eight columns: order_id (primary key), customer_id, order_status, order_date, required_date, shipped_date, store_id, and staff_id. The customer_id, store_id, and staff_id columns are foreign keys referencing the respective tables.
- CREATE TABLE sales.order_items: Creates a new table called "order_items" in the "sales" schema. The table has six columns: order_id, item_id, product_id, quantity, list_price, and discount. The primary key consists of both the order_id and item_id columns, and the product_id column is a foreign key referencing the products table.
- CREATE TABLE production.stocks: Creates a new table called "stocks" in the "production" schema. The table has three columns: store_id, product_id, and quantity. The primary key consists of both the store_id and product_id columns, and both columns are foreign keys referencing their respective tables.


These SQL queries can also be used as a reference for creating similar tables and schemas in other SQL databases like MySql and PostgresSQL.
