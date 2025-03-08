# MERN Authentication Server

This is the backend server for a MERN stack authentication system, offering secure APIs for user registration, login, and authentication. Built with Node.js, Express, and MongoDB, it ensures robust user management with JWT-based authentication and password hashing for enhanced security.

## Features

- User registration
- User login
- Token-based authentication
- Password hashing
- User logout

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Tokens (JWT)
- bcrypt.js

## Getting Started

### Prerequisites

- Node.js installed
- MongoDB installed and running

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/Authentication-Backend.git
2. Navigate to the server directory:
    ```bash
    cd Authentication-Backend
    ```
3. Install dependencies:
    ```bash
    npm install
    ```

### Configuration

1. Create a `.env` file in the root of the server directory and add the following environment variables:
    ```env
    PORT=5000
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    EMAIL_SERVICE=your_email_service_provider
    EMAIL_USERNAME=your_email_username
    EMAIL_PASSWORD=your_email_password
    ```
    
2. Refer to the `.env` file in your code to access these variables:
    ```javascript
    require('dotenv').config();
    const port = process.env.PORT;
    const mongoUri = process.env.MONGO_URI;
    const jwtSecret = process.env.JWT_SECRET;
    const emailService = process.env.EMAIL_SERVICE;
    const emailUsername = process.env.EMAIL_USERNAME;
    const emailPassword = process.env.EMAIL_PASSWORD;
    ```

### Running the Server

Start the server:
```bash
npm start
```

The server will be running on `http://localhost:5000`.

## API Endpoints

- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login a user
- `GET /api/auth/user` - Get authenticated user details
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login a user
- `GET /api/auth/user` - Get authenticated user details
- `POST /api/auth/logout` - Logout a user
- `POST /api/auth/refresh-token` - Refresh authentication token

## License

This project is licensed under the MIT License.