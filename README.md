# Ex02 Django ORM Web Application
# Date:26/11/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
admin.py

from django.contrib import admin 
from .models import Car_Inventory, Car_InventoryAdmin 
admin.site.register(Car_Inventory, Car_InventoryAdmin)

models.py

from django.db import models 
from django.contrib import admin 

class  Car_Inventory(models.Model): 
    Car_Model = models.CharField() 
    Car_Type = models.CharField() 
    Mileage = models.IntegerField() 
    Engine_Type = models.CharField() 
    Make_Date = models.DateField() 
    

class Car_InventoryAdmin(admin.ModelAdmin): 
    list_display = ('Car_Model', 'Car_Type', 'Mileage', 'Engine_Type', 'Make_Date')  
```
# OUTPUT

<img width="1917" height="972" alt="nithyaorm" src="https://github.com/user-attachments/assets/d953a1a5-7f13-4685-9a03-fc421d6ddc6e" />

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
