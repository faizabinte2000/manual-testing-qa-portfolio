# Manual Test Cases

## Project
Web Application Manual Testing

## Testing Type
Functional Testing

## Test Cases

| Test Case ID | Module | Test Scenario | Preconditions | Test Steps | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|---|
| TC-001 | Login | Login with valid credentials | Valid account exists | Enter valid username and password, then click Login | User should be logged in successfully | To be executed | Not Run |
| TC-002 | Login | Login with invalid password | Valid username exists | Enter valid username and incorrect password | Appropriate error message should be displayed | To be executed | Not Run |
| TC-003 | Login | Login with empty username | Login page is accessible | Leave username blank and enter password | Username validation message should be displayed | To be executed | Not Run |
| TC-004 | Login | Login with empty password | Login page is accessible | Enter username and leave password blank | Password validation message should be displayed | To be executed | Not Run |
| TC-005 | Login | Login with both fields empty | Login page is accessible | Leave username and password blank, then click Login | Appropriate validation messages should be displayed | To be executed | Not Run |
