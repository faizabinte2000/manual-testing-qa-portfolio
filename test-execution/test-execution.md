# Test Execution Report

## Project

Swag Labs – Web Application Manual Testing

## Testing Type

Functional Testing

## Test Environment

- Application: Swag Labs
- Testing Type: Manual Functional Testing
- Browser: Google Chrome
- Test Execution: Manual

## Test Execution Summary

| Test Case ID | Module | Test Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|
| TC-001 | Login | Login with valid credentials | User should be logged in successfully | User was successfully logged in and redirected to the inventory/product page. | PASS |
| TC-002 | Login | Login with invalid password | Appropriate error message should be displayed | Error message "Epic sadface: Username and password do not match any user in this service" was displayed and login was prevented. | PASS |
| TC-003 | Login | Login with empty username | Username validation message should be displayed | Error message "Epic sadface: Username is required" was displayed and login was prevented. | PASS |
| TC-004 | Login | Login with empty password | Password validation message should be displayed | Error message "Epic sadface: Password is required" was displayed and login was prevented. | PASS |
| TC-005 | Login | Login with both fields empty | Appropriate validation message should be displayed | Error message "Epic sadface: Username is required" was displayed and login was prevented. | PASS |
| TC-006 | Products | Verify products page loads correctly | Products page should display product names, prices, and Add to cart buttons | Products page loaded successfully with product names, prices, and Add to cart buttons visible. | PASS |
| TC-007 | Products | Verify product sorting by Name (Z to A) | Products should be displayed in descending alphabetical order | Products were successfully reordered in descending alphabetical order. | PASS |
| TC-008 | Cart | Add a product to the cart | Product should be added to the cart and cart count should increase to 1 | Sauce Labs Backpack was successfully added to the cart and the cart count displayed 1. | PASS |
| TC-009 | Cart | Verify added product appears in cart | Added product should be displayed with correct quantity, price, and Remove option | Sauce Labs Backpack was displayed in the cart with quantity 1, price $29.99, and a Remove button. | PASS |
| TC-010 | Cart | Remove product from cart | Product should be removed and cart count should be cleared | Sauce Labs Backpack was successfully removed from the cart and the cart count disappeared. | PASS |
| TC-011 | Checkout | Checkout with valid customer information | User should be taken to the Checkout: Overview page | Valid customer information was accepted and the user was successfully redirected to the Checkout: Overview page. | PASS |
| TC-012 | Checkout | Checkout with missing First Name | A validation message should indicate that First Name is required | Error message "First Name is required" was displayed and the user could not continue. | PASS |
| TC-013 | Checkout | Checkout with missing Postal Code | A validation message should indicate that Postal Code is required | Error message "Postal Code is required" was displayed and the user could not continue. | PASS |
| TC-014 | Checkout | Verify checkout order summary | Order summary should display the correct product, quantity, price, item total, tax, and final total | Sauce Labs Backpack was displayed with quantity 1 and price $29.99. Item total was $29.99, tax was $2.40, and final total was $32.39. Payment and shipping information were also displayed. | PASS |
| TC-015 | Checkout | Complete an order successfully | Order should be completed and a confirmation message should be displayed | Checkout was successfully completed. The "Checkout: Complete!" page and "Thank you for your order!" confirmation message were displayed. | PASS |
| TC-016 | Products | Verify product sorting by Price (Low to High) | Products should be displayed in ascending order of price | Products were successfully reordered from lowest to highest price. | PASS |
| TC-017 | Checkout | Verify cart state after cancelling checkout | User should leave the checkout flow, return to the appropriate previous page, and the product should remain in the cart with the correct cart count | User successfully exited the checkout flow and returned to the previous page. The product remained in the cart, the cart count remained correct, and no unintended changes were observed. | PASS |

## Execution Summary

- Total Test Cases: 17
- Passed: 17
- Failed: 0
- Blocked: 0
## Test Coverage

The test execution covered the following modules:

- Login
- Products
- Cart
- Checkout

## Overall Result

All 17 executed test cases passed successfully.

## Conclusion

The tested Swag Labs functionalities behaved as expected during manual functional testing. The execution covered authentication, product page functionality, product sorting, cart operations, checkout validation, order summary verification, and successful order completion.
