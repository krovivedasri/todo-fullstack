**Todo Application - Full Stack**
A complete full-stack todo application built with React, Spring Boot, and PostgreSQL.

---Features---

Create new todos with title and description
Mark todos as complete/incomplete
Edit todo inline
Delete todos
Filter todos (All/Active/Completed)
Responsive and modern UI
REST API backend
PostgreSQL database persistence

--Prerequisites--
Before running this application, make sure you have:

Java 17+ installed
Maven installed
Node.js 16+ and npm installed
PostgreSQL installed and running on port 5433
A database named todo created in PostgreSQL

---Database Setup---
Make sure PostgreSQL is running
Create the database:
CREATE DATABASE todo;
The application will automatically create the required tables on first run.

----Backend Setup (Spring Boot)---
Navigate to the backend directory:
cd backend
Run the Spring Boot application:
mvnw spring-boot:run
Or on Windows:

mvnw.cmd spring-boot:run
The backend will start on http://localhost:8080

Backend API Endpoints
POST /api/todos - Create a new todo
GET /api/todos - Get all todos
GET /api/todos?completed=true - Get completed todos
GET /api/todos?completed=false - Get active todos
PUT /api/todos/{id} - Update a todo
DELETE /api/todos/{id} - Delete a todo

---Frontend Setup (React)----
Navigate to the frontend directory:
cd frontend
Install dependencies:
npm install
Start the development server:
npm start
The frontend will start on http://localhost:3000

---Usage----
Start the backend server (port 8080)
Start the frontend server (port 3000)
Open your browser and navigate to http://localhost:3000
Start managing your todos!
----Project Structure----
todo/
├── backend/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/todo/
│   │   │   │   ├── controller/
│   │   │   │   ├── model/
│   │   │   │   ├── repository/
│   │   │   │   ├── service/
│   │   │   │   └── exception/
│   │   │   └── resources/
│   │   │       └── application.properties
│   └── pom.xml
│
└── frontend/
    ├── public/
    ├── src/
    │   ├── components/
    │   │   ├── AddTodo.jsx
    │   │   ├── TodoList.jsx
    │   │   └── TodoItem.jsx
    │   ├── services/
    │   │   └── todoService.js
    │   └── App.jsx
    └── package.json



---Technology Stack----
Backend:

Spring Boot 3.2.2
Spring Data JPA
PostgreSQL
Maven
Frontend:

React 18
Axios
CSS3

---License---
This project is open source and available for educational purposes.
