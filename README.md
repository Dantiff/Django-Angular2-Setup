# Django + AngularJS-2 Basic Setup

Please find the live application <a href="http://bivestventures.pythonanywhere.com/"> HERE </a>

This is a boilerplate project for using AngularJS-2 with Django. The project was inspired by the  hardships faced by most people while trying to integrate the Django and AngularJS frameworks to work together. The setup can be downloaded and used as the starter settings for any Django-Angular projects in future. The procedure to implementation of this setup is gven as follows:

### Features

* Django backend in `./core`
* AngularJS 2 (v4) frontend in `./ngApp`
* Support and integration of both Jinja2 and Django template engines
* Jinja2 Template with variales from django and angular
* Testing support using Karma and Lite-Servers
* Makefile to make your life easy


### Development environment setup

Ensure you have the latest versions of <a href="https://help.pythonanywhere.com/pages/Node/"> npm and node (v4 and above) </a> to esure you can run es5 scripts without errors since VueJS is based on the es5 syntax.

Foremost, be sure to create a virtual environment for your project since the default python instance available will be used. Use the mkvirtualenv command as follows:

```bash
$ mkvirtualenv nenv
```

Install database client. For MySQL, istallation is given as follows:

For Python 2.7

```bash
$ pip install mysql-python
```

For Python 3.x

```bash
$ pip install mysqlclient
```

The requirements.txt file is meant to reduce the number of commands to execute.

These steps will install all required dependencies including development ones, run migrations and start dev server.


## Project Setup
```python
#Create a new Virtual Environment.
virtualenv appenv
cd appenv

#Fork or clone this repo.
git clone https://github.com/Dantiff/Django-Angular2-Setup.git
cd Django-Angular2-Setup/ngApp/

#prepare the debelopment env
make install

#Open a new terminal window
cd ../

#Migrate and Run Development Server
make run
```






