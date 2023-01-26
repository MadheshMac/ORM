# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![madesh](https://user-images.githubusercontent.com/119828952/214765182-660072c3-4bc6-4108-98dc-8b36d6d35fe2.png)


## DESIGN STEPS

### STEP 1:
Create a table usingrequired details in Django-ORM


### STEP 2:
Upload the python code

### STEP 3:
Push the code to github




## PROGRAM

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



## OUTPUT
![Screenshot (15)](https://user-images.githubusercontent.com/119828952/214765243-4ddbaa70-80e3-422a-ba10-a68fc8d5d1b5.png)





## RESULT
Thus,the experiment was completed successfully
