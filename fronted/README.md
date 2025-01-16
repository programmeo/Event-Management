<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Frontend - Event Management Web App</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.16/dist/tailwind.min.css" rel="stylesheet">
</head>

<body class="bg-gray-50 text-gray-900">
    <div class="max-w-4xl mx-auto p-6">
        <h1 class="text-4xl font-bold text-center mb-6">Frontend - Event Management Web App</h1>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Overview</h2>
            <p>
                This is the frontend for the Event Management Web App. It is built using React for dynamic rendering,
                TailwindCSS for styling, and React Router DOM for handling navigation. This app communicates with the
                backend API to manage events, handle user authentication, and display event data to users.
            </p>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Features</h2>
            <ul class="list-disc pl-6">
                <li><strong>Dynamic Rendering</strong>: The frontend uses React to dynamically display event data.</li>
                <li><strong>Responsive Design</strong>: TailwindCSS is used to ensure the app is responsive and visually appealing.</li>
                <li><strong>Navigation</strong>: React Router DOM is used to handle page routing for seamless navigation.</li>
                <li><strong>User Authentication</strong>: Login and registration forms communicate with the backend to authenticate users.</li>
                <li><strong>Event Management</strong>: Users can create, update, and view events through the frontend interface.</li>
            </ul>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Technologies Used</h2>
            <ul class="list-disc pl-6">
                <li><strong>React</strong>: JavaScript library for building user interfaces with dynamic rendering.</li>
                <li><strong>React Router DOM</strong>: Library for managing navigation and routing within the app.</li>
                <li><strong>TailwindCSS</strong>: Utility-first CSS framework for building custom, responsive designs.</li>
                <li><strong>Axios</strong>: Used to send HTTP requests to the backend API for event management and user authentication.</li>
            </ul>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Setup</h2>
            <h3 class="text-xl font-medium mb-2">Prerequisites</h3>
            <ul class="list-disc pl-6">
                <li>Node.js (v14 or higher)</li>
                <li>npm or yarn</li>
            </ul>

            <h3 class="text-xl font-medium mt-4 mb-2">Installation</h3>
            <ol class="list-decimal pl-6">
                <li>Clone the repository:
                    <pre><code class="text-sm">git clone https://github.com/programmeo/Event-Management.git cd frontend</code></pre>
                </li>
                <li>Install dependencies:
                    <pre><code class="text-sm">npm install</code></pre>
                </li>
                <li>Run the application:
                    <pre><code class="text-sm">npm start</code></pre>
                    The frontend will run on <code>http://localhost:3000</code>.
                </li>
            </ol>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Components and Routes</h2>

            <h3 class="text-xl font-medium mb-2">Main Pages:</h3>
            <ul class="list-disc pl-6">
                <li><strong>Home Page</strong>: Displays a list of events retrieved from the backend API.</li>
                <li><strong>Event Page</strong>: Displays details of a specific event, including options to update or delete.</li>
                <li><strong>Create Event</strong>: Allows authenticated users to create a new event by submitting a form.</li>
                <li><strong>Login & Register</strong>: Pages for user authentication and registration.</li>
            </ul>

            <h3 class="text-xl font-medium mt-4 mb-2">React Router DOM Routes:</h3>
            <ul class="list-disc pl-6">
                <li><strong>Home Route</strong>: <code>/</code> - Displays the list of all events.</li>
                <li><strong>Event Route</strong>: <code>/events/:id</code> - Displays detailed information about a specific event.</li>
                <li><strong>Create Event Route</strong>: <code>/create</code> - Displays a form for creating a new event.</li>
                <li><strong>Login Route</strong>: <code>/login</code> - Displays a login form.</li>
                <li><strong>Register Route</strong>: <code>/register</code> - Displays a registration form.</li>
            </ul>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Testing</h2>
            <p>To test the frontend, you can simply run the application and interact with the UI. Make sure that the backend API is running and accessible so that all data interactions (like CRUD operations for events and user authentication) work correctly.</p>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Troubleshooting</h2>
            <ul class="list-disc pl-6">
                <li>If the app doesn't display correctly, try clearing the cache or restarting the development server.</li>
                <li>If the frontend cannot reach the backend, make sure the backend server is running and the correct API URLs are used in your Axios requests.</li>
            </ul>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Contributing</h2>
            <p>Feel free to open issues and submit pull requests to contribute to the development of this project. For major changes, please open an issue first to discuss what you would like to change.</p>
        </section>

        <section>
            <h2 class="text-2xl font-semibold mb-4">License</h2>
            <p>This project is licensed under the MIT License.</p>
        </section>
    </div>
</body>

</html>
