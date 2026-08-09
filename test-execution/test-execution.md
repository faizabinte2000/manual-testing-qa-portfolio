# Test Execution Report

## Project
Swag Labs – Manual Testing

## Test Environment
- Application: Swag Labs
- Testing Type: Manual Functional Testing
- Browser: Google Chrome
- Test Date: August 2026

## Execution Summary

| Test Case ID | Test Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|
| TC-001 | Login with valid credentials | User should be logged in successfully | User was logged in successfully | PASS |
| TC-002 | Login with invalid credentials | Appropriate error message should be displayed | "Epic sadface: Username and password do not match any user in this service" was displayed | PASS |
| TC-003 | Login with blank username | Username validation message should be displayed | "Epic sadface: Username is required" was displayed | PASS |
| TC-004 | Login with blank password | Password validation message should be displayed | "Epic sadface: Password is required" was displayed | PASS |
| TC-005 | Add product to cart | Product should be added and cart count should update | Product was added, button changed to "Remove", and cart count changed to 1 | PASS |
| TC-006 | Checkout with missing first name | First Name validation message should be displayed | "Error: First Name is required" was displayed | PASS |
| TC-007 | Checkout with missing postal code | Postal Code validation message should be displayed | "Error: Postal Code is required" was displayed | PASS |
| TC-008 | Complete checkout with valid information | Order should be completed successfully | "Checkout: Complete!" page was displayed | PASS |

## Overall Result

All executed test cases passed successfully.

## Conclusion

The tested Swag Labs functionalities behaved as expected during manual functional testing. The test execution covered authentication, product selection, cart functionality, checkout validation, and successful order completion.
