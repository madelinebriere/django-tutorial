# Django Tutorial
## Maddie Briere
### What is Django?
Django is "Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design." It is free and open source.

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
* Install Python and Pip
```bash
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

Steps in exploration:
* Creating the project
* Launching a development server
* Creating an app
* Writing your first view
* Setting up a database
* Creating and activating models
* Exploring users/admin
