# Django ORM Web Application

## AIM:

To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:

Include your ER diagram here

## DESIGN STEPS:

## STEP 1:

Clone the problem from github

## STEP 2:

create a new app

## STEP 3:

Enter the codefor admin.py and model.py

## Step 4:

Execute Django admin and create 10 employees

## PROGRAM:

Model.py:

```
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')  
```

Admin.py:

```
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```

## OUTPUT:

### SERVER OUTPUT:

![Screenshot 2023-06-05 232253](https://github.com/Abrinnisha6/django-orm-app/assets/118889454/2194097f-82b1-48f0-a350-8c0c9feff118)

### CLIENT OUTPUT:

![employee](https://user-images.githubusercontent.com/118889454/230270948-855713f5-15dd-4431-94b4-f5aeef00efce.png)

## RESULT:

Thus a Django application to store and retrieve data from a database using Object Relational Mapping(ORM) is developed.
