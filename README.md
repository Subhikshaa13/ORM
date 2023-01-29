# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:
![aqswxdfcgvhbjkml,;'](https://user-images.githubusercontent.com/118787344/212689267-a6c12d33-840c-423d-80cf-55b78d7315e6.png)



## DESIGN STEPS

###STEP 1:
Creating a table using required details in Django--ORM

###STEP 2:
Upload the python code.

###STEP 3:
push the code to github.



## PROGRAM:

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



## OUTPUT:
![Screenshot (10)](https://user-images.githubusercontent.com/118787344/212689784-090231a7-4873-43cc-806c-0cca3e27e2bb.png)





## RESULT:

Thus, the experiment was executed successfully..
