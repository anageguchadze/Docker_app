# Docker_app

This project consists of two Django Rest Framework (DRF) applications running in separate containers using Docker and Docker Compose. The applications are:

1. **Library App** - A simple API for managing books.
2. **Tasks App** - A simple API for managing tasks.

## Features
- Django Rest Framework (DRF) for API development.
- PostgreSQL as the database backend.
- Docker and Docker Compose for containerization.
- Automatic migrations and superuser creation.
- Exposed endpoints for books and tasks management.

## Installation and Setup

### Prerequisites
- Docker
- Docker Compose

### Steps to Run
1. Clone the repository:
   git clone https://github.com/anageguchadze/Docker_app.git
   cd Docker_app

2. Create a `.env` file in the root directory and define necessary environment variables (e.g., PostgreSQL credentials).

3. Build and start the services:
   docker-compose up --build
  
4. The services will be available at:
   - Library App: `http://localhost:8001`
   - Tasks App: `http://localhost:8002`

## API Endpoints

### Library App (Books API)
- `GET /books/` - Retrieve all books
- `POST /books/` - Add a new book
- `GET /books/{id}/` - Retrieve a specific book
- `PUT /books/{id}/` - Update a book
- `DELETE /books/{id}/` - Delete a book

### Tasks App (Tasks API)
- `GET /tasks/` - Retrieve all tasks
- `POST /tasks/` - Create a new task
- `GET /tasks/{id}/` - Retrieve a specific task
- `PUT /tasks/{id}/` - Update a task
- `DELETE /tasks/{id}/` - Delete a task

## Contributing
Feel free to fork this repository and submit pull requests.

## License
This project is licensed under the MIT License.