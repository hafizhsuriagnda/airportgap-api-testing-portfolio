# AirportGap API Testing Portfolio

This repository contains an API testing portfolio project performed on the public AirportGap API.

## Project Overview

The objective of this project is to design and execute API test scenarios to validate authentication, favorites management, and API response behavior.

---

## API Information

The testing in this project was performed on the public AirportGap API.

**Base URL**

https://airportgap.com/api

**API Documentation**

https://airportgap.com/docs

---

## Test Environment

API Base URL: https://airportgap.com/api  
API Documentation: https://airportgap.com/docs  
Tool: Postman  
Operating System: Windows 10  
Execution Type: Manual API Testing + Postman Collection Runner

---

## Test Strategy

The API testing was designed to validate both functional behavior and error handling of the AirportGap API.

The strategy included:

- Authentication validation
- Authorization validation
- Positive test scenarios for successful operations
- Negative test scenarios for invalid inputs and missing tokens
- Duplicate resource validation
- Response structure validation
- Postman assertions
- Collection Runner

The testing was executed manually using Postman, with additional response validation implemented through Postman test scripts and Collection Runner.

---

## Testing Approach

The API testing included both positive and negative test scenarios:

- Valid authentication
- Invalid authentication
- Missing authorization token
- Invalid authorization token
- Duplicate resource validation
- Invalid request body validation
- Resource retrieval validation
- Response structure validation

---

## API Endpoints Tested

- POST /api/tokens
- GET /api/favorites
- POST /api/favorites
- GET /api/favorites/{id}
- PATCH /api/favorites/{id}
- DELETE /api/favorites/{id}

---

## Test Coverage

Total Test Cases: **15**

Test scenarios include:

- Valid authentication
- Invalid authentication
- Authorization validation
- Favorite airport creation
- Duplicate prevention
- Input validation
- Resource retrieval
- Update operations
- Delete operations
- Response structure validation

---

## Tools Used

- Postman
- Excel
- JSON API

---

## Test Artifacts

This repository contains:

- Test Scenario
- Test Case
- Test Execution
- Test Summary Report
- Test Evidence (screenshots)
- Postman Collections

---

## Test Result

All 15 test cases were executed successfully, with all endpoints returning expected status codes and response structures.

The API demonstrates stable behavior across authentication and favorites management functionalities, with no defects identified within the tested scope.

---

## Repository Structure

```
airportgap-api-testing-portfolio
│
├── Evidence
│   ├── API_Collection_Run_Details.png
│   ├── API_Collection_Run_Summary.png
│   ├── TC_API_01_Login_Success.png
│   ├── TC_API_02_Login_InvalidCredentials.png
│   ├── TC_API_03_Get_Favorites_List.png
│   ├── TC_API_04_Get_Favorites_NoToken.png
│   ├── TC_API_05_Get_Favorites_InvalidToken.png
│   ├── TC_API_06_Create_Favorite_Success.png
│   ├── TC_API_07_Create_Favorite_Duplicate.png
│   ├── TC_API_08_Create_Favorite_InvalidBody.png
│   ├── TC_API_09_Get_Favorite_ByID.png
│   ├── TC_API_10_Get_Favorite_InvalidID.png
│   ├── TC_API_11_Update_Favorite_Note.png
│   ├── TC_API_12_Update_Favorite_InvalidNote.png
│   ├── TC_API_13_Delete_Favorite.png
│   ├── TC_API_14_Delete_Favorite_InvalidID.png
│   └── TC_API_15_Response_Structure.png
├── Test-Documentation
│   ├── airportgap-api-collection-runner.postman_collection
│   └── airportgap-api-manual-testing.postman_collection
├── Test-Documentation
│   └── AirportGap_API_Testing.xlsx
└──  README.md
```
