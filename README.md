# Class activity
# Topic: Backend development

## 1 Database Design
- Use **DBdiagrams** (https://dbdiagram.io) to design your database schema.
- Clearly define:
  - Tables (entities)
  - Columns and data types
  - Primary keys and foreign keys
- Your design **must include**:
  - One-to-One relationship  
  - One-to-Many relationship  
  - Many-to-Many relationship
- Export or save the diagram for submission.

---

## 2 Backend Repository
- Create a **new repository** specifically for the backend.
- Host the repository on **GitLab**.
- Add a `README.md` explaining:
  - Project purpose
  - Technologies used
  - How to run the project locally
- Add all collaborators/contributors.

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
- Create one or more Django apps for your domain logic.
- Define models in models.py based on your database diagram.
- Use Django ORM relationship fields:
  - `OneToOneField`
  - `ForeignKey`
  - `ManyToManyField`

- Add meaningful field names and constraints (null, blank, unique).

---

## 6 Views and URLs
- Install Django REST Framework (DRF).
- Create serializers for your models.
- Implement API views or viewsets for CRUD operations.
- Configure URL routing to expose endpoints for data access and modification.

---

## 7 PostgreSQL Driver
- Install the PostgreSQL database driver for Python.
  
`pip install psycopg[binary]
 psql -h localhost -U myuser -d mydb
`
---

## 8 Hosting
- Create an account on Render: https://render.com/
- Provision:
    - A PostgreSQL database service
    - A web service for your Django application
- Ensure both services can communicate securely.

---

## 9 Environment Variables
- Create a .env file to store sensitive information:
    - Database name
    - Username
    - Password
    - Host
    - Port
- Install dotenv support:
  
`pip install python-dotenv
`
- Load environment variables in Django settings.
- Add environment variables to Render’s dashboard (do not commit secrets).

---

## 10 Database Configuration
- Update `settings.py` to use PostgreSQL.
- Configure the `DATABASES` setting using environment variables.
- Confirm Django can connect to the database.

---

## 11 Migrations
- Run Django migrations to create database tables.
  
`python manage.py makemigrations
python manage.py migrate`

---

## 12 Data Seeding and API Testing
- Create a data seeding script or Django management command.
- Populate the database with sample data.
- Use Postman to:
    - Test API endpoints
    - Validate responses
    - Confirm correct HTTP status codes

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



# To submit
1. Database diagrams
2. Backend repository link (GitLab)
3. Backend domain URL hosted on Render
4. List of API endpoints with example requests
