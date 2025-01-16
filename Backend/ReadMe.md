  Backend - Event Management Web App 

Backend - Event Management Web App
==================================

Overview
--------

This is the backend for the Event Management Web App. It is built with Node.js, Express, and MongoDB Atlas. It provides secure authentication using JWT and Bcrypt and supports CRUD operations for managing events. The app’s backend handles user registration, login, and event data storage.

Features
--------

*   **JWT-based Authentication**: Secure user login and registration with JWT and Bcrypt for password hashing.
*   **CRUD Operations**: Create, read, update, and delete events.
*   **MongoDB Atlas Integration**: Data is stored securely on MongoDB Atlas.
*   **Role-based Access Control**: Admin users can manage events, while regular users can view and create events.
*   **Environment Variables**: Configurable for development and production environments with `.env` file.

Technologies Used
-----------------

*   **Node.js**: JavaScript runtime for building the server.
*   **Express.js**: Framework to simplify routing and handling HTTP requests.
*   **MongoDB Atlas**: Cloud-based NoSQL database for storing event and user data.
*   **JWT (JSON Web Tokens)**: Secure token-based authentication for users.
*   **Bcrypt**: Password hashing library for secure storage and verification.

Setup
-----

### Prerequisites

*   Node.js (v14 or higher)
*   npm or yarn
*   MongoDB Atlas account and cluster

### Installation

1.  Clone the repository:
    
        git clone https://github.com/programmeo/Event-Management.git cd backend
    
2.  Install dependencies:
    
        npm install
    
3.  Set up your environment variables:
    *   Create a `.env` file in the root of the backend directory.
    *   Add the following environment variables:
        
            PORT=5000
            MONGO_URI=
            JWT_SECRET=
        
4.  Run the application:
    
        npm start
    
    The server will run on `http://localhost:5000`.

API Endpoints
-------------

### Authentication Routes:

*   **POST \`/api/auth/register\`**: Register a new user.
    
        {
          "username": "exampleUser",
          "email": "user@example.com",
          "password": "yourPassword"
        }
    
*   **POST \`/api/auth/login\`**: Login and receive a JWT token.
    
        {
          "email": "user@example.com",
          "password": "yourPassword"
        }
    

### Event Routes:

*   **GET \`/api/events\`**: Get all events.
    
        [
          {
            "id": "eventId",
            "title": "Event Title",
            "date": "Event Date",
            "description": "Event Description"
          }
        ]
    
*   **POST \`/api/events\`**: Create a new event.
    
        {
          "title": "Event Title",
          "date": "Event Date",
          "description": "Event Description"
        }
    
*   **PUT \`/api/events/:id\`**: Update an existing event.
    
        {
          "title": "Updated Event Title",
          "date": "Updated Event Date",
          "description": "Updated Event Description"
        }
    
*   **DELETE \`/api/events/:id\`**: Delete an event.

Testing
-------

You can test the API using tools like Postman or Insomnia. Make sure to include the `Authorization: Bearer <jwt-token>` header when making requests to protected routes.

Troubleshooting
---------------

*   If the server doesn’t start, ensure that you have set the correct MongoDB URI and JWT secret in the `.env` file.
*   Check for any missing dependencies if you encounter `module not found` errors.

Contributing
------------

Feel free to open issues and submit pull requests to contribute to the development of this project. For major changes, please open an issue first to discuss what you would like to change.

License
-------

This project is licensed under the MIT License.
