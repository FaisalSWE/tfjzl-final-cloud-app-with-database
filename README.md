# Online Course Django Application

This Django project is an online course platform where users can enroll in courses, take exams, and view their results.

---

## Features

- User registration and login/logout
- Course browsing and enrollment
- Course detail pages with lessons
- Exam functionality with multiple-choice questions (including multi-select)
- Exam submission and result evaluation
- Admin interface for managing courses, lessons, questions, choices, and submissions

---

## Setup Instructions

### Prerequisites

- Python 3.7+
- Django 4.x
- Virtual environment recommended

### Installation

1. Clone the repository:

```bash
git clone https://github.com/FaisalSWE/tfjzl-final-cloud-app-with-database
cd tfjzl-final-cloud-app-with-database
```
2. Create and activate a virtual environment:
```bash
python3 -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
```

3. Install dependencies:

``` bash

pip install -r requirements.txt
```

4. Apply migrations:
```bash
python manage.py makemigrations
python manage.py migrate
```

5. Create a superuser for admin access:
```bash

python manage.py createsuperuser
```

6. Run the development server:

``` bash

python manage.py runserver
```

## Usage:

- Visit **http://localhost:8000/onlinecourse/** in your browser.

- Register a new user or log in.

- Browse courses and enroll.

- Take exams by selecting answers and submitting.

- View your exam results with scores and feedback.

- Admins can manage courses, lessons, questions, and exam choices via Django admin at /admin/.

## Important Files
- **onlinecourse/models.py** — Contains models for courses, lessons, enrollments, questions, choices, and submissions.

- **onlinecourse/views.py** — Views handling user registration, course details, exam submission, and result display.

- **onlinecourse/urls.py** — URL patterns for app routes.

- **onlinecourse/templates/** — HTML templates with Bootstrap styling.

- **onlinecourse/admin.py** — Admin registration and customization.

## Testing the Application
1. Log in as a registered user.

2. Enroll in a course.

3. Take the exam on the course detail page.

4. Submit answers and view your score and results.

5. Admins can add/edit courses, questions, and choices via the Django admin interface.

## Troubleshooting
- If you encounter migration issues, try deleting the SQLite database (**db.sqlite3**) and rerun migrations.

- Make sure media files (like course images) are placed correctly if used.

- Check console output for errors and tracebacks.

