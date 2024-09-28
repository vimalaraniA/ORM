# Ex02 Django ORM Web Application
## Date: 28/9/24

## AIM
To develop a Django application to store and retrieve data from a Bank database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![exp 2 img 1](https://github.com/user-attachments/assets/20965814-d1f0-4a35-8752-9d5a6518bfcc)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 customers.

## PROGRAM
admin.py
```
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```
models.py
```
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')


```

## OUTPUT

![exp 2 img 2](https://github.com/user-attachments/assets/226a1c2e-502d-4879-8448-d708c2e07018)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
