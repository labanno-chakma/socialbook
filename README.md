# Student Management System

CRUD application with React JS (Frontend), Spring Boot (Backend), MySQL (Database)

## Project Structure

```
students/
├── backend/          # Spring Boot REST API
├── frontend/         # React JS application
└── database/         # SQL scripts
```

## Prerequisites

- Java 17+
- Maven
- Node.js & npm
- XAMPP (MySQL/phpMyAdmin)

## Setup Instructions

### 1. Database Setup

1. Start Apache and MySQL from XAMPP Control Panel
2. Open phpMyAdmin: http://localhost/phpmyadmin
3. Go to Import tab
4. Import `database/student_management.sql`

### 2. Backend Setup

```bash
cd backend
mvn spring-boot:run
```

Backend runs at: http://localhost:8080

API Endpoints:
- GET    /api/students        - List all students
- GET    /api/students/{id}   - Get student by ID
- POST   /api/students        - Create student
- PUT    /api/students/{id}   - Update student
- DELETE /api/students/{id}   - Delete student

### 3. Frontend Setup

```bash
cd frontend
npm install
npm start
```

Frontend runs at: http://localhost:3000

## Fields

| Field        | Type         | Required |
|-------------|-------------|----------|
| Student ID  | String(20)  | Yes      |
| Name        | String(100) | Yes      |
| Class       | String(50)  | Yes      |
| Mobile      | String(15)  | No       |
| Email       | String(100) | No       |
| Remarks     | Text        | No       |
"# socialbook" 
