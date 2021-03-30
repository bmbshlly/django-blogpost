### [Live Demo](https://django-blogpost.herokuapp.com)

# Introduction

Blogpost is a web application backed by Django where every user can creates, updates and deletes post on the feed. New users can set profile picture(update later). Users can reset password via registered email. Application uses postreg(relation database) to store user information and their blogs. AWS is used to store static files(profile picture). Heroku is used for deloyment.

# Tools:
- [Bootstap](https://getbootstrap.com) - A CSS framework.
- [Django](https://www.djangoproject.com) - Backend framework in python.
- [PostgreSQL](https://www.postgresql.org) - A relational database system.
- [Heroku](https://www.heroku.com) - Deloyment.
- [AWS](https://aws.amazon.com) - S3 bucket.

## Getting Started

**Step 1: Clone the code into a fresh folder**

```
$ git clone https://github.com/bmbshlly/django-blogpost.git
$ cd django-blogpost
```

**Step 2: Create a Virtual Environment and install Dependencies**

Create a new Virtual Environment for the project and activate it. If you don't have the `virtualenv` command yet, you can find installation [instructions here](https://virtualenv.readthedocs.io/en/latest/).

```
$ virtualenv venv
$ source venv/bin/activate
```

Next, we need to install the project dependencies, which are listed in `requirements.txt`.

```
(venv) $ pip install -r requirements.txt
```

**Step 3: Run application**

Now we're ready to start our server which is as simple as:

```
(venv) $ python manage.py runserver
```

Open http://localhost:8000 (port number is prompted) to view it in your browser.

The app will automatically reload if you make changes to the code.
You will see the build errors and warnings in the console.(DEBUG = True)
