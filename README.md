## [Live Demo](https://django-blogpost.herokuapp.com)

# Introduction

Blogpost is a web application backed by Django where every user can create, update and delete post on the feed(with timestamp). New users can set profile picture(also update later). Users can reset password via registered e-mail.  
Application uses PostgreSQL(relation database) to store user information and their blogs. AWS is used to store static files(profile picture). Heroku is used for deloyment.

[<img src="https://github.com/bmbshlly/django-blogpost/blob/main/giphy.gif" width="480" height="270">](https://django-blogpost.herokuapp.com)
<img src="https://github.com/bmbshlly/django-blogpost/blob/main/reset_pass.png" width="470" height="270">

## Tools:
- [Bootstrap](https://getbootstrap.com) - A CSS framework.
- [Django](https://www.djangoproject.com) - Backend framework in python.
- [PostgreSQL](https://www.postgresql.org) - A relational database system.
- [Heroku](https://www.heroku.com) - Deloyment.
- [AWS](https://aws.amazon.com) - S3 bucket, IAM.
- [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) - Let browser to access AWS bucket.

## Key features:
- Authentication (register, login, logout)
- Reset password via SMTP (mail received with reset password link!)
- Create, update, delete post with timestamp (only author can edit)
- Pagination (per page 5 post) - navigation to first, previous 3, current, next 3 and last page in the bottom
- Profile update with picture
- View all post by a user in page.



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

Try hosted app [here.](https://django-blogpost.herokuapp.com)
