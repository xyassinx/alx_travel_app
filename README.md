# ALX Travel App 🌍

Welcome to the **ALX Travel App**, a robust Django-based backend system built as a foundation for a travel listing platform. This application is designed following industry best practices for project setup, database integration, and API documentation.

## 🚀 Project Overview

This project is part of a milestone to build a scalable and maintainable travel app backend using:

- Django & Django REST Framework
- MySQL for data management
- Swagger for API documentation
- CORS support for frontend-backend interaction
- Environment-based configuration
- Celery & RabbitMQ (for future background task handling)

---

## 🧠 Learning Objectives

- Master advanced Django project setup with modular and production-ready configs
- Secure configuration using `django-environ` and `.env` files
- Integrate essential developer tools for API development and documentation
- Prepare a backend that is scalable, secure, and collaboration-ready

---

## 🔧 Tech Stack

- **Language:** Python 3.x
- **Framework:** Django, Django REST Framework
- **Database:** MySQL
- **API Docs:** drf-yasg (Swagger)
- **Task Queue (Planned):** Celery + RabbitMQ
- **Version Control:** Git + GitHub
- **Environment Config:** django-environ

---

## 📁 Project Structure

```
alx_travel_app/
│
├── alx_travel_app/           # Django project folder
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── listings/                 # Main app for travel listings
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── migrations/
│
├── venv/                     # Virtual environment
├── .env                      # Environment variables (DO NOT COMMIT)
├── requirement.txt           # Dependency list
├── manage.py
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repo

```bash
git clone https://github.com/<your-username>/alx_travel_app.git
cd alx_travel_app
```

### 2. Create and Activate Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate     # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirement.txt
```

### 4. Setup `.env` File

Create a `.env` file in the root with the following:

```ini
DEBUG=True
DB_NAME=your_db_name
DB_USER=your_db_user
DB_PASSWORD=your_db_password
DB_HOST=localhost
DB_PORT=3306
```

### 5. Run Migrations and Start Server

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

### 6. Access Swagger API Docs

Visit: [http://localhost:8000/swagger/](http://localhost:8000/swagger/)

---

## ✅ API Endpoints Preview

| Endpoint        | Method | Description                  |
|-----------------|--------|------------------------------|
| `/swagger/`     | GET    | API documentation (Swagger)  |
| `/listings/`    | GET    | Sample Listings API (stub)   |

> More endpoints will be added in future milestones.

---

## 🧪 Testing the App (Optional)

You can add unit tests in the `tests.py` file of the `listings` app and run:

```bash
python manage.py test
```

---

## 📦 Future Improvements

- Add user authentication and authorization
- Advanced filtering and pagination for listings
- Celery integration for email/task queues
- Dockerize the app for deployment
- CI/CD integration for testing and deployment


