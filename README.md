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

3.Run the application

4.Access the application at http://localhost:8080

** Use Postman for endpoint testing
## Usage

- Register a new user: `http://localhost:8080/api/v1/auth/register`
  sample data (POST): 
  {
    "firstname": "mohammad",
    "lastname": "alabed",
    "email": "mohammad@gmail.com",
    "password": "1234"
  } the response is your jwt

- Login with existing user credentials: `http://localhost:8080/api/v1/auth/authenticate`
  sample data (POST): 
  {
    "email": "mohammad@gmail.com",
    "password": "1234"
  } also the response is your jwt
  
- Access protected resources with JWT: Include the JWT in the Authorization header as `Bearer token` using get method
  http://localhost:8080/api/v1/demo-controller
  
