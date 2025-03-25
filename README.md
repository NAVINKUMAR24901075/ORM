# Ex02 Django ORM Web Application
# Date:24-03-2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2025-03-25 085622](https://github.com/user-attachments/assets/29e6e59d-c82f-4430-86d2-7510c707f267)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
models.py
from django.db import models
from django.contrib import admin
class Loan(models.Model):
   loan_id=models.CharField(max_length=8,primary_key="loan_id")
   loan_type=models.CharField(max_length=30)
   name=models.CharField(max_length=30)
   aadhar=models.CharField(max_length=10)
   account_number=models.CharField(max_length=10) 
   amount=models.CharField(max_length=30)

class LoanAdmin(admin.ModelAdmin):
    list_display=('loan_id','loan_type','name','aadhar','account_number','amount')

admin.py
from django.contrib import admin
from.models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)
```
# OUTPUT
![Screenshot 2025-03-24 130435](https://github.com/user-attachments/assets/829efc63-1527-4502-8c92-a8a9984c7b64)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
