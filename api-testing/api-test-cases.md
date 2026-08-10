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
