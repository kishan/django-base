# django-base

This is base Django project to help kickstart a new webapp. It has a simple Django project set up without any apps.

## How to Setup Project


### 1. Create new repo from this template
Rename the repo to your project
![django-base-template-button](https://user-images.githubusercontent.com/10304626/171469020-b0ce32f0-11a8-45ff-a009-6c203343c3c1.png)


### 2. Clone the new repo
```
Ex. git clone git@github.com:kishan/new-django-webapp.git
```

### 3. Create your own virtual environment
  ```
 $ python3 -m venv venv
 $ source venv/bin/activate
```

### 4. Install requirements
`$ pip install -r requirements.txt`

### 5. Set environment variables
Create `.env` file based upon `.env_sample` and fill in variables
```
cp .env_sample .env
```
`DJANGO_SECRET_KEY`: you'll need to generate a new Django secret key which you can do via [Djecrety](https://djecrety.ir/)

### 6. Run server
We'll be using [localhost.run](localhost.run) which provides us with a publicly accessible URL to our Django app.
```
  $ python manage.py runserver
  $ ssh -R 80:localhost:8000 localhost.run
```
