# Ex02 Django ORM Web Application
## Date: 
28.02.2024
## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://github.com/Rajkumar28072005/ORM/assets/144980101/d89412b9-58ff-4216-9d03-871c78dc4a98)


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
```
from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
      sno=models.IntegerField(primary_key="sno");
      name=models.CharField(max_length=50);
      author=models.CharField(max_length=70);
      price=models.IntegerField();
      publisher=models.CharField(max_length=60);

class Book_DBAdmin(admin.ModelAdmin):
    list_display=("sno","name","author","price","publisher");
```

## admin.py
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

## OUTPUT

![image](https://github.com/Rajkumar28072005/ORM/assets/144980101/c1d477fd-963c-4d98-b83f-d7a952b7a47a)

## Result
Thus the program for creating a database using ORM hass been executed successfully

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
