Code Summary: Regex Data Validation in Python
This Python script demonstrates how to use regular expressions (regex) to validate four types of commonly encountered data: emails, URLs, phone numbers, and currency amounts.

 What It Does
The script defines four functions using the re (regex) module:

is_valid_email(email)

Checks if the given string is in a valid email format.

Example of valid input: user@example.com

is_valid_url(url)

Validates URLs starting with http:// or https://.

Example of valid input: https://www.example.com

is_valid_phone(phone)

Accepts US-style phone numbers in different formats:

(123) 456-7890

123-456-7890

123.456.7890

is_valid_currency(amount)

Validates US currency formats like:

$19.99

$1,234.56

 Test Data
A dictionary named test_data is used to simulate real-world input data for each type (email, URL, phone number, currency). Each value is tested using the corresponding validation function.

 Output
The script prints whether each test input is valid. For example:

pgsql
Copy
Edit
Email 'user@example.com' is valid? True
Phone '123.456.7890' is valid? True
Currency '$123456.78' is valid? False

 How It Works
Each function uses a regular expression pattern and Python’s re.match() to determine if the input fits the expected format.


