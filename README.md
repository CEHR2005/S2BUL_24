# Movie Rating Application

A full-stack application for rating and reviewing movies, built with React (frontend) and FastAPI (backend).

## Project Structure

- `frontend/`: React application built with Vite
- `backend/`: FastAPI application with PostgreSQL database
- `docker-compose.yml`: Docker Compose configuration for running the entire application

## Prerequisites

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

1. Clone the repository:

```bash
git clone <repository-url>
cd <repository-directory>
```

2. Start the application using Docker Compose:

```bash
docker-compose up
```

This will start three services:
- Frontend: React application running on http://localhost:5173
- Backend: FastAPI application running on http://localhost:8000
- PostgreSQL: Database running on localhost:5432

3. Access the application:
   - Frontend: http://localhost:5173
   - Backend API documentation: http://localhost:8000/docs

## Development

### Frontend

The frontend is a React application built with Vite. It includes:
- User authentication
- Movie listing and details
- Rating and commenting on movies
- User profiles
- Statistics visualization

### Backend

The backend is a FastAPI application with the following features:
- RESTful API endpoints
- PostgreSQL database integration with SQLAlchemy
- JWT authentication
- CORS configuration for frontend integration
- Swagger UI documentation

## API Documentation

The API documentation is available at http://localhost:8000/docs when the application is running.

## Environment Variables

### Backend

- `DATABASE_URL`: PostgreSQL connection URL
- `SECRET_KEY`: Secret key for JWT token generation
- `CORS_ORIGINS`: Comma-separated list of allowed origins for CORS

### Frontend

- `VITE_API_URL`: URL of the backend API

## License

[MIT](LICENSE)