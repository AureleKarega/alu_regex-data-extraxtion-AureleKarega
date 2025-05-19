Code Overview

 Regex Based Data Validation In Python:  

This python program presents regular expression (regex) validation of data types such as emails, URLs, phone numbers, and currency values that are commonly encountered.  

What It Does:  

The script uses re (regex) module to define four functions:  

def is_valid_email(email)  

Validates if email is in proper format  

Example of valid input: user@example.com  

def is_valid_url(url)  

Checks validity for URLs starting with http:// or https://.  

Example of valid input: https://www.example.com  

def is_valid_phone(phone)  

Validates (US) phone numbers in the following formats:  

(123) 456-7890  
123-456-7890  
123.456.7890  
  
def is_valid_currency(amount)  

Checks validity for US currency formats such as:  

$19.99  
$1,234.56  
  
Test Data:
The input data for each type (email, URL, phone number, currency) is stored in a dictionary named test_data which is used to mimic real life scenarios. Each value is tested using the corresponding validation functions.  

Output: 
The script checks all test inputs for validity and returns the result. For example:  

pgsql Copy Edit Email 'user@example.com' is valid? True Phone '123.456.7890' is valid? True Currency '$123456.78' is valid? False 

How It Works:
 Each function employs a regular expression patter and uses python's re.match() to execute the function.


