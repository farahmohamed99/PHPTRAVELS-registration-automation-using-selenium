# PHPTRAVELS-registration-automation-using-selenium

A test automation script that automates testcases with a set of conditions and checks the website’s efficiency using selenium automation tool , Jupyter notebook , Chrome web driver, unittest,  and Python.

Running the tests :


1- Download the repository as a zip file.


2- Upload the zip file on jupyter notebook.

3- To unzip the file you have to create a notebook and run this code and a folder named "Pixelogic_Assignment" will be created:

    import zipfile
    with zipfile.ZipFile("PHPTRAVELS-registration-automation-using-selenium-main.zip","r") as zip_ref:
        zip_ref.extractall("Assignment")
        
 4- Delete the reports and logs folders to create new ones.
 
 5- Open the cmd and install the following packages :
 
    •	pip install selenium
   
    •	pip install unittest

    •	pip install ipynb

    •	pip install htmltestrunner

    •	pip install os-sys

    •	pip install json

    •	pip install Pillow==2.2.2

    •	pip install Faker

    •	pip install random
   
    •	pip install requests

    •	pip install time
    
 
 6- Run test.ipynb.
 
 
Components and features :


    •	Python

    •	Selenium

    •	Chrome web driver

    •	HTML test runner (reports generator)

    •	Requests 

    •	Os

    •	json

    •	PIL

    •	Faker (data generator)

    •	random

    •	Time



The project consists of 6 python files :



1-	Locator :- contains 3 classes, Each class represents a page that contains 
    all the information needed for each element to access.
    Ex: (By.NAME , 'firstname').
    
    
    

2-	Elements :- contains 9 classes. A base class that represents one element on the page and fill it with the specified value, the other classes represent all the textboxes and     inherits from the base class to be filled with the data.
    Ex: Firstname textbox = ‘ Stefan’.
    
    
    
    

3-	Page :-  contains 4 classes, a base class and 3 other classes that represent the pages ex: register page , login page and account page.



4-	Utlis :- contains the helper functions and variables that are needed.



5-	Test :- contains 1 class that contains all the testcases.



Testcases :

•	def test_firstname_empty(self), def test_lastname_empty(self), def test_phone_empty(self), def test_email_empty(self), def test_password_empty(self), def test_confirmpassword_empty(self) :

    6 testcases, each testcase will leave a textbox empty.


•	def test_firstname_lower(self) , def test_lastname_lower(self), def test_password_lower(self) :

    3 testcases that let all the letters pf the word in lowercase.


•	def test_firstname_firstletter_upper(self), def test_lastname_firstletter_upper(self) :

    2 testcases that let only the first letter of the word in uppercase.


•	def test_firstname_upper(self), def test_lastname_upper(self), def test_password_upper(self) :

    3 testcases that let all the letters of the word in uppercase.


•	def test_firstname_equal_lastname(self), def test_password_equals_confirmpassword(self) :

    2 testcases that matches between 2 textboxes (password & confirmed password).


•	def test_phone_less_than_10(self) :

    1 testcase that let the length of the phone number less than 10.


•	def test_phone_10_letters(self) :

    1 testcase that has a length but letters.


•	def test_phone_valid(self) :

    1 testcase that is a valid phone number.


•	def test_email_invalid1(self) ,  def test_email_invalid2(self), def test_email_invalid3(self), def test_email_invalid4(self) :

    4 testcases with invalid structure of an email. 

        ex: missing ‘ . ’ , missing ‘ @ ’ , swap between ‘ @ ’ and ‘ . ’ , same order of the ‘ @ ’ and ‘ . ’ but with no word between them.


•	def test_redundant_email(self):

    1 testcases that has the same email as another testcase by saving the email of the other testcases in a txt file and check if it’s matching or not .


•	def test_email_valid(self):

    1 testcases with a valid email structure.


•	def test_password_more_than_8(self):

    1 testcase with a password length more than 8.


•	def test_password_less_than_6(self):

    1 testcase with a password length less than 6.


•	def test_valid_password(self):

    1 testcase with a valid structure of a password which contains at least 1 capital and 1 small letter with length less than .


•	def test_password_not_equals_confirmpassword(self):

    1 testcase with different password and confirmed password.


•	def test_Validation_login(self):

    1 testcase with successful registration followed by a login.


    After running all the testcases a report will be created with screenshots for failures.
