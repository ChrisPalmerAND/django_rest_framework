# django_rest_framework


Created a blank repository. 

```django-admin startproject my_rest_api . ```
```django-admin startapp myhero ```
```python3 manage.py migrate```
```pip3 freeze > requirements.txt```

Set up an env.py file and ensure it's in the git ignore.
Add the following code to the env.py - make sure you change the secret key.

```import os 
  os.environ['SECRET_KEY'] = 'yoursecretkey'
```

In my_Rest_api settings.py, import os and change secret key to this.
```
import os
if os.path.exists('env.py'):
    import env

SECRET_KEY = os.environ.get('SECRET_KEY', '')
```
Follow tutorial: 
https://medium.com/swlh/build-your-first-rest-api-with-django-rest-framework-e394e39a482c

