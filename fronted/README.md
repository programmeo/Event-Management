  Frontend - Event Management Web App 

Frontend - Event Management Web App
===================================

Overview
--------

This is the frontend for the Event Management Web App. It is built using React for dynamic rendering, TailwindCSS for styling, and React Router DOM for handling navigation. This app communicates with the backend API to manage events, handle user authentication, and display event data to users.

Features
--------

*   **Dynamic Rendering**: The frontend uses React to dynamically display event data.
*   **Responsive Design**: TailwindCSS is used to ensure the app is responsive and visually appealing.
*   **Navigation**: React Router DOM is used to handle page routing for seamless navigation.
*   **User Authentication**: Login and registration forms communicate with the backend to authenticate users.
*   **Event Management**: Users can create, update, and view events through the frontend interface.

Technologies Used
-----------------

*   **React**: JavaScript library for building user interfaces with dynamic rendering.
*   **React Router DOM**: Library for managing navigation and routing within the app.
*   **TailwindCSS**: Utility-first CSS framework for building custom, responsive designs.
*   **Axios**: Used to send HTTP requests to the backend API for event management and user authentication.

Setup
-----

### Prerequisites

*   Node.js (v14 or higher)
*   npm or yarn

### Installation

1.  Clone the repository:
    
        git clone https://github.com/programmeo/Event-Management.git cd frontend
    
2.  Install dependencies:
    
        npm install
    
3.  Run the application:
    
        npm start
    
    The frontend will run on `http://localhost:3000`.

Components and Routes
---------------------

### Main Pages:

*   **Home Page**: Displays a list of events retrieved from the backend API.
*   **Event Page**: Displays details of a specific event, including options to update or delete.
*   **Create Event**: Allows authenticated users to create a new event by submitting a form.
*   **Login & Register**: Pages for user authentication and registration.

### React Router DOM Routes:

*   **Home Route**: `/` - Displays the Home Page
*   **Event Route**: `/dashboard` - Displays detailed information about a specific event.
*   **Create Event Route**: `/dashboard` - Displays a form for creating a new event.
*   **Login Route**: `/login` - Displays a login form.
*   **Register Route**: `/register` - Displays a registration form.

Testing
-------

To test the frontend, you can simply run the application and interact with the UI. Make sure that the backend API is running and accessible so that all data interactions (like CRUD operations for events and user authentication) work correctly.

Troubleshooting
---------------

*   If the app doesn't display correctly, try clearing the cache or restarting the development server.
*   If the frontend cannot reach the backend, make sure the backend server is running and the correct API URLs are used in your Axios requests.

Contributing
------------

Feel free to open issues and submit pull requests to contribute to the development of this project. For major changes, please open an issue first to discuss what you would like to change.

License
-------

This project is licensed under the MIT License.
