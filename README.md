# Recruitment Management System

This project is a full-stack application designed to manage resumes efficiently, allowing users to add personal details, professional experience, academic qualifications, and contact information.

## Technologies

* Back-End: Django with Django REST Framework (DRF) for creating the API
* Front-End: React.js with Vite for fast and responsive UI

## Project Features

* Django backend providing a RESTful API using DRF to manage resume data
* React.js frontend allowing users to add and update personal, professional, and academic information
* Basic validation for user inputs like email formats, phone numbers, and date formats
* Admin panel in Django for managing submitted resumes

## Running Locally

**Prerequisites:** Ensure you have Python and Node.js installed on your machine. Clone the project and set up the backend and frontend.

### Backend Setup

Clone the project
```
git clone --recurse-submodules https://github.com/Lemersom/Recruitment-Fullstack.git
```

Navigate to the backend directory
```
cd backend
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

Create SuperUser
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
cd frontend  # If you are in the backend directory `cd ../frontend` 
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

* Backend API: Runs on http://localhost:8000
* Frontend: Runs on http://localhost:5173








