# Ex02 Django ORM Web Application

## Date: 
 Name: Hari prasath.R.K

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot 2024-04-04 214853](https://github.com/Hariprasath2023/ORM/assets/145207783/7b663e63-95ed-4d88-9806-98957d1d5333)



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
models.py

from django.db import models
from django.contrib import admin
class bookdetails(models.Model):
       bookid=models.IntegerField()
       bookname=models.CharField(max_length=25)
       author=models.CharField(max_length=20)
       publishedyear=models.DateField()
       price=models.IntegerField()
       publishedcompany=models.CharField(max_length=20)
class bookdetailsAdmin(admin.ModelAdmin):
      list_display=("bookid","bookname","author","publishedyear","price","publishedcompany")

admin.py

from django.contrib import admin
from .models import bookdetails,bookdetailsAdmin
admin.site.register(bookdetails,bookdetailsAdmin)


```

## OUTPUT

![Screenshot 2024-04-04 214904](https://github.com/Hariprasath2023/ORM/assets/145207783/eef7b579-a314-4504-8466-d19a586f472a)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
