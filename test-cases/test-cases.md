# Manual Test Cases

## Project
Web Application Manual Testing

## Testing Type
Functional Testing

## Test Cases

| Test Case ID | Module | Test Scenario | Preconditions | Test Steps | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|---|
| TC-001 | Login | Login with valid credentials | Valid account exists | Enter valid username and password, then click Login | User should be logged in successfully | User was successfully logged in and redirected to the inventory/product page. | Pass |
| TC-002 | Login | Login with invalid password | Valid username exists | Enter valid username and incorrect password | Appropriate error message should be displayed | Error message "Epic sadface: Username and password do not match any user in this service" was displayed and login was prevented. | Pass |
| TC-003 | Login | Login with empty username | Login page is accessible | Leave username blank and enter password | Username validation message should be displayed | Error message "Epic sadface: Username is required" was displayed and login was prevented. | Pass |
| TC-004 | Login | Login with empty password | Login page is accessible | Enter username and leave password blank | Password validation message should be displayed | Error message "Epic sadface: Password is required" was displayed and login was prevented. | Pass |
| TC-005 | Login | Login with both fields empty | Login page is accessible | Leave username and password blank, then click Login | Appropriate validation message should be displayed | Error message "Epic sadface: Username is required" was displayed and login was prevented. | Pass |
| TC-006 | Products | Verify products page loads correctly | User is successfully logged in | Navigate to the Products page | Products page should display product names, prices, and Add to cart buttons | Products page loaded successfully with product names, prices, and Add to cart buttons visible. | Pass |
| TC-007 | Products | Verify product sorting by Name (Z to A) | User is logged in and Products page is displayed | Select "Name (Z to A)" from the sorting dropdown | Products should be displayed in descending alphabetical order | Products were successfully reordered in descending alphabetical order. | Pass |
| TC-008 | Cart | Add a product to the cart | User is logged in and Products page is displayed | Click "Add to cart" for Sauce Labs Backpack | Product should be added to the cart and cart count should increase to 1 | Sauce Labs Backpack was successfully added to the cart and the cart count displayed 1. | Pass |
| TC-009 | Cart | Verify added product appears in cart | Product has been added to cart | Open the shopping cart | Added product should be displayed with correct quantity, price, and Remove option | Sauce Labs Backpack was displayed in the cart with quantity 1, price $29.99, and a Remove button. | Pass |
| TC-010 | Cart | Remove product from cart | Sauce Labs Backpack is in the cart | Click "Remove" for Sauce Labs Backpack | Product should be removed and cart count should be cleared | Sauce Labs Backpack was successfully removed from the cart and the cart count disappeared. | Pass |
| TC-011 | Checkout | Checkout with valid customer information | Product is in the cart | Enter valid first name, last name, and postal code, then click Continue | User should be taken to the Checkout: Overview page | Valid customer information was accepted and the user was successfully redirected to the Checkout: Overview page. | Pass |
| TC-012 | Checkout | Checkout with missing First Name | Product is in the cart | Leave First Name blank, enter Last Name and Postal Code, then click Continue | A validation message should indicate that First Name is required | Error message "First Name is required" was displayed and the user could not continue. | Pass |
| TC-013 | Checkout | Checkout with missing Postal Code | Product is in the cart | Enter First Name and Last Name, leave Postal Code blank, then click Continue | A validation message should indicate that Postal Code is required | Error message "Postal Code is required" was displayed and the user could not continue. | Pass |
