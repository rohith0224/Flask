# Task Master

Task Master is a simple Flask-based task management application. It allows users to create, update, and delete tasks, with a clean and responsive user interface.

---

## Features
- Add new tasks with a description.
- View all tasks in a table format.
- Update existing tasks.
- Delete tasks.

---

## Prerequisites
- Python 3.12 or higher
- Flask
- Flask-SQLAlchemy

---

## Installation

### 1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-folder>
```

### 2. Create and activate a virtual environment:
```bash
python3 -m venv env
source env/bin/activate   # On Windows: env\Scripts\activate
```

### 3. Install dependencies:
```bash
pip install -r requirements.txt
```

If `requirements.txt` does not exist, create it using:
```bash
pip freeze > requirements.txt
```

---

## Usage

### 1. Set Flask environment variables:
```bash
export FLASK_APP=app.py      # Mac/Linux
set FLASK_APP=app.py         # Windows
```

(Optional) Enable debug mode:
```bash
export FLASK_ENV=development
```

### 2. Run the Flask application:
```bash
flask run
```

By default, the app runs on:
```
http://127.0.0.1:5000
```

---

## Database Setup
This app uses **Flask-SQLAlchemy** for database management.

To create the database tables:
```bash
python
>>> from app import db
>>> db.create_all()
```

---

## Project Structure
```
project-folder/
│
├── app.py                # Main Flask application
├── templates/            # HTML templates
├── static/               # CSS, JS, Images
├── env/                  # Virtual environment
├── requirements.txt      # Project dependencies
└── README.md             # Project documentation
```

