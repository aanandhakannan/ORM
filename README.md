# Ex02 Django ORM Web Application
NAME:AANANDHA KANNAN.S

REG NO 21224040003

## Date: 15/04/2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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

from django.db import models

from django.contrib import admin

class Movie(models.Model):

mid=models.IntegerField()

    mname=models.CharField(max_length=100)
    
    collection=models.IntegerField()
    
    year=models.IntegerField()
    
    rating=models.FloatField()

class MovieAdmin(admin.ModelAdmin):
    
    list_display=('mid','mname','collection','year','rating')

from django.contrib import admin

from .models import Movie,MovieAdmin

admin.site.register(Movie,MovieAdmin)



## OUTPUT

![Screenshot 2025-04-15 091712](https://github.com/user-attachments/assets/aa021b81-7d75-4ea7-af3e-9f6b9d4e9580)



## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
