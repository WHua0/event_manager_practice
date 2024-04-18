# Event Manager Practice

## Closed Issues
Github Issue Image Placeholder

[Github Closed Issues Link](https://github.com/WHua0/event_manager_practice/issues?q=is%3Aissue+is%3Aclosed)

### Closed Issue 1: Settings Max Login Attempts Description is Incorrect

![Github Issue 3](submissions/CodeMod1Issue.png)

![Code Modifications 3](submissions/CodeMod1.png)

[Github Issue 1 Link](https://github.com/WHua0/event_manager_practice/issues/10)

Description for max_login_attempts in class Settings in config.py incorrectly stated "Background color of QR codes". The description is updated to "Max number of login attempts".

### Closed Issue 2: Username Validation (TBD)
Github Issue Image Placeholder

Github Issue 2 Link

Github Code Modifications Placeholder

Github Test Codes Placeholder

Documentation

### Closed Issue 3: Password Validation is Missing No Spaces Allowed and Max Length
![Github Issue 3](submissions/CodeMod3Issue.png)

![Code Modifications 3](submissions/CodeMod3.png)

![Code Modification Result 3](submissions/CodeMod3Test.png)

[Github Issue 3 Link](https://github.com/WHua0/event_manager_practice/issues/4)

POST/register Register and POST/users Create User allowed passwords with spaces, and of unlimited lengths. Password validator in class UserCreate in user_schemas.py is updated to return ValueError if length of password is over 128 characters, or if a space is found within the password. This is to increase security.

### Closed Issue 4: Email Validation is Missing Max Length

Github Issue Image Placeholder

[Github Issue 4 Link](https://github.com/WHua0/event_manager_practice/issues/8)

Github Code Modifications Placeholder

Github Test Codes Placeholder

Documentation

### Closed Issue 5: Profile Picture Url Validation is missing Max Length, HTTPS/HTTP protocol, and Valid Domain 

![Github Issue 5](submissions/CodeMod5Issue.png)

![Code Modifications 5](submissions/CodeMod5.png)

![Code Modification Result 5](submissions/CodeMod5Test.png)

[Github Issue 5 Link](https://github.com/WHua0/event_manager_practice/issues/7)

POST/register Register and POST/users Create User allowed Profile Picture Url of no restriction except with image file extension. Profile Picture Url validator in class UserBase and class UserUpdate in user_schemas.py are updated to return ValueError if url is missing http or https, missing domain name, or containing an invalid domain name. Max Length of 2083 is also added to UserBase BaseModel. This is to increase security.

### Closed Issue 6: POST/register JSON Schema Example is Inconsistent
![Github Issue 6](submissions/CodeMod6Issue.png)

![Code Modifications 6](submissions/CodeMod6.png)

![Code Modification Result 6](submissions/CodeMod6Test.png)

[Github Issue 6 Link](https://github.com/WHua0/event_manager_practice/issues/1)

In POST/register Register request body, the test user is John Doe, however the test profile picture url was for Jane Smith.Class Config in class UserBase in user_schemas.py is corrected to reflect the test profile picture url of John Doe. This is for consistency.

### Closed Issue 7: POST/register HTTP 400 Detail Message is Missing Email Already In Use
![Github Issue 7](submissions/CodeMod7Issue.png)

![Code Modifications 7](submissions/CodeMod7.png)

![Code Modification Result 7](submissions/CodeMod7Test.png)

[Github Issue 7 Link](https://github.com/WHua0/event_manager_practice/issues/3)

HTTP 400 detail message stated "Username already exists" even when duplicate email returned HTTP 400. HTTPException detail in Router Post Register in user_routes.py is corrected to "Username or Email already in use". This is to provide an accurate error message.

### Closed Issue 8: POST/users Create User is Missing HTTP 400 and Detail Message for Email Already In Use

Github Issue Image Placeholder

[Github Issue 8 Link](https://github.com/WHua0/event_manager_practice/issues/12)

Github Code Modifications Placeholder

Github Test Codes Placeholder

Documentation

### Closed Issue 9: POST/users Get User is Missing Return Values for Full Name, Bio, and Profile Picture Url

Github Issue Image Placeholder

[Github Issue 9 Link](https://github.com/WHua0/event_manager_practice/issues/9)

Github Code Modifications Placeholder

Github Test Codes Placeholder

Documentation

### Closed Issue 10: POST/users Get Users is Missing HTTP 400 for Skip Integer Less Than 0, and Limit Integer Less Than or Equal to 0

Github Issue Image Placeholder

[Github Issue 10 Link](https://github.com/WHua0/event_manager_practice/issues/5)

Github Code Modifications Placeholder

Github Test Codes Placeholder

Documentation

### Closed Issue 11: PUT/users Update User is Not Functional

Github Issue Image Placeholder

[Github Issue 11 Link](https://github.com/WHua0/event_manager_practice/issues/6)

Github Code Modifications Placeholder

Github Test Codes Placeholder

Documentation

## Dockerhub
Dockerhub Image Placeholder

Dockerhub Link 

## Pytest Coverage
Pytest Coverage Image Placeholder

## Reflection
Documentation