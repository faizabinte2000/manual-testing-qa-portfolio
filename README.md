# Manual Testing & QA Portfolio

A hands-on Software Quality Assurance portfolio demonstrating **manual functional testing, API testing, SQL database validation, test case design, test execution, and bug reporting**.

The project uses the **Swag Labs web application** for manual testing and **JSONPlaceholder** and a local MySQL database for API and SQL testing practice.

---

## Project Overview

This portfolio was created to demonstrate practical QA skills through hands-on testing activities.

The project covers:

- Manual functional testing
- Positive and negative testing
- Test case design
- Test execution and documentation
- Bug reporting
- REST API testing using Postman
- SQL database validation using MySQL
- Response and data validation

---

# 1. Manual Web Application Testing

## Application

Swag Labs

## Testing Type

Manual Functional Testing

## Testing Scope

The following modules were tested:

- Login
- Products
- Product Sorting
- Shopping Cart
- Checkout
- Order Completion

## Test Coverage

A total of **17 manual test cases** were designed and executed.

| Module | Test Cases | Result |
| ------ | ---------: | ------ |
| Login | 5 | 5 Passed |
| Products | 2 | 2 Passed |
| Cart | 3 | 3 Passed |
| Checkout | 6 | 6 Passed |
| **Total** | **17** | **17 Passed** |

### Execution Summary

- **Total Test Cases:** 17
- **Passed:** 17
- **Failed:** 0
- **Blocked:** 0

## Manual Testing Activities

- Designed functional test cases
- Defined test scenarios and preconditions
- Documented test steps and expected results
- Executed test cases manually
- Recorded actual results and test status
- Performed positive and negative testing
- Tested authentication and validation
- Tested product sorting
- Tested shopping cart operations
- Tested checkout workflow
- Verified order summary and calculations
- Tested checkout navigation and cart persistence
- Identified and documented a UI defect
- Attached screenshot evidence to the bug report
- Tested checkout navigation and cart persistence

---

# 2. API Testing

## API

JSONPlaceholder

## Testing Tool

Postman

## Testing Type

Manual API Testing

## API Test Coverage

A total of **8 API test cases** were designed and executed.

| Test Case | Method | Testing Area | Result |
| --------- | ------ | ------------ | ------ |
| API-001 | GET | Retrieve existing user | PASS |
| API-002 | POST | Create user | PASS |
| API-003 | PUT | Update user | PASS |
| API-004 | DELETE | Delete user | PASS |
| API-005 | GET | Non-existent resource | PASS |
| API-006 | POST | Incomplete request payload | FAIL |
| API-007 | GET | Response structure validation | PASS |
| API-008 | GET | Content-Type validation | PASS |

### API Execution Summary

- **Total Test Cases:** 8
- **Passed:** 7
- **Failed:** 1
- **Blocked:** 0

The failed test was a negative test involving an incomplete user payload. The API accepted the incomplete payload and returned `201 Created` instead of returning a validation error.

## API Testing Activities

- GET request testing
- POST request testing
- PUT request testing
- DELETE request testing
- HTTP status-code validation
- Response-body validation
- Negative API testing
- Response structure validation
- Response header validation
- Content-Type validation
- Manual API testing using Postman

---

# 3. SQL Database Testing

## Database

MySQL

## Tool

MySQL Workbench

## Testing Type

SQL Data Validation Testing

A local e-commerce database was created for testing customer, product, and order data.

## SQL Test Coverage

A total of **5 SQL test cases** were executed.

| Test Case | SQL Operation | Testing Area | Result |
| --------- | ------------- | ------------ | ------ |
| SQL-001 | SELECT | Retrieve customer records | PASS |
| SQL-002 | SELECT + WHERE | Filter customers by city | PASS |
| SQL-003 | SELECT + ORDER BY | Sort products by price | PASS |
| SQL-004 | INNER JOIN | Validate customer-order relationships | PASS |
| SQL-005 | Calculation + JOIN | Validate order totals | PASS |

### SQL Execution Summary

- **Total Test Cases:** 5
- **Passed:** 5
- **Failed:** 0
- **Blocked:** 0

## SQL Testing Activities

- Data retrieval using `SELECT`
- Data filtering using `WHERE`
- Data sorting using `ORDER BY`
- Relational data validation using `INNER JOIN`
- Calculated-value validation
- Customer and order relationship validation
- Product and order data validation

---

# 4. Bug Reporting

A UI defect was identified during manual testing involving an **incorrect product image being displayed**.

The defect was documented with:

- Bug ID
- Bug description
- Steps to reproduce
- Expected result
- Actual result
- Screenshot evidence

### Bug Evidence

The supporting screenshot is available in the `bug-reports` folder.

---

# Tools & Technologies

### Testing Tools

- Postman
- MySQL Workbench
- Google Chrome
- Git
- GitHub

### Technical Skills

- Manual Testing
- Functional Testing
- API Testing
- SQL Testing
- REST APIs
- Test Case Design
- Test Execution
- Bug Reporting
- Data Validation
- HTTP Status Codes
- JSON
- MySQL

### Testing Techniques

- Positive Testing
- Negative Testing
- Functional Testing
- Response Validation
- Database Validation
- Boundary/Validation Testing
- End-to-End Workflow Testing

---

# Repository Structure

```text
manual-testing-qa-portfolio/
│
├── README.md
│
├── test-cases/
│   └── test-cases.md
│
├── test-execution/
│   └── test-execution.md
│
├── bug-reports/
│   ├── bug-reports.md
│   └── BUG-001-incorrect-product-image.jpg
│
├── api-testing/
│   ├── api-test-cases.md
│   └── api-test-execution.md
│
└── sql-testing/
    ├── sql-test-cases.md
    ├── sql-validation.md
    └── sql-execution.md
```

---

# Project Outcome

This project provided hands-on experience in the complete QA testing workflow, from **test case design and execution to defect reporting, API validation, and database verification**.

The portfolio demonstrates practical experience with:

- Manual web application testing
- REST API testing using Postman
- SQL database validation using MySQL
- Test documentation
- Defect reporting
- Positive and negative testing
- Data and response validation

The project is intended to demonstrate practical QA skills and provide a foundation for further learning in **Software Quality Assurance and Test Automation**.
