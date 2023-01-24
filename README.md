# **[Django Admin Black PRO](https://appseed.us/product/black-dashboard-pro/django/)**

**Django** starter styled with **[Django Admin Black PRO](https://appseed.us/product/black-dashboard-pro/django/)**, a premium `Bootstrap 5` design from [Creative-Tim](https://bit.ly/3fKQZaL).
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme:

**Private REPO**: `git+https://github.com/app-generator/priv-django-admin-black-pro`

<br />

## Features: 

- **UI Kit**: Black Dashboard PRO `v1.1.2` by Creative-Tim
- [Django Black PRO](https://appseed.us/product/black-dashboard-pro/django/) - `sample project`
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Django Black PRO - Premium Seed project powered by Flask.](https://user-images.githubusercontent.com/51070104/187623954-c4ade6a0-8cb2-4d2e-8698-e962621a613c.png)

<br />

## Why `Django Admin Black PRO`

- Modern [Bootstrap](https://www.admin-dashboards.com/bootstrap-5-templates/) Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`

Designed for those who like bold elements and beautiful websites. Made of hundred of elements, designed blocks, and fully coded pages, **Soft UI Dashboard PRO** is ready to help you create stunning websites and web apps.

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install git+https://github.com/app-generator/priv-django-admin-black-pro.git
```

<br />

> Add `admin_black_pro` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

```python
    INSTALLED_APPS = (
        ...
        'admin_black_pro.apps.AdminBlackProConfig',
        'django.contrib.admin',
    )
```

<br />

> Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:

```python
    LOGIN_REDIRECT_URL = '/'
    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `admin_black_pro` urls in your Django Project `urls.py` file

```python
    from django.urls import path, include

    urlpatterns = [
        ...
        path('', include('admin_black_pro.urls')),
    ]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

Access the `admin` section in the browser: `http://127.0.0.1:8000/`

<br />

---
**[Django Admin Black PRO](https://appseed.us/product/black-dashboard-pro/django/)** - Modern `Admin Interface` provided by **[AppSeed](https://appseed.us/)**.
