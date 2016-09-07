##DJANGO PRIMER

<http://etherpad.io/django-training>

framework built on pythong to make web applications easier with ORM (object relational model) = backed by a database but you interact with objects and classes (not with SQL)

DRF (Django Rest Framework) allows you to build APIs simply

MVT - Model View Template (Python)
* template - view in mvc
* model (bigger)
* view - a controller (smaller)

MVC - model View Controller (JS)

* controller takes a request and returns a response
* model is the representation of a table
* view is returned, by controler

class is an agregation or collection of certain properties - like a project (title, name), person (type, name)

object - calls constructor `__init__`

self = this

* whenever you create functions that belong to a class, the first argument is (self)
* when you're calling that method, you don't need to pass anything in, it's implied
* inheritance - you can have specializations of classes `Developer(Person)` <- inherits all properties and functions of person
* super = call base classes constructor


###Setup
Use python 3 - provides virtual environment in tool itself

setup your VE 

`pyvenv env` - creates a director that stores all project dependencies

`pip install django` - install django in that directory, you only need this in the beginning

`django-admin startproject mofo` - start project subcommand; mofo is the name

This generates a scaffolding for your project.

mofo directory and `manage.py` (specific to django that allows you to run all django commands)
`__init__.py` - empty file, makes packages out of a directory...in any scripts, you can require, mofo.settings

`urls.py` all accessible url configs
`wsgi.py` layer between your server and django

I usually change base directory to `app` by convention, holds all contents

Define your requirements (packag.json), `requirements.txt` in python

`pip install -r requirements.txt` for other people to install dependencies