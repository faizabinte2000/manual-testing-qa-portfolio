# Manual Testing & QA Portfolio

A manual software testing portfolio demonstrating functional testing, test case design, test execution, bug reporting, and QA documentation using the Swag Labs web application.

## Project Overview

This project was created to practice and demonstrate core Software Quality Assurance (SQA) activities through hands-on manual testing.

The testing focused on validating major user workflows including authentication, product browsing, cart operations, and checkout.

## Testing Scope

The following modules were tested:

- Login
- Products
- Product Sorting
- Shopping Cart
- Checkout
- Order Completion

## Test Coverage

A total of **15 manual test cases** were designed and executed.

| Module | Test Cases | Result |
|---|---:|---|
| Login | 5 | 5 Passed |
| Products | 2 | 2 Passed |
| Cart | 3 | 3 Passed |
| Checkout | 5 | 5 Passed |
| **Total** | **15** | **15 Passed** |

### Execution Summary

- **Total Test Cases:** 15
- **Passed:** 15
- **Failed:** 0
- **Blocked:** 0

## Testing Activities

The following QA activities were performed:

- Designed functional test cases
- Defined test scenarios and preconditions
- Documented test steps and expected results
- Executed test cases manually
- Recorded actual results and test status
- Performed negative testing for login and checkout validation
- Tested shopping cart operations
- Tested product sorting functionality
- Verified checkout calculations and order summary
- Identified and documented a UI defect
- Attached screenshot evidence to a bug report

## Bug Reporting

A UI defect was identified during testing involving an incorrect product image being displayed.

The defect was documented with:

- Bug ID
- Bug description
- Steps to reproduce
- Expected result
- Actual result
- Screenshot evidence

See the `bug-reports` folder for the complete bug report and supporting screenshot.

## Test Evidence

The repository contains documentation and evidence from the testing process, including:

- Manual test cases
- Test execution results
- Bug report
- Screenshot evidence

## Repository Structure

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
└── bug-reports/
    ├── bug-reports.md
    └── BUG-001-incorrect-product-image.jpg
