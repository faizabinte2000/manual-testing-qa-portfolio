# API Test Cases

## Project

REST API Testing Practice

## API

JSONPlaceholder

## Test Cases

| Test Case ID | Method | Endpoint | Test Scenario | Expected Result | Actual Result | Status |
| ------------ | ------ | -------- | ------------- | --------------- | ------------- | ------ |
| API-001 | GET | /users/1 | Retrieve user by ID | API should return HTTP 200 OK and a valid JSON response containing user details | API returned 200 OK with valid JSON containing ID 1, name "Leanne Graham", username "Bret", and email "Sincere@april.biz". | PASS |
| API-002 | POST | /users | Create a new user with valid data | API should return HTTP 201 Created and the response should contain the submitted user data and a generated ID | API returned 201 Created with the submitted name, username, email, and generated ID 11. | PASS |
API-003 | PUT | /users/1 | Update an existing user with valid data | API should return HTTP 200 OK and the response should contain the updated user information | API returned 200 OK with the updated name, username, email, and ID 1. | PASS
API-004 | DELETE | /users/1 | Delete an existing user | API should return a successful HTTP response and an appropriate response body after deletion | API returned 200 OK with an empty JSON object {}. | PASS
API-005 | GET | /users/9999 | Request a non-existent user | API should return HTTP 404 Not Found for an unavailable resource | API returned 404 Not Found with an empty JSON response {}. | PASS
API-006 | POST | /users | Submit a user creation request with missing required fields | API should reject incomplete user data with an appropriate 4xx validation response | API returned 201 Created and accepted the incomplete payload, returning username and generated ID. | FAIL
API-007 | GET | /users/1 | Validate response structure and required fields | Response should contain the expected user fields with appropriate data types and nested objects | Response contained all expected fields, including id, name, username, email, address, phone, website, and company, with address and company represented as objects. | PASS
API-008 | GET | /users/1 | Validate response Content-Type | Response should have a JSON Content-Type | Response Content-Type was application/json; charset=utf-8. | PASS
