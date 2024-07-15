MERN Todo Web Application
This project implements a web-based Todo application using the MERN stack (MongoDB, Express, React, Node.js). The app allows users to create, read, update, and delete todo items, helping them manage their tasks efficiently.

Table of Contents
Introduction
Features
Installation
Usage
API Endpoints
Project Structure
Introduction
The MERN Todo Web Application is designed to help users manage their daily tasks. With a simple and intuitive interface, users can easily add, update, delete, and mark tasks as complete. The application uses MongoDB for data storage, Express and Node.js for the backend, and React for the frontend.

Features
Add new todo items
Update existing todo items
Delete todo items
Mark todo items as complete or incomplete
User authentication and profile management
Installation
Clone the repository:
git clone https://github.com/Chukwuskindall/todo-app-web.git
cd mern-todo-web
Install backend dependencies:
cd server
npm install
Install frontend dependencies:
cd ../client
npm install
Set up environment variables:
Create a .env file in the server directory and add your environment variables:

MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
Run the application:
Backend:
cd server
npm start
The backend server will start on http://localhost:5000.

Frontend:
cd ../client
npm start
The frontend will start on http://localhost:3000.

Usage
Open your web browser and navigate to http://localhost:3000.
Sign up or log in to your account.
Add new tasks using the input field.
Update or delete tasks by clicking the respective buttons next to each task.
Mark tasks as complete or incomplete by clicking the checkbox.
API Endpoints
Todos
GET /api/todos: Retrieve all todos
POST /api/todos: Create a new todo
PUT /api/todos/:id: Update an existing todo
DELETE /api/todos/:id: Delete a todo
Users
POST /api/users/signup: Sign up a new user
POST /api/users/login: Log in a user
GET /api/users/profile: Retrieve user profile (authenticated users only)
Project Structure
mern-todo-web/
│
├── server/                  # Backend code (Node.js, Express, MongoDB)
│   ├── controllers/         # Controller files for handling requests
│   ├── models/              # Database models
│   ├── routes/              # Route definitions
│   ├── middlewares/         # Middleware functions
│   ├── config/              # Configuration files
│   ├── .env                 # Environment variables
│   ├── server.js            # Main server file
│   └── package.json         # Backend dependencies
│
├── client/                  # Frontend code (React)
│   ├── public/              # Public files
│   ├── src/                 # Source files
│   │   ├── components/      # Reusable React components
│   │   ├── pages/           # React pages
│   │   ├── App.js           # Main React component
│   │   ├── index.js         # Entry point for React
│   └── package.json         # Frontend dependencies
│
└── README.md                # Project README file
