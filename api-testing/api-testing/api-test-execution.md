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

## Execution Summary

- Total Test Cases: 1
- Passed: 1
- Failed: 0
- Blocked: 0

## Overall Result

The GET request was successfully executed using Postman and returned the expected response with HTTP 200 OK.

## Conclusion

API-001 successfully validated basic GET request functionality, HTTP status code handling, and response data validation.
