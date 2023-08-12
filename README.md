Login and Signup REST API with Security and JWT Authentication

This project implements a backend REST API for user login and signup functionality with security features and JSON Web Token (JWT) authentication. Users can securely create accounts, log in, and access protected resources using JWT tokens. The project is built on the Spring Boot framework and utilizes an H2 database.

Prerequisites:

Before you begin, ensure you have the following prerequisites:
- Java Development Kit (JDK) 8 or later
- Apache Maven
- Git

Installation and Setup:

1. Clone the repository:
   git clone https://github.com/your-username/your-project.git
   cd your-project

2. Build and run the application:
   mvn spring-boot:run

3. The application will start on http://localhost:8080.

Endpoints:

Signup
- Endpoint: POST /signup
- Request Body: JSON object containing user details (e.g., username, password)
- Creates a new user account securely in the database.

Login
- Endpoint: POST /login
- Request Body: JSON object containing user credentials (e.g., username, password)
- Returns a JWT token upon successful authentication.

Hello
- Endpoint: GET /hello
- Requires Authorization header with a valid JWT token.
- Returns a "Hello from GreenStitch" message.

Security and Web Tokens:

- User passwords are securely hashed before storage.
- JSON Web Tokens (JWT) are used for authentication and authorization.
- Spring Security is configured to protect resources and handle authentication.

Database:

- The H2 database is used for storing user account information securely.
- The database schema is designed to store user details.

Testing:

1. Run tests:
   mvn test

Contributing:

Contributions are welcome! If you find any issues or want to enhance the project, feel free to open a pull request.

License:

This project is licensed under the MIT License. See the LICENSE file for details.