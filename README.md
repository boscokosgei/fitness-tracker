## A Fitness tracking app Created in Python to Track workout sessions

## Prerequisite
 - Python
 - Linux

 ## Tools
 - Python --version 3.8 above
 - pip installed
 - VS code

 The final application will look like this
 ![Images](Live%20workout%20app.png)

## Workflow of The application
1. A webpage will be available for users to fill in their activities and submit the form
2. The data will be sent to Django.
3. Django views function will receive and validate date and finally store in database.
4. The page will display the workout once pulled from the database for viewing.
5. Django will render a data to HTML so that it will be displayed.

## Step 1. Creating a Virtual Environment
Create the Repo on Github and clone it to local machine
```sh
    git clone https://github.com/boscokosgei/fitness-tracker
```
Navigate into the directory
```sh
   cd fitness-tracker
   code .
```
Creating Python Virtual Environment
```sh
   python3 -m venv venv
```
Activate the virtual environment
```sh
   source venv/bin/activate
```

Installing Django
```sh
   pip install django
   python3 -m django --version

```
## Step 2. Creating the Project
The environment is setup now it time to create the project
```sh
   django-admin startproject fitness_project .
```

Running the development server to test everything is ok
```sh
    python manage.py runserver
```

## Step 3. Creating a Django APP
Run this command on terminal to create a project inside django container
```sh
   python manage.py startapp tracker
```
It will create a folder of the project with modules such as 
- models.py
- views.py
- admin.py 