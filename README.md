## Ex02:Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity digram

## Procdure
### STEP 1:
Clone the problem from github.
### STEP 2:
create a new app.
### STEP 3:
Enter the code for admin.py and model.py.
### Step 4:
Execute Django admin and create student user.
## PROGRAM
```
admin.py

from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)

models.py

from django.db import models
from django.contrib import admin
class Student(models.Model):
    referencenumber=models.CharField(max_length=20,help_text="referencenumber")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()

class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```

## OUTPUT
![Screenshot from 2023-12-12 10-10-23](https://github.com/DivyaMunirathnamm/django-orm-app/assets/147474097/77a43f8a-e9fb-45a9-95ae-eeee28575cbc)

## RESULT
The program for creating a database using ORM has been executed sucessfully.

