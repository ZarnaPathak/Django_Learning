# Django_Learning
- Django is a Free and Open-Source Framework for building Web Apps with Python
- Time Saving and Code Efficiency because it comes with features like, The Admin Site and Authentication etc
- Architectural pattern that Django follows is MVT - Model View Template
  
  ![image](https://github.com/ZarnaPathak/Django_Learning/assets/112220757/8790db5c-6fa5-4937-87c2-7f6e00864572)
                   MVT [Model View Template]

  - **Model**
    It is responsible for defining the structure of your database, including the fields and behaviors of the data you are storing
  - **Views**
    Views in Django take requests and return responses, typically rendering a template with context data to be displayed to the user
  - **Template**
     This allows you to embed logic, such as loops and conditionals, directly within your HTML to display data from the model that has been passed to the template by the view

## Creating new Django Project
  - We use command **django-admin startproject ProjectName** to create new django project
  - For running Django Server we use command **python manage.py runserver** , It shows follwing page

    ![image](https://github.com/ZarnaPathak/Django_Learning/assets/112220757/1b2fe5e0-09c1-4b8a-bf27-67e05c048bd8)

## Apps in Django Project
  In a Django project, an App is a self-contained module that performs a specific function or set of related functions
- For creating Django App we use command **python manage.py startapp myAppName**
- It creates a directory of the AppName having certain files including **admin.py, apps.py, models.py, tests.py, views.py, __init__.py** etc
- These files are used for different purposes in our project
- Whenever we create new App for different functionalities we have to Register each Apps in **settings.py** of our main project directory

  ![image](https://github.com/ZarnaPathak/Django_Learning/assets/112220757/496e0495-b7e8-406c-aa86-43f2ce894c27)
  
  ## views.py
    This file contains function of any particular action on the webpage, it recieves request, processes it on particular function and returns web responce
  ## urls.py
    This file is created by user manually to map URLS in the views.py.
    It defines URL patterns and associates each pattern with a specific view, determining which code runs when a particular URL is visited. 
    The URLs created in every App are routed to **mainProject/urls.py** for defining url patterns of the entire Project, which links different app URL configurations to the main project's URL 
    structure.
