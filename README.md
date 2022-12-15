# [Finance REST API](https://miniproject.cf/)

Cloud Computing mini-project that implements a cloud application which provides useful financial insights related of stock market listed companies.

<br />


The mini project works on the following aspects of Cloud applications:
<ul>
<li>REST-based service interface for CRUD operations </li>

<li>Interaction with external REST services.  </li>

<li>Use of an external Cloud database for persisting information. (GCP used here). </li>
</ul>

<br />


## Build from sources

> **Step #1** - Clone sources (this repo)

```bash
$ # Clone the sources
$ git clone https://github.com/KarshVashi/FinanceRestApi
$ cd FinanceRestApi
```

<br />


> **Step #2** - Install dependencies

```bash
$ # Install requirements
$ pip3 install -r requirements.txt
```

<br />

<!-- > **Step #3** - Create Tables (SQLite persistance)

```bash
$ # Create tables
$ flask shell
$ >>> from app import db
$ >>> db.create_all()
```

<br /> -->

> **Step #4** - (optional) Enable DEBUG Environment (local development)

```bash
$ # Set up the DEBUG environment
$ # (Unix/Mac) export FLASK_ENV=development
$ # (Windows) set FLASK_ENV=development
$ # (Powershell) $env:FLASK_ENV = "development"
```

<br />

> **Step #5** - Start the project

```bash
$ # Run the application
$ # --host=0.0.0.0 - expose the app on all network interfaces (default 127.0.0.1)
$ # --port=5000    - specify the app port (default 5000)  
$ flask run --host=0.0.0.0 --port=5000
$
$ # Access the app in browser: http://127.0.0.1:5000/
```



<br />

## Code-base structure

The project has a super simple structure, represented as bellow:

```bash
< PROJECT ROOT >
   |
   |-- app/
   |    |-- static/
   |    |    |-- <css, JS, images>    # CSS files, Javascripts files
   |    |
   |    |-- templates/
   |    |    |
   |    |    |-- index.html           # Index File
   |    |    |-- login.html           # Login Page
   |    |    |-- register.html        # Registration Page
   |    |    |-- navigation.html 
   |    |    |-- footer.html   
   |    | 
   |    |     
   |   config.py                      # Provides APP Configuration 
   |   forms.py                       # Defines Forms (login, register) 
   |   models.py                      # Defines app models 
   |   views.py                       # Application Routes 
   |
   |-- requirements.txt
   |-- run.py
   |
   |-- ************************************************************************
```

<br />

Credits for Login and Register auth system:
https://github.com/app-generator/sample-flask-auth-session.git
