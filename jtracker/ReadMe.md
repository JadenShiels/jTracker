# install django

python -m pip install django

# start new project

django-admin startproject jtracker

# run project

cd jtracker/jtracker
python manage.py runserver

# this will show a url the development sever

# add site

cd jtracker (directory with manage.py)
python manage.py startapp jsite

# Add website to the INSTALLED_APPS in settings.py

# URL path in urls.py
python manage.py runserver
http://127.0.0.1:8000/welcome.html

# How to Use Python Requests with REST APIs
# https://www.nylas.com/blog/use-python-requests-module-rest-apis/
pip install requests
