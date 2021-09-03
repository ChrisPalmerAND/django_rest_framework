# django_rest_framework
To use this boilerplae:



Created a blank repository. 
CD into you repository in your chosen IDE.

Use ```git clone https://github.com/ChrisPalmerAND/django_rest_framework.git```

Then install the requirements using:

```pip3 install requirements.txt```

After that, run the following command to set up your database. 
```python3 manage.py migrate```


Set up an 'env.py' file and ensure it's in the git ignore.
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

If you would like to create this from scratch, then this is the tutorial I used.
Follow tutorial: 
https://medium.com/swlh/build-your-first-rest-api-with-django-rest-framework-e394e39a482c

