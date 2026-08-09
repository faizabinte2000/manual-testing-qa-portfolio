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
