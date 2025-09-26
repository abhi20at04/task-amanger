📋 Task Manager System

A full-stack Task Manager application built with React (frontend), Node.js/Express (backend), and MongoDB (database).
This app allows users to register, login, and manage their tasks with due dates.
The backend is secured with JWT authentication, and MongoDB Compass can be used to inspect stored data.

✨ Features
🔐 User Authentication

📝 Signup with email & password

🔑 Login securely with JWT tokens

🛡️ Protected APIs accessible only by authenticated users

✅ Task Management

➕ Add new todos with due dates

📃 View todo list specific to logged-in user

❌ Delete todos individually

🎨 Frontend

⚛️ Built with React + Vite

📱 Responsive UI styled with Bootstrap

🧩 Components for Login, Signup, Entertodo, Todoitems, and Welcome messages

🌐 Uses React Context API for global auth state

⚙️ Backend

🌍 RESTful API using Express.js

🗄️ MongoDB with Mongoose

🔒 Secure password hashing with bcrypt

🎟️ JWT-based authentication middleware

🗃️ Database

👤 MongoDB collection for users

📝 MongoDB collection for todos

🖥️ View/manage data using MongoDB Compass

🛠️ Technologies Used

Frontend: React, Bootstrap, React Icons, Axios
Backend: Node.js, Express, Mongoose, bcrypt, jsonwebtoken
Database: MongoDB, MongoDB Compass
Authentication: JWT tokens
Other Tools: Vite, Postman

🚀 Getting Started
📋 Prerequisites

Node.js & npm installed

MongoDB server running (local or Atlas)

MongoDB Compass (optional, for database inspection)

🖥️ Backend Setup
# clone repo and go to backend folder
cd backend
npm install

# create .env file
JWT_SECRET=your_jwt_secret
MONGO_URI=your_mongodb_connection_string

# run backend
npm start

🎨 Frontend Setup
cd frontend
npm install
npm run dev

🧑‍💻 Usage

📝 Register a new account (Signup page)

🔑 Login with your credentials

➕ Add todos with name + due date

📃 View & ❌ delete todos

🖥️ Use MongoDB Compass to inspect collections

🔗 API Endpoints

POST /api/auth/signup → User registration

POST /api/auth/login → User login + token issuance

GET /api/todos → Get user’s todos (auth required)

POST /api/todos → Add new todo (auth required)

DELETE /api/todos/:id → Delete todo by ID (auth required)

📝 Special Notes

🔒 Passwords hashed using bcrypt

⏳ JWT tokens expire in 1 hour

⚠️ UI provides feedback on errors (login failure, duplicate signup, etc.)

📡 Axios attaches JWT token in auth headers

🚪 Token cleared on logout

🛠️ Meant for local dev (deployment steps can be added)

🤝 Contributing

💡 PRs are welcome for features, bug fixes, or enhancements.
📑 Follow proper commit conventions & document changes.

📜 License

This project is provided as-is for learning & development purposes.
