mengunbakan WEB : https://www.saucedemo.com/

@login
Feature:Login
@valid_login
Scenario:Login using valid email and password
Givenuser is on login page
Anduser input username with "standard_user"
Anduser input password with "secret_sauce"
Whenuser click login button
Thenuser is on homepage
@invalid_login
Scenario:Login using invalid email and password
Givenuser is on login page
Anduser input username with "standard_user"
Anduser input password with "invalid"
Whenuser click login button
Thenuser able to see error message "Epic sadface: Username and password do not match any user in this service"
