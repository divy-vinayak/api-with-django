# api-with-django

## Create a virtual env
`$ python3 -m venv .venv`

## activate your virtual env
`$ . .venv/bin/activate`
or 
`$ source .venv/bin/activate`

*Note: To deactivate, `$ deactivate`*

# AFter activating the virtual env
## Install django and django rest framework
`$ pip install django`
`$ pip install djangorestframework`

## Create the django project
`$ django-admin startproject drinks .`

## Create admin to access /admin endpoint in the app
`$ python manage.py createsuperuser`

### created a drink model class in drinks/models.py
### next step - make migrations
`$ python manage.py makemigrations drinks`

### apply these migrations using
`$ python manage.py migrate`

## To see these db tables in /admin endpoint
### register the models in drinks/admin.py