# SQL Test Cases

## Project

E-commerce Database Validation Practice

## Testing Type

SQL Data Validation Testing

## Database

MySQL

## Test Cases

| Test Case ID | Test Scenario              | SQL Operation        | Expected Result                                            | Actual Result                                                                                         | Status |
| ------------ | -------------------------- | -------------------- | ---------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ------ |
| SQL-001      | Retrieve all customers     | SELECT               | All customer records should be returned                    | 4 customer records were returned successfully.                                                       | PASS   |
| SQL-002      | Filter customers by city   | SELECT + WHERE       | Only customers from the specified city should be returned  | 2 customers from Dhaka, Aisha Rahman and Sara Karim, were returned.                                   | PASS   |
| SQL-003      | Sort products by price     | SELECT + ORDER BY    | Products should be displayed in ascending price order      | All 4 products were returned in ascending order of price.                                            | PASS   |
| SQL-004      | Join customers with orders | INNER JOIN           | Matching customer and order records should be returned     | 4 orders were returned with the correct customer information.                                        | PASS   |
| SQL-005      | Validate order total       | SELECT + calculation | Calculated order total should match the stored order total | Calculated order totals matched the stored order totals for all 4 orders.                            | PASS   |
