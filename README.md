# Class activity
# Fullstack web development

## 1 Database Design
- Define your database structure using **DBdiagrams**.
- Your schema must include at least one of each relationship type:
  - One-to-One  
  - One-to-Many  
  - Many-to-Many  

---

## 2 Backend Repository
- Create a **separate repository** for your backend application.
- Host the repository on **GitLab**.
- Add all collaborators/contributors to the repository.

---

## 3 Virtual Environment
- Navigate to your project working directory.
- Create and activate a Python virtual environment.
`python -m venv venv`
`source venv/bin/activate`
---

## 4 Django Project
- Create a new **Django project** inside the repository.
`django-admin startproject name`

---

## 5 Models
- Define Django models based on the database structure created in **Step 1**.
- Ensure relationships are correctly represented using Django ORM fields.

---

## 6 Views and URLs
- Create API views using **Django REST Framework (DRF)**.
- Configure URL routing for all endpoints.

---

## 7 PostgreSQL Driver
- Install the PostgreSQL database driver for Python.
`pip install psycopg[binary]
 psql -h localhost -U myuser -d mydb
`
---

## 8 Hosting
- Host the **PostgreSQL database** and **Django application** on **Render**.
  https://render.com/

---

## 9 Environment Variables
- Add database environment variables to a `.env` file.
- Install and use **python-dotenv** to load environment variables.
`pip install python-dotenv
`
- Upload the `.env` configuration to the hosting platform.

---

## 10 Database Configuration
- Configure the PostgreSQL database connection in `settings.py`.

---

## 11 Migrations
- Run Django migrations to create database tables.
`python manage.py makemigrations
python manage.py migrate`
---

## 12 Data Seeding and API Testing
- Create a data seeding script to populate the database.
- Use **Postman** to test all API endpoints.

---

## 13 Frontend–Backend Communication
- Implement fetch logic in the frontend.
- Use appropriate HTTP methods:
  - `GET`
  - `POST`
  - `PUT`
  - `PATCH`

---

## 14 Data Presentation
- Fetch data from the backend.
- Display database data on the frontend UI.
