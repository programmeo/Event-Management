  Event Management Web App 

Event Management Web App
========================
![Event-Home](https://github.com/user-attachments/assets/76c39215-4622-4ccf-8f90-cb5cea7943fd)
![Event-Login](https://github.com/user-attachments/assets/0b5fa0fe-2544-416b-866a-9f5e2f188ac3)
![Event-Register](https://github.com/user-attachments/assets/fef807ab-adf0-4636-8756-2163f4fb45a3)


Overview
--------

This is a full-stack Event Management Web App that allows users to manage events, authenticate with secure login functionality, and perform CRUD operations. The backend is built with **Node.js**, **Express**, **JWT**, and **MongoDB Atlas**, while the frontend is built using **React** with **TailwindCSS** for styling and **React Router DOM** for navigation.

Backend
-------

The backend of this application is responsible for user authentication, event management, and data storage. It features JWT-based authentication, password hashing with Bcrypt, and MongoDB Atlas for data persistence.

Key Features:

*   **User Authentication**: Secure login and registration using JWT and Bcrypt.
*   **CRUD Operations**: Create, read, update, and delete events.
*   **MongoDB Atlas Integration**: Store event data and user details in MongoDB Atlas.

For testing purposes, you can use the following dummy credentials to log in:

*   **Username**: `yash@example.com`
*   **Password**: `password123`

Access the backend API here: https://event-management-q3fb.onrender.com

Frontend
--------

The frontend of the Event Management Web App provides a responsive, user-friendly interface built with **React** and styled with **TailwindCSS**. It uses **React Router DOM** for page navigation and Axios to interact with the backend API.

Key Features:

*   **Dynamic Rendering**: The frontend uses React to dynamically display event data.
*   **Responsive Design**: TailwindCSS ensures the app is responsive and visually appealing.
*   **Navigation**: React Router DOM is used for handling page routing and navigation.
*   **User Authentication**: Login and registration forms communicate with the backend to authenticate users.
*   **Event Management**: Users can create, update, and view events through the frontend interface.

Access the frontend here: https://event-management-henna-nine.vercel.app/

Testing
-------

To test the app, you can use the following dummy credentials to log in:

*   **Username**: `yash@example.com`
*   **Password**: `password123`

After logging in, you will be able to test the event management features such as viewing, creating, updating, and deleting events.

License
-------

This project is licensed under the MIT License.
