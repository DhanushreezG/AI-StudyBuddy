# Phase 3: Project Design

## Project Title
AI StudyBuddy API

## 1. Introduction
The design phase describes the architecture, modules, database structure, and API flow of the AI StudyBuddy project.

## 2. System Architecture
The project follows a client-server architecture.

1. Client: Sends API requests using Postman or another application.
2. Express.js Server: Receives requests and routes them to the appropriate controller.
3. Authentication Middleware: Verifies JWT tokens for protected routes.
4. Controllers: Process requests and coordinate application logic.
5. MongoDB: Stores user accounts and study material information.
6. Gemini AI: Generates summaries, flashcards, quizzes, and study plans.

## 3. Main Modules
- Authentication Module: Handles user registration and login.
- User Module: Manages user accounts and roles.
- Materials Module: Uploads, retrieves, and deletes study materials.
- Summary Module: Generates summaries using AI.
- Flashcard Module: Creates flashcards from study materials.
- Quiz Module: Generates quizzes for revision.
- Study Plan Module: Creates personalized study plans.

## 4. Database Design
The project uses MongoDB, a NoSQL database.

### User Collection
Stores user information such as name, email, hashed password, and role.

### Materials Collection
Stores study material details such as title, file information, owner, and uploaded date.

## 5. API Design
| Method | Endpoint | Purpose |
|---|---|---|
| POST | /api/auth/register | Register a user |
| POST | /api/auth/login | Log in a user |
| POST | /api/materials/upload | Upload study material |
| GET | /api/materials | Retrieve materials |
| GET | /api/materials/:id | Retrieve one material |
| DELETE | /api/materials/:id | Delete a material |
| POST | /api/materials/:id/summarize | Generate a summary |
| POST | /api/materials/:id/flashcards | Generate flashcards |
| POST | /api/materials/:id/quiz | Generate a quiz |
| POST | /api/materials/:id/study-plan | Generate a study plan |

## 6. Security Design
- JWT-based authentication protects restricted API routes.
- Passwords are hashed before storage.
- Environment variables store sensitive configuration.
- User access is controlled according to authentication and permissions.

## 7. Technology Design
- Node.js: JavaScript runtime.
- Express.js: Backend framework.
- MongoDB and Mongoose: Database and data modeling.
- JWT: Authentication.
- Google Gemini AI: AI-generated learning content.

## 8. Conclusion
The design phase defines the structure and interaction of the main components of the AI StudyBuddy API.