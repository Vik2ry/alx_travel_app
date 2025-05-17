# ALX Travel App

The **ALX Travel App** is a Django-based backend application designed as the foundation for a scalable travel listing platform. This project sets up a modular, production-ready architecture with robust database integration and automated API documentation.

## 🚀 Project Overview

This milestone focuses on:

- Creating a Django project and app structure.
- Setting up MySQL as the primary database using environment variables.
- Integrating Swagger (via drf-yasg) for API documentation.
- Enabling CORS for cross-origin API access.
- Laying the groundwork for scalable task management using Celery and RabbitMQ.

---

## 📁 Project Structure

```
alx_travel_app/
├── alx_travel_app/       # Core Django config (settings, URLs, WSGI)
│   ├── settings.py
│   ├── urls.py
│   └── ...
├── listings/             # App for managing travel listings
├── manage.py             # Django CLI entry point
├── requirements.txt      # Project dependencies
├── .env                  # Environment variables (not committed)
├── .gitignore
└── README.md             # Project documentation
```

---

## Tech Stack

- **Django**: Web framework
- **Django REST Framework**: API layer
- **MySQL**: Database
- **drf-yasg**: Swagger/OpenAPI documentation
- **django-environ**: Environment variable management
- **django-cors-headers**: CORS support
- **Celery + RabbitMQ** _(future-ready)_: Background task processing

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/alxtravelapp.git
cd alxtravelapp
```

### 2. Set Up Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirement.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory:

```env
DEBUG=True
SECRET_KEY=your-secret-key
DB_NAME=your_db_name
DB_USER=your_db_user
DB_PASSWORD=your_db_password
DB_HOST=localhost
DB_PORT=3306
```

### 5. Set Up the Database

Ensure MySQL is running and the database exists, then run:

```bash
python manage.py migrate
```

### 6. Run the Server

```bash
python manage.py runserver
```

Access the API documentation at:
👉 `http://127.0.0.1:8000/swagger/`

---

## 📌 API Documentation

This project uses **Swagger** via `drf-yasg`. All API endpoints are automatically documented and available at:

```
/swagger/
```

---

## 📦 Git Version Control

This project is version-controlled using Git. Key setup files and configuration are committed. Sensitive data like `.env` is excluded via `.gitignore`.

---

## ✅ Milestone Status

- [x] Django project initialized
- [x] `listings` app created
- [x] MySQL database configured via environment variables
- [x] Swagger integrated
- [x] CORS headers set
- [x] Git repository initialized and pushed

---
