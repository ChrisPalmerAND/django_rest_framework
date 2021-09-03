# django_rest_framework
### To use this boilerplate:

Created a blank repository. 
CD into you repository in your chosen IDE.

Use ```git clone https://github.com/ChrisPalmerAND/django_rest_framework.git```

Then install the requirements using:

```pip3 install requirements.txt```

After that, run the following command to set up your database:

```python3 manage.py migrate```


Set up an 'env.py' file at the top level and ensure it's in the git ignore.
Add the following code to the env.py - make sure you change the secret key.

```import os 
  os.environ['SECRET_KEY'] = 'yoursecretkey'
```

In my_rest_api settings.py, you are importing this. 
```
import os
if os.path.exists('env.py'):
    import env

SECRET_KEY = os.environ.get('SECRET_KEY', '')
```

You will need to create yourself a superuser:

```python3 manage.py createsuperuser```

Fill in your details and then once you have a superuser, run the app using:

```python3 manage.py runserver```

Once the local host has opened, naviagate to 'localhostpath'/admin. This will take you to the content management system of django where you CRUD data. 



### If you would like to create this from scratch, then this is the tutorial I used.
Follow tutorial: 
https://medium.com/swlh/build-your-first-rest-api-with-django-rest-framework-e394e39a482c

