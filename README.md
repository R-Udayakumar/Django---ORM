# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

## STEP 1:
Creating a table using required details in Django--ORM

## STEP 2:
Upload the python code.

## STEP 3:
Push the code to github
## PROGRAM
## Models.py
```html
from django.db import models
from django.contrib import admin
# Create your models here.

class student(models.Model):
    reference_no=models.CharField(max_length=75,help_text='Reference_No.')
    name=models.CharField(max_length=100,help_text='Name')
    email=models.EmailField(help_text='Email')
    age=models.IntegerField(help_text='Age')
    Class=models.IntegerField(help_text='Class')
class studentAdmin(admin.ModelAdmin):
    list_display=('reference_no','name','Class','age','email')
```
## Admin.py
```html
from django.contrib import admin
from .models import student,studentAdmin

# Register your models here.
admin.site.register(student,studentAdmin)
```
## OUTPUT
![image](https://user-images.githubusercontent.com/118708024/215467492-69f0e7fa-b3f5-4658-9c65-86c68f048230.png)
## RESULT
Thus, the Program is executed successfully.
