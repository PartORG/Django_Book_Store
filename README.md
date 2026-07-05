# Django_Book_Store

**A simple example of a Django-based book store application.**

[![Python](https://img.shields.io/badge/python-3.x-blue.svg)] [![License](https://img.shields.io/badge/license-MIT-green.svg)] [![Package Manager](https://img.shields.io/badge/package-manager-pip-yellow.svg)] [![Framework](https://img.shields.io/badge/framework-Django-brightgreen.svg)] [![Testing](https://img.shields.io/badge/testing-None-red.svg)]

Django_Book_Store is a basic example of a Django application designed to demonstrate some key features of the Django framework. It provides a simple interface for managing books, authors, and addresses.

## Table of Contents

1. [Features](#features)
2. [How It Works](#how-it-works)
3. [Technology Stack](#technology-stack)
4. [Requirements](#requirements)
5. [Installation](#installation)
6. [Configuration](#configuration)
7. [Quick Start](#quick-start)
8. [Usage](#usage)
9. [Project Structure](#project-structure)
10. [Development](#development)
11. [Limitations](#limitations)
12. [License](#license)

## Features

### Book Management
- **Book Details:** View, add, edit, and delete book details.
- **Author Management:** Manage authors associated with books.

### Address Management
- **Address Details:** Add, edit, and manage addresses for authors.

### Templates
- **Base Template:** A reusable base template for all pages.
- **Book Detail Page:** Displays detailed information about a specific book.
- **Index Page:** Lists all available books.

## How It Works

Django_Book_Store is built using Django, a high-level Python web framework that encourages rapid development and clean, pragmatic design. The application follows the Model-View-Template (MVT) architecture, where:

- **Models** define the data structure.
- **Views** handle business logic and interact with models.
- **Templates** generate HTML output.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| Django     | Web framework for building robust web applications. |
| Python     | Programming language used to develop the application. |
| SQLite     | Database for storing book, author, and address data. |

## Requirements

- Python 3.x
- pip (Python package installer)

## Installation

To install Django_Book_Store, follow these steps:

1. Clone the repository:
   ```sh
   git clone https://github.com/PartORG/Django_Book_Store.git
   ```

2. Navigate to the project directory:
   ```sh
   cd Django_Book_Store
   ```

3. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

4. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

5. Run migrations:
   ```sh
   python manage.py migrate
   ```

6. Create a superuser (for admin access):
   ```sh
   python manage.py createsuperuser
   ```

7. Start the development server:
   ```sh
   python manage.py runserver
   ```

## Configuration

Django_Book_Store uses environment variables for configuration. The following environment variables are used:

- `SECRET_KEY`: A secret key for cryptographic signing.
- `DEBUG`: Set to `True` for development and `False` for production.

These variables can be set in a `.env` file or directly in the operating system's environment variables.

## Quick Start

To quickly get started with Django_Book_Store, follow these steps:

1. Clone the repository:
   ```sh
   git clone https://github.com/PartORG/Django_Book_Store.git
   cd Django_Book_Store
   ```

2. Create a virtual environment and activate it:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

4. Run migrations:
   ```sh
   python manage.py migrate
   ```

5. Create a superuser:
   ```sh
   python manage.py createsuperuser
   ```

6. Start the development server:
   ```sh
   python manage.py runserver
   ```

7. Access the application in your web browser at `http://127.0.0.1:8000/`.

## Usage

To use Django_Book_Store, follow these steps:

1. **Admin Interface:** Navigate to `http://127.0.0.1:8000/admin` and log in with the superuser credentials.
2. **Add Books:** Go to the "Books" section and add new books.
3. **Manage Authors:** Add authors associated with each book.
4. **View Details:** Access the "Book Detail" page to view detailed information about a specific book.

## Project Structure

```
Django_Book_Store/
├── book_outlet/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── migrations/
│   │   ├── 0001_initial.py
│   │   └── ...
│   ├── models.py
│   ├── templates/
│   │   ├── book_outlet/
│   │   │   ├── base.html
│   │   │   ├── book_detail.html
│   │   │   └── index.html
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── book_store/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── db.sqlite3
└── manage.py
```

- `book_outlet/`: Contains the application logic.
- `book_store/`: Contains project-wide settings and configurations.
- `db.sqlite3`: The SQLite database file.

## Development

Django_Book_Store follows a standard Django development workflow. For more information, refer to the [Django documentation](https://docs.djangoproject.com/en/stable/intro/tutorial01/).

## Limitations

- **No Testing:** This example does not include any automated tests.
- **Basic Features:** The application provides basic features for demonstration purposes.

## License

Django_Book_Store is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.