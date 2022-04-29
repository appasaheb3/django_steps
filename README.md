# django_steps
Important steps to create project ,app,migrate it and run it in django

## Create Project
	django-admin startproject myproject

## Run Server
	python manage.py runserver

## Run server Globally
	python manage.py runserver http:0.0.0.0:8000

## Create Application
	python manage.py startapp myapp

## Migrate Database
	python manage.py migrate

## Create Superuser
	python manage.py createsuperuser

## mysql coonectivity
	python-devel
	mysql-devel

## not showing static file .js .css
	python manage.py collectstatic

## view html file
	add in setting.py
	after BASE_DIR
	TEMPLATE_DIR = os.path.join(BASE_DIR,'templates')
	STATIC_DIR=os.path.join(BASE_DIR,'static')
	
	template block
	'DIRS': [TEMPLATE_DIR],

## Cookies Manually 
	It will be use in views function to handle the cookies
	Set Cookies
		request.session['username']
	Check keys
		request.session.has_key('username'):

	Get Value of cookies
		request.session['username']

	Session expire age setting.py 
	### SESSION AGE 5 Minutes
	SESSION_COOKIE_AGE = 5*60

## template 
	{% if status=='1' %}
	
	show variable
	{{ username }}
