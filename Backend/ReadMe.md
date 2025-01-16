<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Backend - Event Management Web App</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.16/dist/tailwind.min.css" rel="stylesheet">
</head>

<body class="bg-gray-50 text-gray-900">
    <div class="max-w-4xl mx-auto p-6">
        <h1 class="text-4xl font-bold text-center mb-6">Backend - Event Management Web App</h1>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Overview</h2>
            <p>
                This is the backend for the Event Management Web App. It is built with Node.js, Express, and MongoDB Atlas.
                It provides secure authentication using JWT and Bcrypt and supports CRUD operations for managing events.
                The app’s backend handles user registration, login, and event data storage.
            </p>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Features</h2>
            <ul class="list-disc pl-6">
                <li><strong>JWT-based Authentication</strong>: Secure user login and registration with JWT and Bcrypt for password hashing.</li>
                <li><strong>CRUD Operations</strong>: Create, read, update, and delete events.</li>
                <li><strong>MongoDB Atlas Integration</strong>: Data is stored securely on MongoDB Atlas.</li>
                <li><strong>Role-based Access Control</strong>: Admin users can manage events, while regular users can view and create events.</li>
                <li><strong>Environment Variables</strong>: Configurable for development and production environments with <code>.env</code> file.</li>
            </ul>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Technologies Used</h2>
            <ul class="list-disc pl-6">
                <li><strong>Node.js</strong>: JavaScript runtime for building the server.</li>
                <li><strong>Express.js</strong>: Framework to simplify routing and handling HTTP requests.</li>
                <li><strong>MongoDB Atlas</strong>: Cloud-based NoSQL database for storing event and user data.</li>
                <li><strong>JWT (JSON Web Tokens)</strong>: Secure token-based authentication for users.</li>
                <li><strong>Bcrypt</strong>: Password hashing library for secure storage and verification.</li>
            </ul>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Setup</h2>
            <h3 class="text-xl font-medium mb-2">Prerequisites</h3>
            <ul class="list-disc pl-6">
                <li>Node.js (v14 or higher)</li>
                <li>npm or yarn</li>
                <li>MongoDB Atlas account and cluster</li>
            </ul>

            <h3 class="text-xl font-medium mt-4 mb-2">Installation</h3>
            <ol class="list-decimal pl-6">
                <li>Clone the repository:
                    <pre><code class="text-sm">git clone https://github.com/programmeo/Event-Management.git cd backend</code></pre>
                </li>
                <li>Install dependencies:
                    <pre><code class="text-sm">npm install</code></pre>
                </li>
                <li>Set up your environment variables:
                    <ul class="list-inside">
                        <li>Create a <code>.env</code> file in the root of the backend directory.</li>
                        <li>Add the following environment variables:
                            <pre><code class="text-sm">PORT=5000
MONGO_URI=<your-mongodb-atlas-connection-string>
JWT_SECRET=<your-jwt-secret-key></code></pre>
                        </li>
                    </ul>
                </li>
                <li>Run the application:
                    <pre><code class="text-sm">npm start</code></pre>
                    The server will run on <code>http://localhost:5000</code>.
                </li>
            </ol>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">API Endpoints</h2>

            <h3 class="text-xl font-medium mb-2">Authentication Routes:</h3>
            <ul class="list-disc pl-6">
                <li><strong>POST `/api/auth/register`</strong>: Register a new user.
                    <pre><code class="text-sm">{
  "username": "exampleUser",
  "email": "user@example.com",
  "password": "yourPassword"
}</code></pre>
                </li>
                <li><strong>POST `/api/auth/login`</strong>: Login and receive a JWT token.
                    <pre><code class="text-sm">{
  "email": "user@example.com",
  "password": "yourPassword"
}</code></pre>
                </li>
            </ul>

            <h3 class="text-xl font-medium mb-2">Event Routes:</h3>
            <ul class="list-disc pl-6">
                <li><strong>GET `/api/events`</strong>: Get all events.
                    <pre><code class="text-sm">[
  {
    "id": "eventId",
    "title": "Event Title",
    "date": "Event Date",
    "description": "Event Description"
  }
]</code></pre>
                </li>
                <li><strong>POST `/api/events`</strong>: Create a new event.
                    <pre><code class="text-sm">{
  "title": "Event Title",
  "date": "Event Date",
  "description": "Event Description"
}</code></pre>
                </li>
                <li><strong>PUT `/api/events/:id`</strong>: Update an existing event.
                    <pre><code class="text-sm">{
  "title": "Updated Event Title",
  "date": "Updated Event Date",
  "description": "Updated Event Description"
}</code></pre>
                </li>
                <li><strong>DELETE `/api/events/:id`</strong>: Delete an event.</li>
            </ul>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Testing</h2>
            <p>You can test the API using tools like Postman or Insomnia. Make sure to include the <code>Authorization: Bearer &lt;jwt-token&gt;</code> header when making requests to protected routes.</p>
        </section>

        <section class="mb-6">
            <h2 class="text-2xl font-semibold mb-4">Troubleshooting</h2>
            <ul class="list-disc pl-6">
                <li>If the server doesn’t start, ensure that you have set the correct MongoDB URI and JWT secret in the <code>.env</code> file.</li>
                <li>Check for any missing dependencies if you encounter <code>module not found</code> errors.</li>
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
