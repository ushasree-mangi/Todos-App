# Todo Web Application

## Overview

This is a full-stack Todo Web Application that allows users to manage their daily tasks efficiently. Users can register, log in, and perform CRUD operations on their tasks, as well as update their profile information. The application ensures user data security through JWT-based authentication.

## Technologies Used

- **Frontend**: ReactJS
- **Backend**: Node.js, Express.js
- **Database**: SQLite
- **Authentication**: JWT (JSON Web Token)
- **Unique ID Generation**: UUID

## Features

### User Authentication

- **Signup**: Users can register by providing their name, email, and password.
- **Login**: Registered users can log in using their email and password.
- **JWT Authentication**: Secures routes by validating tokens to ensure only authenticated users can access them.

### Todo Management

- **Create**: Users can add new tasks with a title and description.
- **Read**: Users can view their list of tasks.
- **Update**: Users can edit existing tasks.
- **Delete**: Users can remove tasks they no longer need.
- **Status Update**: Users can set the status of tasks to "done," "pending," "in progress," or "completed."

### User Profile Management

- **View Profile**: Users can view their profile information.
- **Update Profile**: Users can update their name, email, and password.
- **Profile Security**: Profile updates are restricted to authenticated users only.

## Installation and Setup

### Prerequisites

- Node.js
- npm (Node Package Manager)
- SQLite3 or MongoDB

### Steps to Run the Application

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/Todo-App.git
   cd Todo-App
   ```

2. **Install Dependencies**

   ```bash
   # Navigate to the backend folder
   cd backend
   npm install

   # Navigate to the frontend folder
   cd ../frontend
   npm install
   ```

3. **Configure Environment Variables**
   Create a `.env` file in the backend directory and add the following:

   ```env
   PORT=5000
   JWT_SECRET=your_jwt_secret_key
   DATABASE_URL=path_to_your_database (for SQLite3)
   ```

4. **Run the Backend Server**

   ```bash
   cd backend
   npm start
   ```

5. **Run the Frontend Application**

   ```bash
   cd frontend
   npm start
   ```

## API Endpoints

### Authentication Routes

- **POST /register**: Register a new user.
- **POST /login**: Authenticate user and return JWT.

### Task Management Routes (Protected)

- **GET /tasks**: Retrieve all tasks for the authenticated user.
- **POST /tasks**: Create a new task.
- **PUT /tasks/**: Update an existing task.
- **DELETE /tasks/**: Delete a task.

### Profile Management Routes (Protected)

- **GET /profile**: Retrieve user profile information.
- **PUT /profile**: Update user profile information.

## Folder Structure

```
Todo-App/
|-- backend/
|   |-- controllers/
|   |-- models/
|   |-- routes/
|   |-- server.js
|   |-- .env
|-- frontend/
|   |-- src/
|   |-- public/
|   |-- package.json
|-- README.md
```

## Security Measures

- **Password Hashing**: User passwords are hashed using `bcrypt` for security.
- **JWT Tokens**: Used to secure API routes and protect user data.
- **CORS**: Configured to allow cross-origin resource sharing.

## Future Enhancements

- Implementing task categorization.
- Adding task reminders and notifications.
- Enhancing UI/UX for a better user experience.

## License

This project is licensed under the MIT License.

---



For any questions or issues, please contact [[ushasree2022@gmail.com](mailto\:your-email@example.com)].



 
