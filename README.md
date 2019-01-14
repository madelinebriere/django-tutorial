# Django Tutorial
## Maddie Briere
### What is Django?
Django is "a high-level Python Web framework that encourages rapid development and clean, pragmatic design." It is free, open-source, and very secure. It removes the hassle of Web development and lets you focus on your own app development. Learn more about this framework in this brief [presentation](https://docs.google.com/presentation/d/1IQ7Aoat-7xVT4wqCi2b76jSBOni0QtHpoJPGB0_Cni4/edit?usp=sharing).

### Why use Django?
Django has advantages and disadvantages like any framework. This [blog](https://hackernoon.com/advantages-and-disadvantages-of-django-499b1e20a2c5) explores some of the pros and cons.

| Pros           | Cons          | 
| ------------- |:-------------:| 
| Simplified framework     | Monolithic | 
| Founded on Python     | Components deployed together      |  
| Add-ons for user authentication | Bad design can cause slow performance     | 
| Scalable | |
| Versatile | | 

### Installation
Installation instructions are linked [here](https://docs.djangoproject.com/en/2.1/intro/install/).

Steps:
* Login to VM
* Install Python, Pip, and other libaries.
```bash
sudo apt-get update
sudo apt-get install pip
sudo apt-get install python
sudo apt-get install python3-venv
```
* Fork and install Django from ``https://github.com/django/django.git``
* Set up virtualenv, described [here](https://docs.djangoproject.com/en/2.1/intro/contributing/), using this script:
```bash
python3 -m venv ~/.virtualenvs/djangodev
source ~/.virtualenvs/djangodev/bin/activate
pip install -e django/ 
```
* Verify installation using 
```bash
$ python
>>> import django
>>> print(django.get_version())
```
### Explore the tutorial
The tutorial is linked [here](https://docs.djangoproject.com/en/2.1/intro/tutorial01/).

For a basic startup, run the following commands:
```bash
django-admin startproject mysite
cd mysite
python manage.py runserver
```
And navigate to 127.0.0.1:8000. Note that to see the start-up page, you will need to have your display linked to your VM or be running the VM graphically.

Steps in exploration:
* Creating the project
* Launching a development server
* Creating an app
* Writing your first view
* Setting up a database
* Creating and activating models
* Exploring users/admin

### Launch to production
Use the tutorial [here](https://codingstartups.com/deploy-django-nginx-gunicorn-postgresql-supervisor/) to deploy your project to production. It is *not* recommended to use the built-in Django development server as the production server. Third-party tools should be used for this purpose instead.

### Review the documentation
The Django documentation is available [here](https://docs.djangoproject.com/en/2.1/). It reviews the mechanics behind model, view and template layers, the development process, automated user interfaces, etc.
