# myapp — assignment setup

This README shows the steps students should follow to create and register a new Django app named `myapp` in this project.

**Prerequisites**
- Python 3.x and `pip`
- `git` (to clone the repository)

**Steps**

1. Clone the repository (use the URL provided for your assignment):

```bash
git clone <repository-url>
cd <repo-directory>
# Example: cd Day2-10-days-django-bootcamp-assignment
```

2. (Optional but recommended) Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

3. Install project dependencies:

```bash
pip install -r requirements.txt
```

4. Create the Django app `myapp`:

```bash
python manage.py startapp myapp
```

5. Register `myapp` in `proj/settings.py` by adding it to `INSTALLED_APPS`.

Open `proj/settings.py` and find the `INSTALLED_APPS` list. Add `'myapp',` to the list. Example:

```python
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'myapp',  # <-- add this line
]
```

6. Apply migrations and run the development server to verify everything works:

```bash
python manage.py migrate
python manage.py runserver
```

You should now be able to visit `http://127.0.0.1:8000/` and begin building your app inside `myapp/`.

If you want, I can also create a minimal `myapp` view and URL example. Would you like that?
