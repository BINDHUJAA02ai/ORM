# Ex02 Django ORM Web Application
## Date: 26/03/2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## DIAGRAM
![Screenshot 2025-04-08 135323](https://github.com/user-attachments/assets/80e288da-fd43-4e9f-b664-b1500dd6993e)

## DESIGN STEPS


### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
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
admin.py
```
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```


## OUTPUT
![alt text](<ormapp/Screenshot 2025-03-26 204447.png>)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
