# User Authentication System

This project implements a simple user authentication system using **Express** (Node.js) and **MongoDB**. Users can register and log in by submitting data via JSON requests.

## Features
- User registration with password hashing (bcrypt)
- User login with JWT-based authentication
- JSON request and response handling
- MongoDB database to store user credentials

## Technologies Used
- Node.js
- Express.js
- MongoDB
- Mongoose
- bcrypt.js
- JWT (JSON Web Token)
- HTML, CSS, and JavaScript for frontend

## Setup Instructions

### Prerequisites

- **Node.js** installed (v14 or higher)
- **MongoDB** instance running locally or in the cloud (e.g., MongoDB Atlas)
- **npm** (Node Package Manager)
### 1. Clone the repository

git clone https://github.com/your-username/user-authentication-system.git
cd user-authentication-system


### 2. Install Dependencies

npm install


### 3. Set up environment variables

MONGO_URI=your_mongo_database_uri
JWT_SECRET=your_jwt_secret_key

### 4. Run the application

node server.js

### 5. Access the aplication
You can access the application in your browser:

Registration page: http://localhost:3000/register.html
Login page: http://localhost:3000/login.html


## Project Structure
. ├── public/ │ ├── register.html # Registration form │ ├── login.html # Login form │ └── styles.css # CSS for the frontend ├── .env # Environment variables ├── node_modules/ # Installed Node modules ├── server.js # Main server file ├── package.json # Project dependencies and scripts └── README.md # Project documentation
## How It Works
User Registration: The registration page collects a username, email, and password from the user. The password is hashed using bcrypt, and the user is stored in the MongoDB database.

User Login: The login page collects the email and password from the user. If the credentials match an existing user in the database, a JWT token is generated and sent back to the user.

JWT Authentication: The token is stored client-side and can be used to authenticate further requests to protected routes (in the future).







