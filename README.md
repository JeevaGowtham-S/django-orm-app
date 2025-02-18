# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Fork and clone the repository in to your IDE
### STEP 2:
Cteate a django project and an aap and a superuser account and run the server.
### STEP 3:
Modify the changes in settings and write your code on models and admin and run the server.
### STEP 4:
Login into admin using your superuser account and populate the records

## PROGRAM

```
from django.db import models
from django.contrib import admin

# Create your models here.
class Grocery(models.Model):
    brandname = models.CharField(max_length=100,primary_key= True)
    weight = models.CharField(max_length=100)
    mrp= models.CharField(max_length=80)
    manufacturedate = models.DateField()
    expiredate = models.DateField()

    
class GroceryAdmin(admin.ModelAdmin):
    list_display = ('brandname','weight','mrp','manufacturedate','expiredate')
```

## OUTPUT 
 ![Output](./images/grocrey.png)
 ![Output](./images/er.png)

## RESULT:
Thus we developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
