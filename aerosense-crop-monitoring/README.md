# AeroSense

Django project for aerial crop monitoring (thesis). The backend is named **aerosense**; a single home template is in place so frontend work can start immediately.

## Requirements

- Python 3.11+
- pip

## Setup

From the project root:

```bash
python -m venv .venv
```

**Windows (PowerShell)**

```powershell
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

**macOS / Linux**

```bash
source .venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) for the home page. Admin is at `/admin/`.

## Project layout

```
aerosense/          # Django project settings and URLs
home/               # Home app (landing view)
templates/home.html # Landing page template
static/css/home.css # Starter stylesheet
manage.py
requirements.txt
```

Add more templates under `templates/` and assets under `static/` as the frontend grows.
