# Recruitment Management System

[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/Lemersom/Recruitment-Fullstack/blob/main/README.md)
[![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](https://github.com/Lemersom/Recruitment-Fullstack/blob/main/README.pt-br.md)

This project is a full-stack application designed to manage resumes efficiently, allowing users to add personal details, professional experience, academic qualifications, and contact information.

## Technologies

* Back-End: Django with Django REST Framework (DRF) for creating the API
* Front-End: React.js with Vite for fast and responsive UI
* Containerization: Docker for containerizing the application

## Project Features

* Django backend providing a RESTful API using DRF to manage resume data
* React.js frontend allowing users to add and update personal, professional, and academic information
* Basic validation for user inputs like email formats, phone numbers, and date formats
* Admin panel in Django for managing submitted resumes

## Running Locally With Docker

**Prerequisites:** Make sure you have Docker and Docker Compose installed on your machine.

Clone the project
```
git clone --recurse-submodules https://github.com/Lemersom/Recruitment-Fullstack.git
```

Navigate to the cloned directory
```
cd Recruitment-Fullstack
```

Build the containers
```
docker-compose build
```

Start the containers
```
docker-compose up
```

Run database migrations
```
docker-compose exec backend python manage.py migrate
```

Create a SuperUser
```
docker-compose exec backend python manage.py createsuperuser
```

## Running Locally Without Docker

**Prerequisites:** Ensure you have Python and Node.js installed on your machine.

Clone the project
```
git clone --recurse-submodules https://github.com/Lemersom/Recruitment-Fullstack.git
```

### Backend Setup

Navigate to the backend directory
```
cd Recruitment-Fullstack\backend
```

Create and activate a virtual environment
```
python -m venv venv
source venv/bin/activate  # For Windows use `venv\Scripts\activate`
```

Install dependencies
```
pip install -r requirements.txt
```

Run database migrations
```
python manage.py migrate
```

Create a SuperUser
```
py manage.py createsuperuser
```

Start the Django server
```
python manage.py runserver
```

### Frontend Setup

Navigate to the frontend directory
```
cd Recruitment-Fullstack\frontend 
```

Install dependencies
```
npm install
```

Start the development server
```
npm run dev
```

## Accessing the Application

* Backend API: http://localhost:8000
* Admin Panel: http://localhost:8000/admin
* Frontend: http://localhost:5173
