# Ex02 Django ORM Web Application
## Date:21.12.2024 

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![alt text](<entity diagram.jpg>)


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
from .models import loan_db,loan_dbAdmin
admin.site.register(loan_db,loan_dbAdmin)

models.py


from django.db import models
from django.contrib import admin
class loan_db(models.Model):
    customer_id=models.CharField(max_length=20)
    customer_name=models.CharField(max_length=100)
    amount=models.IntegerField()
    acc_no=models.IntegerField()
    email=models.EmailField()

class loan_dbAdmin(admin.ModelAdmin):
    list_display=('customer_id','customer_name','amount','acc_no','email') 


```

## OUTPUT

![alt text](<Screenshot 2024-12-21 144729.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
