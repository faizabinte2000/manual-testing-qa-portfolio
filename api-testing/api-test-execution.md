# API Test Execution Report

## Project

REST API Testing Practice

## API

JSONPlaceholder

## Test Environment

- API: JSONPlaceholder
- Testing Tool: Postman
- Testing Type: Manual API Testing

## Test Execution

| Test Case ID | Method | Endpoint | Expected Result | Actual Result | Status |
| ------------ | ------ | -------- | --------------- | ------------- | ------ |
| API-001 | GET | /users/1 | API should return HTTP 200 OK and a valid JSON response containing user details | API returned 200 OK with valid JSON containing ID 1, name "Leanne Graham", username "Bret", and email "Sincere@april.biz". | PASS |
| API-002 | POST | /users | API should return HTTP 201 Created and the response should contain the submitted user data and a generated ID | API returned 201 Created with the submitted name, username, email, and generated ID 11. | PASS |
| API-003 | PUT | /users/1 | API should return HTTP 200 OK and the response should contain the updated user information | API returned 200 OK with the updated name, username, email, and ID 1. | PASS |
| API-004 | DELETE | /users/1 | API should return a successful HTTP response and an appropriate response body after deletion | API returned 200 OK with an empty JSON object `{}`. | PASS |
| API-005 | GET | /users/9999 | API should return HTTP 404 Not Found for an unavailable resource | API returned 404 Not Found with an empty JSON response `{}`. | PASS |
| API-006 | POST | /users | API should reject incomplete user data with an appropriate 4xx validation response | API returned 201 Created and accepted the incomplete payload, returning username and generated ID. | FAIL |
| API-007 | GET | /users/1 | Response should contain the expected user fields with appropriate data types and nested objects | Response contained all expected fields, including id, name, username, email, address, phone, website, and company, with address and company represented as objects. | PASS |
| API-008 | GET | /users/1 | Response should have a JSON Content-Type | Response Content-Type was `application/json; charset=utf-8`. | PASS |

## Execution Summary

- Total Test Cases: 8
- Passed: 7
- Failed: 1
- Blocked: 0

## Overall Result

Seven of the eight executed API test cases passed successfully. One negative test case failed because the API accepted an incomplete user payload instead of returning a validation error.

## Conclusion

The API testing exercise covered GET, POST, PUT, and DELETE operations, along with negative testing, response structure validation, HTTP status code validation, and response Content-Type validation. The failed negative test demonstrated the importance of validating API behavior against expected requirements rather than considering every successful HTTP response as a functional success.
