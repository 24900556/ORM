# Ex02 Django ORM Web Application
## Date: 12.03.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).




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
admin.py

from django.contrib import admin
from .models import movie,movieAdmin
admin.site.register(movie,movieAdmin)

models.py

from django.db import models
from django.contrib import admin
class movie(models.Model):
    movieid=models.CharField(max_length=20,help_text="Employee ID")
    moviename=models.CharField(max_length=100)
    date_of_release=models.DateField()
    genre=models.CharField(max_length=30)
    lang=models.CharField(max_length=20)


class movieAdmin(admin.ModelAdmin):
    list_display=('movieid','moviename','date_of_release',' genre','lang')
```


## OUTPUT

![Screenshot 2025-05-20 093350](https://github.com/user-attachments/assets/cae37dee-fd56-419a-808c-67cc1d1359a1)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
