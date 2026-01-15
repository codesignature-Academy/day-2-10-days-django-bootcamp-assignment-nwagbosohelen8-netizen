[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/kAAaG5C-)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=22246011&assignment_repo_type=AssignmentRepo)
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
