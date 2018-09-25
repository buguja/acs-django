# Proyecto para aprender Django

## Requerimientos
- Python 3
- Django 2.1
- PostgreSQL

## Cómo ejecutar en Linux
Clonar proyecto
```
$ mkdir ~/proyecto-acs-django
$ cd ~/proyecto-acs-django/
$ git clone https://github.com/buguja/acs-django.git
```

Configurar proyecto
```
$ sudo apt install python3
$ sudo apt install python3-pip
$ python3 -m pip install virtualenv
$ sudo apt-get install python3-venv
$ python3 -m venv virtual_env
```

Activar enviropment
```
$ . virtual_env/bin/activate
```

Instalar librerías
```
$ python3 -m pip install django
$ python3 -m pip install psycopg2
```

Configuar proyecto
```
$ cd acs-django
$ python3 manage.py makemigrations
$ python3 manage.py migrate
$ python3 manage.py createsuperuser

Username (leave blank to use 'javier'): admin
Email address: admin@admin.com
Password: 
Password (again): 
The password is too similar to the email address.
This password is too short. It must contain at least 8 characters.
This password is too common.
Bypass password validation and create user anyway? [y/N]: y
Superuser created successfully

$ python3 manage.py runserver
```

http://127.0.0.1:8000  
http://127.0.0.1:8000/admin

Desactivar enviropment
```
$ deactivate
```
