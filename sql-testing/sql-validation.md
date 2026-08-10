# SQL Validation Queries

## Project

E-commerce Database Validation Practice

## Testing Type

SQL Data Validation Testing

## Database

MySQL

## Purpose

This document contains the SQL queries used to validate customer, product, and order data during manual database testing.

---

## SQL-001 — Retrieve All Customers

### Query

```sql
SELECT * FROM customers;
```

### Validation

Verified that all customer records were successfully retrieved from the database.

### Result

4 customer records were returned successfully.

**Status: PASS**

---

## SQL-002 — Filter Customers by City

### Query

```sql
SELECT *
FROM customers
WHERE city = 'Dhaka';
```

### Validation

Verified that the database correctly filters customer records based on their city.

### Result

2 customers from Dhaka were returned:

- Aisha Rahman
- Sara Karim

**Status: PASS**

---

## SQL-003 — Sort Products by Price

### Query

```sql
SELECT *
FROM products
ORDER BY price ASC;
```

### Validation

Verified that products are displayed in ascending order based on price.

### Result

All 4 products were returned in the correct ascending price order:

1. Wireless Mouse — 1200.00
2. USB-C Hub — 1800.00
3. Laptop Stand — 2500.00
4. Mechanical Keyboard — 4500.00

**Status: PASS**

---

## SQL-004 — Join Customers with Orders

### Query

```sql
SELECT
    o.order_id,
    c.name AS customer_name,
    c.city,
    o.product_id,
    o.quantity,
    o.order_total
FROM orders o
INNER JOIN customers c
    ON o.customer_id = c.customer_id;
```

### Validation

Verified that customer information is correctly associated with their orders using the customer ID relationship.

### Result

4 orders were returned with the correct customer information.

| Order ID | Customer Name | City |
| -------- | ------------- | ---- |
| 1001 | Aisha Rahman | Dhaka |
| 1002 | Nadia Ahmed | Chattogram |
| 1003 | Sara Karim | Dhaka |
| 1004 | Aisha Rahman | Dhaka |

**Status: PASS**

---

## SQL-005 — Validate Order Total

### Query

```sql
SELECT
    o.order_id,
    p.product_name,
    p.price,
    o.quantity,
    p.price * o.quantity AS calculated_total,
    o.order_total AS stored_total
FROM orders o
INNER JOIN products p
    ON o.product_id = p.product_id;
```

### Validation

Verified that the calculated order total matches the order total stored in the database.

The calculated total is determined using:

```text
Product Price × Quantity = Calculated Total
```

### Result

The calculated totals matched the stored order totals for all 4 orders.

| Order ID | Product | Quantity | Calculated Total | Stored Total |
| -------- | ------- | -------- | ---------------- | ------------ |
| 1001 | Wireless Mouse | 2 | 2400.00 | 2400.00 |
| 1002 | Mechanical Keyboard | 1 | 4500.00 | 4500.00 |
| 1003 | USB-C Hub | 2 | 3600.00 | 3600.00 |
| 1004 | Laptop Stand | 1 | 2500.00 | 2500.00 |

**Status: PASS**

---

## Execution Summary

- **Total SQL Test Cases:** 5
- **Passed:** 5
- **Failed:** 0
- **Blocked:** 0

## Overall Result

All 5 SQL validation tests passed successfully.

## Conclusion

The SQL testing exercise successfully demonstrated database validation using MySQL. The tests covered data retrieval, filtering, sorting, table joins, and calculated-value validation.

The exercise also demonstrated how SQL can be used by QA testers to verify that application data is correctly stored and related within a database.
