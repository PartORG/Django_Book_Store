# Django_Book_Store

**A simple book store application built with the Django Framework.**

[![Python](https://img.shields.io/badge/python-3.x-blue.svg)] [![License](https://img.shields.io/badge/license-MIT-green.svg)] [![Package Manager](https://img.shields.io/badge/package-manager-pip-yellow.svg)] [![Framework](https://img.shields.io/badge/framework-Django-brightgreen.svg)]

## Introduction

Django_Book_Store is a practical example of using the Django Framework to build a book store application. It includes models, views, templates, and migrations for managing books, authors, and addresses.

This project serves as a learning resource for understanding Django's core concepts and provides a solid foundation for building more complex applications.

## Table of Contents

- [Features](#features)
- [How It Works](#how-it-works)
- [Technology Stack](#technology-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Development](#development)
- [Limitations](#limitations)
- [License](#license)

## Features

### Models
- **Book**: Represents a book with attributes like title, author, ISBN, and rating.
- **Author**: Represents an author with attributes like name, bio, and address.
- **Address**: Represents an address with attributes like street, city, state, and country.

### Views
- **Index View**: Displays a list of all books.
- **Book Detail View**: Displays details of a specific book.

### Templates
- **Base Template**: Provides the basic structure for other templates.
- **Book Detail Template**: Displays detailed information about a book.

## How It Works

Django_Book_Store follows a typical Django project structure. The main components are:

1. **Models**: Define the data structure using Django's ORM.
2. **Views**: Handle business logic and interact with models.
3. **Templates**: Generate HTML content based on views.
4. **URLs**: Map URLs to views.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| Python     | Programming language |
| Django     | Web framework |
| SQLite     | Database |

## Requirements

- Python 3.x
- pip (Python package installer)

## Installation

To install the project, follow these steps:

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

5. Apply migrations:
   ```sh
   python manage.py migrate
   ```

6. Create a superuser (for admin access):
   ```sh
   python manage.py createsuperuser
   ```

7. Run the development server:
   ```sh
   python manage.py runserver
   ```

## Configuration

The project uses environment variables for configuration. The following variables are observed:

- `SECRET_KEY`: A secret key used by Django for cryptographic signing.
- `DEBUG`: Controls whether debug mode is enabled.

These variables can be set in a `.env` file or directly in the environment.

## Quick Start

To quickly get started, follow these steps:

1. Clone the repository and navigate to the project directory.
2. Create and activate a virtual environment.
3. Install dependencies.
4. Apply migrations.
5. Create a superuser.
6. Run the development server.

Example commands:
```sh
git clone https://github.com/PartORG/Django_Book_Store.git
cd Django_Book_Store
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

## Usage

To interact with the application, you can:

- Access the admin panel at `http://127.0.0.1:8000/admin/` using the superuser credentials.
- Browse books and their details at `http://127.0.0.1:8000/`.

## Project Structure

```
Django_Book_Store/
├── book_outlet/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── migrations/
│   │   ├── 0001_initial.py
│   │   ├── 0002_book_author_book_is_bestselling_alter_book_rating.py
│   │   ├── 0003_book_slug.py
│   │   ├── 0004_author_alter_book_slug_alter_book_author.py
│   │   ├── 0005_alter_book_author.py
│   │   ├── 0006_address_author_address.py
│   │   ├── 0007_country_alter_address_options_and_more.py
│   │   └── __init__.py
│   ├── models.py
│   ├── templates/
│   │   └── book_outlet/
│   │       ├── base.html
│   │       ├── book_detail.html
│   │       └── index.html
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

- `book_outlet/`: Contains the application code.
- `book_store/`: Contains project-wide configuration and management scripts.

## Development

The development workflow involves:

1. Writing models in `models.py`.
2. Creating views in `views.py`.
3. Designing templates in `templates/`.
4. Defining URLs in `urls.py`.

## Limitations

- The application is a simple example and lacks advanced features like user authentication, search functionality, or payment processing.
- Error handling is minimal.

## License

Django_Book_Store is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.