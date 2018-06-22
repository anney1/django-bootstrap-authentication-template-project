[![Build Status](https://travis-ci.org/alexdlaird/django-bootstrap-authentication-template-project.svg?branch=master)](https://travis-ci.org/alexdlaird/django-bootstrap-authentication-template-project)
[![codecov](https://codecov.io/gh/alexdlaird/django-bootstrap-authentication-template-project/branch/master/graph/badge.svg)](https://codecov.io/gh/alexdlaird/django-bootstrap-authentication-template-project)
[![Updates](https://pyup.io/repos/github/HeliumEdu/heliumcli/shield.svg)](https://pyup.io/repos/github/HeliumEdu/heliumcli/)


Django Bootstrap/Authentication Template Project
================

## Prerequisites
* Python (>= 2.7, >= 3.6)
* Pip (>= 9.0)

## Getting Started
The project is developed using [Python](https://www.python.org/), [Django](https://www.djangoproject.com), and [Bootstrap](http://getbootstrap.com/docs/3.3/).

This repository contains the source code for a Django Bootstrap/Authentication Template Project.

### Project Setup
To setup the Python/Django build environment, execute:

```
make install
```

This project is configured to work with a Virtualenv which has now been setup in the .venv folder. If you're unfamiliar with how this works, read up on Virtualenv here. The short version is, virtualenv creates isolated environments for each project's dependencies. To activate and use this environment when developing, execute:

```
source .venv/bin/activate
```

All commands below will now be run within the virtualenv (though `make` commands will always automatically enter the virtualenv before executing).

To ensure the database is in sync with the latest schema, database migrations are generated and run with Django. To run migrations, execute:

```
make migrate
```

Once migrations have been run, you can create a super user, which is a standard user that also has access to the /admin site.

```
python manage.py createsuperuser
```

Before commits are made, be sure to run tests and check the generated coverage report.

```
make test
```

### Development
To get started with minimal effort, assuming you have followed the "Getting Started" directions above, you should have the ENVIRONMENT environment
variable set to "dev".

Now you're all set! To start the development server, execute:

```
bin/runserver
```

A development server will be started at http://localhost:8000.
