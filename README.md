# Ex02 Django ORM Web Application
## Date: 31-10-2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM

### models.py

```html
from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Height=models.IntegerField()
    Position=models.CharField(max_length=100)

class Player_Admin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Height','Position')
```

### admin.py
```html
from django.contrib import admin
from .models import Player,Player_Admin
admin.site.register(Player,Player_Admin)

```

## OUTPUT

![image](https://github.com/SandeepaNagaraj/ORM/assets/113017853/035d7368-8fca-4192-bf3f-12a22e1029d9)

![image-1](https://github.com/SandeepaNagaraj/ORM/assets/113017853/347d85a0-c505-4633-9d25-7c1e9e1f3c14)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
