# Ex02 Django ORM Web Application
## Date: 15-09-2025

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![alt text](<WhatsApp Image 2025-09-13 at 11.18.54_b13d4f67 - Copy.jpg>)

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
from . models import Car
# Register your models here.

admin.site.register(Car)

class CarAdmin(admin.ModelAdmin):
    list_display = ('car_id','brand','model','year','price')
```
```
models.py

from django.db import models

# Create your models here.
class Car(models.Model):
    car_id = models.IntegerField(primary_key=True)
    brand = models.CharField(max_length=20)
    model = models.CharField(max_length=20)
    year = models.DateTimeField()
    price = models.IntegerField()
```


## OUTPUT

![alt text](<Screenshot 2025-09-15 193859.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
