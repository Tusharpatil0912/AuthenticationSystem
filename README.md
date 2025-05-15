
---

## Frontend

The frontend is built using React and includes features like routing, authentication, and responsive design.

### Scripts:
- `npm start`: Runs the app in development mode.
- `npm test`: Launches the test runner.
- `npm run build`: Builds the app for production.

#### Open the app in your browser at
  http://localhost:3000
  
---

# Backend

The backend is built using Node.js and Express, with MongoDB as the database.

## Scripts:
- `npm start`: Starts the server using `nodemon`.

---

## API Documentation

This document provides details about the API endpoints available in the backend of the authentication system.

### Base URL

The base URL for the API is: http://localhost:8000/auth

### Endpoints:

1. **User Signup**
   **Endpoint:** `/api/auth/signup`  
   **Method:** `POST`  
   **Description:** Registers a new user.  

**Request Body:**
```json
{
  "name": "string",
  "email": "string",
  "password": "string"
} 

    Response:
    201 Created

    {
    "message": "Signup successfully",
    "success": true
    }

2. **User Login**
Endpoint: /login
Method: POST
Description: Authenticates a user and returns a JWT token.

**Request Body:**
```json
{
  "email": "string",
  "password": "string"
} 

Response: 200 OK

{
    "message": "Login Success",
    "success": true,
    "jwtToken": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiY0BnbWFpbC5jb20iLCJfaWQiOiI2ODI1YTdhZjczYzEzMDBhNGJjNGY1NzciLCJpYXQiOjE3NDcyOTgzNjAsImV4cCI6MTc0NzM4NDc2MH0.7Bl560H4b_SLH8Od8VEIsRNHJ31jC1i3qaPdDp_27DI",
    "email": "abc@gmail.com",
    "name": "Tushar"
}
---

## Deployment

- **Frontend**: Configured for deployment on Vercel.
- **Backend**: Configured for deployment on Vercel.

---

## Environment Variables

Both the frontend and backend use `.env` files to store environment-specific variables.

### Backend:
- `PORT`: Port number for the server.
- `MONGO_CONNECTION_STRING`: MongoDB connection string.
- `JWT_SECRET`: Secret key for JWT.

### Frontend:


---

## 1.. How to Run Locally

1. Clone the repository:

   git clone <repository-url>

## 2.. Navigate to the frontend and backend folders and install dependencies:
cd frontend
npm install
cd ../backend
npm install

## 3.. Start the backend server:
npm start