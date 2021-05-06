---
title:  "Configure PostgreSQL in Django"
header:
  teaser: "/assets/images/500x300.png"
categories: 
  - Django
tags:
  - PostgreSQL
---

First of all, you install the correct PostgreSQL version for the operating system we have.

Once we have it installed with a password and everything, we create a test database through the command line or the one that is going to be needed.

`create database TestBase`

We must also install a package through pip that does not come by default and is necessary for it to work correctly:

`pip install psycopg2`

If you have errors, especially on mac os, you need to use the following command

`pip install psycopg2-binary`

And with that it should work. However, we still need to configure it in the settings.py


```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'projectrestaurant',
        'USER': 'postgres',
        'PASSWORD': 'XXXXXXX',
        'HOST': '127.0.0.1',
        'PORT': '5432',
    }
}
```

Adding this configuration and we would have the connection made with the database.

So we make sure that we are in the folder of our project and we carry out the migrations

`python manage.py makemigrations`

`python manage.py migrate`

Now, we must bear in mind that our python app must be in INSTALLED_APPS added.

With that if we go to our pgAdmin4 and look for the database and the tables we will see them created.