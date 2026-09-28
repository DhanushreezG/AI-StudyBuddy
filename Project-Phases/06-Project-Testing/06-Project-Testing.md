# Phase 6: Project Testing

## Project Title
AI StudyBuddy API

## 1. Introduction
Testing verifies that the AI StudyBuddy API functions correctly and that its features respond as expected.

## 2. Testing Objectives
- Verify user registration and login.
- Check authentication and access control.
- Test study material upload and retrieval.
- Verify AI-powered features.
- Identify and fix errors.

## 3. Testing Environment
- Node.js and Express.js backend.
- MongoDB Atlas database.
- Postman API testing tool.
- Google Gemini AI integration.

## 4. Test Cases

| Test Case | Functionality | Expected Result |
|---|---|---|
| TC01 | User registration | User account is created successfully. |
| TC02 | User login | Valid credentials return an authentication token. |
| TC03 | Access without token | Protected endpoint rejects the request. |
| TC04 | Upload study material | Material is uploaded successfully. |
| TC05 | Retrieve materials | Material list is returned. |
| TC06 | Get material by ID | Requested material is returned. |
| TC07 | Generate summary | AI-generated summary is returned. |
| TC08 | Generate flashcards | Flashcards are returned. |
| TC09 | Generate quiz | Quiz questions are returned. |
| TC10 | Generate study plan | Study plan is returned. |
| TC11 | Delete material | Material is deleted successfully. |

## 5. Testing Methods
- Functional Testing: Checks whether each API feature works correctly.
- Authentication Testing: Verifies access control.
- Integration Testing: Checks communication between the API, database, and AI service.
- Error Testing: Checks how the API handles invalid requests and failures.

## 6. Testing Tools
- Postman for sending API requests.
- MongoDB Atlas for checking stored data.
- VS Code terminal for monitoring server output.

## 7. Test Results
The main API features were tested during development. Registration, login, material management, summary generation, flashcard generation, quiz generation, and study plan generation were verified.

## 8. Conclusion
The testing phase verifies the main functions of the AI StudyBuddy API and helps identify issues before demonstration and submission.