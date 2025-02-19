API Documentation
Authentication Routes:
POST /api/auth/register: Register a new student.
POST /api/auth/login: Login with username and password.
GET /api/auth/logout: Logout a user.
Course Management (Admin Routes):
GET /api/courses: Get a list of all courses.
GET /api/courses/:id: Get details of a specific course by ID.
POST /api/courses: Create a new course (Admin only).
PUT /api/courses/:id: Update an existing course (Admin only).
DELETE /api/courses/:id: Delete a course (Admin only).
Student Management (Admin Routes):
GET /api/students: Get a list of all students.
GET /api/students/:id: Get details of a specific student by ID.
POST /api/students: Create a new student (Admin only).
PUT /api/students/:id: Update a student's information (Admin only).
DELETE /api/students/:id: Delete a student (Admin only).
Enrollment Management (Admin Routes):
GET /api/enrollments: Get a list of all enrollments.
POST /api/enrollments: Create a new enrollment (Admin only).
PUT /api/enrollments/:id: Update an enrollment (Admin only).
DELETE /api/enrollments/:id: Delete an enrollment (Admin only).


# Online Learning Platform

This is the backend for an **Online Learning Platform**. The system allows students to register, log in, view available courses, and enroll in them. Admins can manage courses, students, and enrollments.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [API Documentation](#api-documentation)
- [Run the Project](#run-the-project)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project is a full-stack web application built with Node.js, Express.js for the backend, and React.js for the frontend. It includes features for user authentication, course management, student management, and enrollment management. The backend connects to a relational database (PostgreSQL) for storing user, course, and enrollment data.

## Technologies Used

- **Backend**:
  - Node.js
  - Express.js
  - PostgreSQL (Database)
  - Sequelize (ORM)
  - JWT (Authentication)
  - Bcrypt.js (Password Hashing)
  - CORS (Cross-Origin Resource Sharing)
  - Dotenv (Environment Variables)
  - Morgan (Request Logger)
  - Nodemon (Development Server)

- **Frontend** (if applicable):
  - React.js (for a compelling user interface)

## Features

### User (Student) Features:
- User registration, login, and logout
- View available courses
- Enroll in courses

### Admin Features:
- Manage (CRUD) courses
- Manage (CRUD) student information
- Manage (CRUD) student enrollments

### Authentication:
- JWT authentication and authorization
- Role-based access control (Admin vs. Student)

## Installation

### Backend Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/online-learning-platform.git
