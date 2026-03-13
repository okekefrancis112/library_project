# Library Project

A Django REST API for managing a library system with book catalog and lending functionality.

## Overview

A RESTful API built with Django REST Framework for managing a library's book collection, providing endpoints for CRUD operations on books.

## Features

- **Book Management** — Add, view, update, and delete books
- **REST API** — Clean RESTful endpoints with DRF
- **Serialization** — JSON serialization for book data
- **Admin Panel** — Django admin for library management

## Tech Stack

- **Python** 3.10
- **Django** — Web framework
- **Django REST Framework** — API toolkit
- **SQLite** — Database

## Getting Started

```bash
git clone https://github.com/okekefrancis112/library_project.git
cd library_project
pip install django djangorestframework
python manage.py migrate
python manage.py runserver
```

### API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/books/` | List all books |
| POST | `/api/books/` | Add a new book |
| GET | `/api/books/<id>/` | Get book details |
| PUT | `/api/books/<id>/` | Update book info |
| DELETE | `/api/books/<id>/` | Remove a book |

## Project Structure

```
├── api/
│   ├── models.py          # API models
│   ├── serializers.py     # DRF serializers
│   ├── views.py           # API views
│   └── urls.py            # API routes
├── books/
│   ├── models.py          # Book model
│   ├── views.py           # Book views
│   └── urls.py            # Book routes
├── manage.py
└── db.sqlite3
```

## License

MIT
