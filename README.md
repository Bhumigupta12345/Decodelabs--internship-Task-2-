# 🚀 Synapse API - Task Management REST API

A RESTful Task Management API built using Node.js and Express.js as part of the DecodeLabs Backend API Development Project.

## 📌 Overview

Synapse API is a backend application that allows users to manage tasks through standard CRUD operations. It follows RESTful architecture principles, includes input validation, proper HTTP status codes, and centralized error handling.

## ✨ Features

- Create new tasks
- Retrieve all tasks
- Retrieve a task by ID
- Update existing tasks
- Delete tasks
- Filter tasks by:
  - Completion status
  - Priority level
- Input validation
- Global error handling
- Health check endpoint
- RESTful API design

## 🛠️ Tech Stack

- Node.js
- Express.js
- JavaScript
- REST API
- JSON

## 📂 Project Structure

```bash
synapse-api/
│
├── server.js
├── package.json
│
├── routes/
│   └── tasks.js
│
├── middleware/
│   ├── validate.js
│   └── errorHandler.js
│
└── data/
    └── store.js
```

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/synapse-api.git
cd synapse-api
```

### Install Dependencies

```bash
npm install
```

### Run the Application

```bash
npm start
```

Server will start on:

```bash
http://localhost:3000
```

## 📡 API Endpoints

### Health Check

```http
GET /api/health
```

### Get All Tasks

```http
GET /api/tasks
```

### Get Task By ID

```http
GET /api/tasks/:id
```

### Create Task

```http
POST /api/tasks
```

Request Body:

```json
{
  "title": "Complete project",
  "description": "Finish backend API",
  "priority": "high",
  "completed": false
}
```

### Update Task

```http
PUT /api/tasks/:id
```

### Delete Task

```http
DELETE /api/tasks/:id
```

## 🔍 Query Parameters

Filter tasks by completion status:

```http
GET /api/tasks?completed=true
```

Filter tasks by priority:

```http
GET /api/tasks?priority=high
```

## 📊 HTTP Status Codes

| Code | Description |
|--------|------------|
| 200 | OK |
| 201 | Created |
| 204 | No Content |
| 400 | Bad Request |
| 404 | Not Found |
| 500 | Internal Server Error |

## 🧪 Sample API Response

```json
{
  "status": "success",
  "count": 1,
  "data": [
    {
      "id": 1,
      "title": "Complete project",
      "description": "Finish backend API",
      "priority": "high",
      "completed": false
    }
  ]
}
```

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience with:

- RESTful API Development
- Express.js Routing
- Middleware Implementation
- Input Validation
- Error Handling
- CRUD Operations
- HTTP Methods and Status Codes
- Backend Architecture Design

## 👩‍💻 Author

**Bhumi Gupta**

- GitHub: https://github.com/Bhumigupta12345
  
