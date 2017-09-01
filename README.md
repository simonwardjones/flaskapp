# Flask Mega tutorial

[Mega Tutorial Link](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)

## lesson 1 - Hello world

**Summary:**

- Install python
- Install virtualenv
- Create virtualenv

Now start the app:
- Create the app/\_\_init__.py file \*\*
- Create the app/views.py file
- Create a run.py file (to launch the app to local host)

\*\*
Files named \_\_init__.py are used to mark directories on disk as Python package directories
This ensures that all python files in such a directory can be imported using . notation
```python
import app.views as views
```
or using the from construction 
```python
from app import views as v
```

**Code snippets:**

Either with pip or conda
```commandline
pip install virtualenv
virtualenv flask
```

Then pip in the packages as below
I could activate and then just use `pip install package_name`

```commandline
flask_python/bin/pip install flask
flask_python/bin/pip install flask-login
flask_python/bin/pip install flask-openid
flask_python/bin/pip install flask-mail
flask_python/bin/pip install flask-sqlalchemy
flask_python/bin/pip install sqlalchemy-migrate
flask_python/bin/pip install flask-whooshalchemy
flask_python/bin/pip install flask-wtf
flask_python/bin/pip install flask-babel
flask_python/bin/pip install guess_language
flask_python/bin/pip install flipflop
flask_python/bin/pip install coverage
```

## lesson 2 - Templates

**Summary:**

- Create Static and Template folders
- Create a template called index
- Change the view to use render_template
- Pass params to template using {{ param_name }}
- Control block in template {% if bool%} ... {% else %} .. {% endif %}
- Loops in templates {% for post in posts %} .. {% endfor %}
- Template inheritance (keep common nav etc...)


**Code snippets:**

Make dirs using terminal command
```commandline
mkdir app/static app/templates
```

## lesson 3 - Web Forms

**Summary:**

- Create Config.py folder
- Add forms settings for extra security
- Add forms.py module and create a form class 
(note the From class we subclass from is now called FlaskForm)
- Add a login html template which uses a form instance as a variable
