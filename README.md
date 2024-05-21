# flask-docker-starter

Flask Docker Starter is a template project for quickly setting up a Dockerized Flask application with PostgreSQL as the database. This starter kit simplifies the process of containerizing your Flask application, enabling easy deployment and scalability. The project includes essential configurations and instructions for getting started with Docker and Docker Compose, making it an ideal starting point for developing Flask applications with a robust database backend.

## Features:

- **Flask Framework**: A lightweight WSGI web application framework in Python.
- **PostgreSQL Database**: A powerful, open-source object-relational database system.
- **Docker and Docker Compose**: Simplifies container management and orchestration.
- **User Registration**: Example implementation of user registration and retrieval functionality.
- **Environment Variable Management**: Secure and flexible configuration of database credentials.
- **Volume Management**: Ensures data persistence across container restarts.

## Getting Started

### Clone the Repository:

```sh
git clone https://github.com/srmandli95/flask-docker-starter.git
cd flask-docker-starter
```

## Prerequisites

- Docker installed on your machine
- Docker Compose installed on your machine

### Build and Run the Application:

```sh
docker-compose up --build
```

### Access the Application:
  - The Flask application will be available at http://localhost:5000.

### Register a New User:

```sh
curl -X POST -H "Content-Type: application/json" -d '{"username": "testuser", "email": "testuser@example.com"}' http://localhost:5000/register
```
### Get the List of Registered Users:

```sh
curl http://localhost:5000/users
```

### Project Structure:
    .
    ├── app.py
    ├── docker-compose.yml
    ├── Dockerfile
    ├── requirements.txt
    └── README.md





