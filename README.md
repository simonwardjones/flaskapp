# Lesson 2

- I recreated the same env on mac using commandline 
```commandline
conda install virtualenv
```

then once again pip in the packages. could activate and then just use `pip install package_name`

```commandline
flask/bin/pip install flask
flask/bin/pip install flask-login
flask/bin/pip install flask-openid
flask/bin/pip install flask-mail
flask/bin/pip install flask-sqlalchemy
flask/bin/pip install sqlalchemy-migrate
flask/bin/pip install flask-whooshalchemy
flask/bin/pip install flask-wtf
flask/bin/pip install flask-babel
flask/bin/pip install guess_language
flask/bin/pip install flipflop
flask/bin/pip install coverage
```
now add database packages:
```commandline
flask/bin/pip install psycopg2 
flask/bin/pip install sqlalchemy-datatables
```
# Project Diverges into two branches
1. Master branch will stay with the tutorial
2. SiScout branch will try to create scout visualisation

