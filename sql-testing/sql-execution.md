# SQL Test Execution Report

## Project

E-commerce Database Validation Practice

## Testing Type

SQL Data Validation Testing

## Database

MySQL

## Test Environment

- Database: MySQL 8.4
- Tool: MySQL Workbench
- Testing Type: Manual SQL Testing
- Database: Local `qa_ecommerce` database

## Test Execution

| Test Case ID | Test Scenario | Expected Result | Actual Result | Status |
| ------------ | ------------- | --------------- | ------------- | ------ |
| SQL-001 | Retrieve all customers | All customer records should be returned | 4 customer records were returned successfully. | PASS |
| SQL-002 | Filter customers by city | Only customers from the specified city should be returned | 2 customers from Dhaka, Aisha Rahman and Sara Karim, were returned. | PASS |
| SQL-003 | Sort products by price | Products should be displayed in ascending price order | All 4 products were returned in the correct ascending price order. | PASS |
| SQL-004 | Join customers with orders | Matching customer and order records should be returned | 4 orders were returned with the correct customer information. | PASS |
| SQL-005 | Validate order total | Calculated order total should match the stored order total | Calculated totals matched the stored order totals for all 4 orders. | PASS |

## Execution Summary

- **Total Test Cases:** 5
- **Passed:** 5
- **Failed:** 0
- **Blocked:** 0

## Test Coverage

The SQL testing covered:

- Data retrieval using `SELECT`
- Data filtering using `WHERE`
- Data sorting using `ORDER BY`
- Relational data validation using `INNER JOIN`
- Calculated-value validation
- Customer, product, and order data relationships

## Overall Result

All 5 SQL test cases passed successfully.

## Conclusion

The SQL testing exercise successfully validated customer, product, and order data within the MySQL database. The testing demonstrated the use of SQL queries to verify data accuracy, filtering, sorting, table relationships, and calculated values.
