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

Github Code Modifications Placeholder

Github Test Codes Placeholder

Github Issue 2 Link

Documentation

### Closed Issue 3: Password Validation is Missing No Spaces Allowed and Max Length
![Github Issue 3](submissions/CodeMod3Issue.png)

![Code Modifications 3](submissions/CodeMod3.png)

![Code Modification Result 3](submissions/CodeMod3Test.png)

[Github Issue 3 Link](https://github.com/WHua0/event_manager_practice/issues/4)

POST/register Register and POST/users Create User allowed passwords with spaces, and of unlimited lengths. Password validator in class UserCreate in user_schemas.py is updated to return ValueError if length of password is over 128 characters, or if a space is found within the password. This is to increase security.

### Closed Issue 4: Email Validation is Missing Max Length

![Github Issue 4](submissions/CodeMod4Issue.png)

![Code Modifications 4](submissions/CodeMod4.png)

![Code Modification Result 4](submissions/CodeMod4Test.png)

[Github Issue 4 Link](https://github.com/WHua0/event_manager_practice/issues/8)

POST/register Register and POST/users Create User allowed emails of unlimited lengths. Email in class UserBase in user_schemas.py is updated to have a maxlength of 255. This is to increase security.

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

POST/register Register HTTP 400 detail message stated "Username already exists" even when duplicate email returned HTTP 400. HTTPException detail in Router Post Register in user_routes.py is corrected to "Username or Email already in use". This is to provide an accurate error message.

### Closed Issue 8: POST/users Create User is Missing HTTP 400 and Detail Message for Email Already In Use, and Update Detail Message for Duplicate User

![Github Issue 8](submissions/CodeMod8Issue.png)

![Code Modifications 8](submissions/CodeMod8.png)

![Code Modification Result 8](submissions/CodeMod8Test.png)

[Github Issue 8 Link](https://github.com/WHua0/event_manager_practice/issues/12)

POST/users Create User returns HTTP 500 instead of HTTP 400 when using a duplicate email. Router Post Create User in user_routes.py is updated to return HTTP 400 "Email already in use" when using a duplicate email after checking for a duplicate username. This is to provide an accurate error message.

POST/users Create User HTTP 400 detail message stated "Username already exists" when using a duplicate username. HTTPException detail in Router Post Create User in user_routes.py is updated to "Username already in use". This is for consistency with POST/register Register in Closed Issue 7.

### Closed Issue 9: POST/users Get User is Missing Return Values for Full Name, Bio, and Profile Picture Url

![Github Issue 9](submissions/CodeMod9Issue.png)

![Code Modifications 9](submissions/CodeMod9.png)

![Code Modification Result 9](submissions/CodeMod9Test.png)

[Github Issue 9 Link](https://github.com/WHua0/event_manager_practice/issues/9)

GET/users Get User By ID returned incorrect null values for Full Name, Bio, and Profile Picture Url for existing user. Router Get User By ID in user_routes.py is updated to return the three missing values from the User database.

### Closed Issue 10: POST/users Get Users is Missing HTTP 400 for Skip Integer Less Than 0, and Limit Integer Not More Than 0

![Github Issue 10](submissions/CodeMod10Issue.png)

![Code Modifications 10](submissions/CodeMod10.png)

![Code Modification Result 10](submissions/CodeMod10Test.png)

[Github Issue 10 Link](https://github.com/WHua0/event_manager_practice/issues/5)

GET/users List User returned HTTP 200 for Skip Integer less than 0, and Limit Integer not more than 0. Router List Users in user_routes.py is updated to return HTTP 400 instead of HTTP 200 for invalid input. This is to provide an accurate error message.

### Closed Issue 11: PUT/users Update User is Not Functional

![Github Issue 11](submissions/CodeMod11Issue.png)

![Code Modifications 11](submissions/CodeMod11.png)

![Code Modification Result 11](submissions/CodeMod11Test.png)

[Github Issue 11 Link](https://github.com/WHua0/event_manager_practice/issues/6)

Documentation

## Dockerhub
Dockerhub Image Placeholder

Dockerhub Link 

## Pytest Coverage
Pytest Coverage Image Placeholder

## Reflection
Documentation