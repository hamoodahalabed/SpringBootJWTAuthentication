# Spring Boot JWT Authentication

This is a sample Spring Boot project that demonstrates JWT (JSON Web Token) authentication using Spring Security.

## Features

- User registration
- User login
- JWT generation and validation

## Technologies Used

- Spring Boot
- Spring Security
- JSON Web Tokens (JWT)
- Hibernate
- PostgreSQL

## Setup

1. Clone the repository: git clone `https://github.com/hamoodahalabed/SpringBootJWTAuthentication.git`

2. Configure your database settings in `application.properties` or `application.yml`:

3. Run the application

4. Access the application at http://localhost:8080

** Use Postman for endpoint testing
## Usage

- Register a new user: `http://localhost:8080/api/v1/auth/register`
  sample data (POST):
  
  <pre>
  {
    "firstName": "mohammad",
    "lastName": "alabed",
    "email": "mohammad@gmail.com",
    "password": "1234"
  } 
    ** The response should be your jwt
</pre>

- Login with existing user credentials: `http://localhost:8080/api/v1/auth/authenticate`
  sample data (POST):
  
  <pre>
  {
    "email": "mohammad@gmail.com",
    "password": "1234"
  } 
    **Also the response should be your jwt
  </pre>
  
- Access protected resources with JWT: Include the JWT in the Authorization header as `Bearer token` using get method
  `http://localhost:8080/api/v1/demo-controller`
  
