# Todo List Application

A Django-based Todo List application with REST API support.

## Features

- Create, Read, Update, and Delete Todo items
- Tag support for todo items
- Status tracking
- Due date management
- REST API with Basic Authentication
- 100% test coverage
- CI/CD with GitHub Actions

## Requirements

- Python 3.11+
- Django 4.2.7+
- Django Rest Framework 3.14.0+

## Installation

1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run migrations:
   ```bash
   python manage.py migrate
   ```
5. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```

## Running the Application

```bash
python manage.py runserver
```

The application will be available at `http://localhost:8000`

## API Endpoints

- `GET /api/todos/` - List all todos
- `POST /api/todos/` - Create a new todo
- `GET /api/todos/{id}/` - Retrieve a specific todo
- `PUT /api/todos/{id}/` - Update a specific todo
- `DELETE /api/todos/{id}/` - Delete a specific todo

## Running Tests

```bash
# Run all tests
python manage.py test

# Run with coverage
coverage run --source='.' manage.py test
coverage report
coverage html
```

## Test Coverage Summary

Unit Tests: 100%
Integration Tests: 100%

## Documentation

API documentation is available at `/api/docs/`

## License

MIT