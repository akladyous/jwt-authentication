# JWT Authentication - Full Stack Application

![JWT Authentication](./jwt-authentication.webp)

## Introduction

This is a **full-stack authentication project** built from the ground up using **plain JavaScript** and modern web technologies. The project implements a complete, secure, and efficient authentication solution entirely from scratch, demonstrating best practices for building production-ready authentication systems.

### Project Overview

This application provides a comprehensive authentication system featuring:

-   **User Registration** - Secure signup with validation
-   **User Login** - JWT-based authentication with refresh tokens
-   **Session Management** - Secure token storage and refresh mechanisms
-   **Protected Routes** - Route protection on both frontend and backend
-   **User State Management** - Centralized state management using Redux
-   **Security Best Practices** - Password hashing, token validation, CORS configuration, and secure cookie handling

### Technology Stack

#### Backend

-   **Express.js** - Web application framework for Node.js
-   **MongoDB** with **Mongoose** - Database and ODM for data modeling
-   **JSON Web Tokens (JWT)** - Secure token-based authentication
-   **bcrypt** - Password hashing and encryption
-   **cookie-parser** - Cookie parsing middleware
-   **CORS** - Cross-Origin Resource Sharing configuration
-   **validator** - Input validation and sanitization
-   **dotenv** - Environment variable management
-   **Babel** - JavaScript compiler for modern ES6+ syntax

#### Frontend

-   **React** - UI library for building user interfaces
-   **Redux Toolkit** - State management library
-   **React Router** - Client-side routing
-   **Axios** - HTTP client for API requests
-   **React Redux** - React bindings for Redux

### Key Features

-   ✅ **Complete Authentication Flow** - Signup, login, logout, and session management
-   ✅ **JWT Token Management** - Access tokens and refresh tokens with automatic renewal
-   ✅ **Secure Password Handling** - Bcrypt hashing with salt rounds
-   ✅ **Protected Routes** - Both client-side and server-side route protection
-   ✅ **State Management** - Centralized user and token state with Redux
-   ✅ **Error Handling** - Comprehensive error handling and user feedback
-   ✅ **CORS Configuration** - Secure cross-origin requests
-   ✅ **Session Persistence** - Token storage in HTTP-only cookies and localStorage
-   ✅ **Input Validation** - Server-side validation using validator library
-   ✅ **Modern JavaScript** - ES6+ syntax with Babel transpilation

### Project Structure

```
jwt-authentication-express.js-react-redux/
├── backend/          # Express.js server
│   ├── config/      # Database, CORS, environment configuration
│   ├── controller/  # Request handlers (signup, signin, signout)
│   ├── middleware/  # Authentication, error handling, CORS middleware
│   ├── models/      # MongoDB models (Users, Sessions)
│   ├── routes/      # API route definitions
│   └── util/        # Utility functions (auth helpers, error classes)
└── frontend/        # React application
    ├── src/
    │   ├── api/     # Axios configuration
    │   ├── auth/    # Authentication hooks and listeners
    │   ├── features/ # Redux slices and thunks
    │   ├── store/   # Redux store configuration
    │   ├── ui/      # React components
    │   └── users/   # User-related components
```

## Getting Started

### Prerequisites

-   Node.js (v14 or higher)
-   MongoDB (local or cloud instance)
-   npm or yarn

### Installation

1. Clone the repository:

```bash
git clone https://github.com/akladyous/jwt-authentication-express.js-react-redux.git
cd jwt-authentication-express.js-react-redux
```

2. Install backend dependencies:

```bash
cd backend
npm install
```

3. Install frontend dependencies:

```bash
cd ../frontend
npm install
```

4. Configure environment variables:

    - Create a `.env` file in the `backend` directory
    - Add your MongoDB connection string, JWT secrets, and other configuration

5. Start the backend server:

```bash
cd backend
npm run dev
```

6. Start the frontend development server:

```bash
cd frontend
npm start
```

The application will be available at `http://localhost:3000` (frontend) and your configured backend port.

## Security Features

This project implements multiple layers of security:

-   **Password Encryption** - Passwords are hashed using bcrypt before storage
-   **JWT Tokens** - Secure token-based authentication with expiration
-   **Refresh Tokens** - Automatic token refresh mechanism
-   **HTTP-Only Cookies** - Secure cookie storage for tokens
-   **CORS Protection** - Configured CORS policies
-   **Input Validation** - Server-side validation to prevent malicious input
-   **Route Protection** - Middleware-based route protection
-   **Error Handling** - Secure error messages without exposing sensitive information

## License

MIT License - see LICENSE file for details

## Author

Boula Akladyous

## Contributing

Contributions, issues, and feature requests are welcome!
