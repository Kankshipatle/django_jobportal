# Django Job Portal

A job portal web application built with Django as a practice project to learn backend web development, authentication, database models, class-based views, and URL routing.

## Overview

The Django Job Portal allows users to browse job listings, post jobs, and apply for available opportunities. It also includes dashboards for users to manage their posted jobs, track their applications, and view applications received for their job postings.

## Features

- **Job Listings:** Browse available job opportunities.
- **Job Details:** View detailed information about individual jobs.
- **User Authentication:** Register, log in, and log out.
- **Post a Job:** Authenticated users can publish job listings.
- **Manage Posted Jobs:** View, update, and delete jobs posted by the logged-in user.
- **Apply for Jobs:** Submit applications for job opportunities.
- **My Applications:** View jobs you have applied for.
- **Employer Applications Dashboard:** View applications received for jobs posted by the logged-in user.
- **Duplicate Application Prevention:** Prevents the same user from applying to the same job more than once.
- **Access Control:** Restricts job management and application views to the appropriate authenticated users.

## Tech Stack

- **Language:** Python
- **Backend Framework:** Django
- **Database:** SQLite
- **Frontend:** HTML, CSS, Django Templates
- **Version Control:** Git and GitHub

## Project Structure

```text
jobportal/
├── accounts/                       # User account functionality
├── jobs/
│   ├── migrations/                 # Database migrations
│   ├── templates/
│   │   ├── job_detail.html
│   │   └── employer_applications_list.html
│   ├── models.py                   # Job and Application models
│   ├── views.py                    # Views and application logic
│   ├── urls.py                     # Job-related URL patterns
│   └── forms.py                    # Job forms
├── jobportal/
│   ├── settings.py                 # Django settings
│   └── urls.py                     # Main URL configuration
├── templates/
│   └── base.html                   # Shared base template and navigation
├── manage.py
└── README.md
```

*Note: The structure above highlights the main project files; other templates and configuration files may also be present.*

## Getting Started

### Prerequisites

- Python 3.11 or a compatible Python version
- pip
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/Kankshipatle/django_jobportal.git
cd django_jobportal
```

### 2. Create and Activate a Virtual Environment

**Windows PowerShell:**

```powershell
py -3.11 -m venv .venv
.\.venv\Scripts\Activate.ps1
```

If PowerShell blocks script execution, you can activate the environment using Command Prompt instead:

```cmd
.venv\Scripts\activate.bat
```

### 3. Install Django

```bash
python -m pip install Django
```

### 4. Apply Database Migrations

```bash
python manage.py migrate
```

### 5. Create an Administrator Account (Optional)

```bash
python manage.py createsuperuser
```

Follow the prompts to set up the administrator account.

### 6. Run the Development Server

```bash
python manage.py runserver
```

Open the application in your browser:

http://127.0.0.1:8000/

## Main Application Routes

| Route | Description |
|---|---|
| `/` | Browse job listings |
| `/jobs/create/` | Post a new job |
| `/jobs/<id>/` | View job details |
| `/jobs/<id>/update/` | Update a job you posted |
| `/jobs/<id>/delete/` | Delete a job you posted |
| `/jobs/<id>/apply/` | Apply for a job |
| `/my-jobs/` | View your posted jobs |
| `/my-applications/` | View your submitted applications |
| `/employer-applications/` | View applications received for your posted jobs |

## Learning Outcomes

This project helped me practice:

- Building web applications with Django.
- Understanding Django models and relationships.
- Working with URL patterns and named routes.
- Using function-based and class-based views.
- Handling forms and database operations.
- Implementing authentication and access restrictions.
- Using Django Template Language and template inheritance.
- Managing code changes with Git and GitHub.

## Future Improvements

- Improve the user interface and responsive design.
- Add job search, filtering, and sorting.
- Add application status tracking.
- Improve form validation and user feedback.
- Add automated tests for key workflows.

## Project Status

**Completed as a Django practice project.**

This project was developed to strengthen my understanding of Django fundamentals and full-stack web application workflows.

## Author

**Kankshi Patle**

GitHub: [Kankshipatle](https://github.com/Kankshipatle)
