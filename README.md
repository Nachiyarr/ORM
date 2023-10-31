# Ex02 Django ORM Web Application
## Date: 14-10-23

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).



##  STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM

# Admin.py
```


from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```
# Models.py
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

## OUTPUT
![Screenshot 2023-10-27 182733](https://github.com/Nachiyarr/ORM/assets/113497340/02dfad95-21d3-4867-9a86-b11314e21905)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
