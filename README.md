# [Flask Pixel UI Kit](https://appseed.us/apps/flask-apps/flask-pixel-bootstrap-uikit)

> Open-Source web app coded in Flask on top of [Pixel UI kit](https://themesberg.com/product/ui-kits/pixel-lite-free-bootstrap-4-ui-kit) (free version) - Starter generated by AppSeed [Web App Generator](https://appseed.us/app-generator).

## Features

- UI-Ready, Jinja2 templating
- SQLite database, Flask-SQLAlchemy ORM
- Session-Based auth flow (login, register)
- UI Kit: **[Pixel UI kit](https://themesberg.com/product/ui-kits/pixel-lite-free-bootstrap-4-ui-kit)** by **Themesberg**
- Support via **Github** and [Discord](https://discord.gg/fZC6hup).

<br />

> Links

- [Flask Pixel UI Kit](https://appseed.us/apps/flask-apps/flask-pixel-bootstrap-uikit) - product page
- [Flask Pixel UI Kit - Demo](https://flask-pixel-bootstrap-uikit.appseed.us/) - LIVE Deployment

<br />

![Flask Pixel UI Kit - Open-Source web app coded in Flask.](https://raw.githubusercontent.com/app-generator/flask-pixel-bootstrap-uikit/master/media/flask-pixel-bootstrap-uikit-screen.png)

<br />

## Prepare your environment

The product is built on top of [Flask](https://palletsprojects.com/p/flask/), a popular Python Web Framework. To build the app, we need a basic tool-chain installed in the workstation: 

- [Python3](https://www.python.org/) - the programming language used to code the app
- [Git](https://git-scm.com/) - used to clone the source code from the Github repository
- Basic development tools (g++ compiler, python development libraries ..etc) used by Python to compile the app dependencies in your environment.

<br />

> Check Python (using the terminal)

```bash
$ # Check Python version
$ python --version
Python 3.7.2 # <--- All good
```

<br />

> Check GIT command tool (using the terminal)

```bash
$ # Check git
$ git --version
$ git version 2.10.1.windows.1 # <--- All good
```

<br />

For more information on how to set up your environment please access the below links. In case we've missed something, contact us on [Discord](https://discord.gg/fZC6hup).

- [How to set up Python](/how-to/install-python)
- [Setup CentOS for development](/how-to/setup-centos-for-development/)
- [Setup Ubuntu for development](/how-to/setup-ubuntu-for-development/)
- [Setup Windows for development](/how-to/setup-windows-for-development/)

<br />

## Build from sources

```bash
$ # Clone the sources
$ git clone https://github.com/app-generator/flask-pixel-bootstrap-uikit.git
$ cd flask-pixel-bootstrap-uikit
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
$
$ # Install requirements
$ pip3 install -r requirements.txt
$
$ # Set the FLASK_APP environment variable
$ (Unix/Mac) export FLASK_APP=run.py
$ (Windows) set FLASK_APP=run.py
$ (Powershell) $env:FLASK_APP = ".\run.py"
$
$ # Set up the DEBUG environment
$ # (Unix/Mac) export FLASK_ENV=development
$ # (Windows) set FLASK_ENV=development
$ # (Powershell) $env:FLASK_ENV = "development"
$
$ # Run the application
$ # --host=0.0.0.0 - expose the app on all network interfaces (default 127.0.0.1)
$ # --port=5000    - specify the app port (default 5000)  
$ flask run --host=0.0.0.0 --port=5000
$
$ # Access the app in browser: http://127.0.0.1:5000/
```

> Note: To use the app, please access the registration page and create a new user. After authentication, the app will unlock the private pages.

<br />

## Code-base structure

The project has a super simple structure, represented as bellow:

```bash
< PROJECT ROOT >
    |
    |--- app/__init__.py
    |--- app/
    |     | --- <static/assets>
    |     |       |
    |     |       |--- <css>
    |     |       |--- <Js>
    |     |       |--- <img>
    |     |
    |     | --- <templates>
    |     |       |
    |     |       |---<includes>                   # Page chunks, components
    |     |       |     |
    |     |       |     | --- navigation.html      # Top bar
    |     |       |     | --- sidebar.html         # Left sidebar
    |     |       |     | --- scripts.html         # JS scripts common to all pages
    |     |       |     | --- footer.html          # The common footer
    |     |       |
    |     |       |---<layouts>                    # App Layouts (the master pages)
    |     |       |     |
    |     |       |     | --- base.html            # Used by common pages like index, UI
    |     |       |     | --- base-fullscreen.html # Used by auth pages (login, register)
    |     |       |
    |     |       |---<accounts>                   # Auth Pages (login, register)
    |     |       |     |
    |     |       |     | --- login.html           # Use layout `base-fullscreen.html`
    |     |       |     | --- register.html        # Use layout `base-fullscreen.html`  
    |     |       |
    |     |    index.html                          # The default page
    |     |    page-404.html                       # Error 404 page (page not found)
    |     |    page-500.html                       # Error 500 page (server error)
    |     |    *.html                              # All other pages provided by the UI Kit
    |
    |--- requirements.txt
    |
    |--- run.py
    |
    |-----------------------------
```

<br />

## Flask Pixel - App screens

> UI Beautiful cards

![Flask Pixel - UI Beautiful cards](https://raw.githubusercontent.com/app-generator/flask-pixel-bootstrap-uikit/master/media/flask-pixel-bootstrap-uikit-screen-1.png)

> Hero Section

![Flask Pixel - Hero Section](https://raw.githubusercontent.com/app-generator/flask-pixel-bootstrap-uikit/master/media/flask-pixel-bootstrap-uikit-screen-2.png)

> More Cards

![Flask Pixel - Hero Section](https://raw.githubusercontent.com/app-generator/flask-pixel-bootstrap-uikit/master/media/flask-pixel-bootstrap-uikit-screen-5.png)

<br />

## Credits & Links

<br />

## What is [Flask](https://www.palletsprojects.com/p/flask/)

[Flask](https://www.palletsprojects.com/p/flask/) is a lightweight WSGI web application framework. It is designed to make getting started quick and easy, with the ability to scale up to complex applications. It began as a simple wrapper around Werkzeug and Jinja and has become one of the most popular Python web application frameworks.

<br />

## [What is dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))

A dashboard is a set of pages that are easy to read and offer information to the user in real-time regarding his business. A dashboard usually consists of graphical representations of the current status and trends within an organization. Having a well-designed dashboard will give you the possibility to act and make informed decisions based on the data that your business provides - *definition provided by Creative-Tim - [Free Dashboard Templates](https://www.creative-tim.com/blog/web-design/free-dashboard-templates/?ref=appseed)*.

<br />

## [Pixel Lite](https://themesberg.com/product/ui-kits/pixel-lite-free-bootstrap-4-ui-kit)

Pixel is a free, fully responsive and modern Bootstrap 4 UI Kit that will help you build creative and professional websites. Use our components and sections, switch some Sass variables to build and arrange pages to best suit your needs - *crafted by [Themesberg](https://themesberg.com/?ref=appseed)*.

<br />

---
[Flask Pixel UI Kit](https://appseed.us/apps/flask-apps/flask-pixel-bootstrap-uikit) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
