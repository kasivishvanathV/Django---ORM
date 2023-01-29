# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![](ENTITY%20RELATIONSHIP%20DIAGRAM.png)

## DESIGN STEPS

### STEP 1:
Creating a table using required details in Django--ORM.

### STEP 2:
Upload the python code.

### STEP 3:
push the code to github.
Write your own steps

## PROGRAM

```
admin.py:  

from django.contrib import admin  
from .models import Student,StudentAdmin  


admin.site.register(Student,StudentAdmin)  

manage.py:  

from django.db import models  
from django.contrib import admin  
#Create your models here.  

class Student(models.Model):  
    referencenumber=models.CharField(max_length=10,help_text="Your Reference Number")  
    name=models.CharField(max_length=100)  
    department=models.CharField(max_length=200)  
    age=models.IntegerField()  
    email=models.EmailField()  

class StudentAdmin(admin.ModelAdmin):  
    list_display = ('referencenumber','name','age','department','email')  
#Register your models here.  
```

## OUTPUT

![](Screenshot%20(30).png)


## RESULT
ORM has been done successfully
