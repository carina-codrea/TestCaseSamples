# Test Case Samples

Below are some Test Case samples that I wrote while working on previous projects.

-------------

## Login ##

**Title:**
Test login with correct credentials

**Description:**
Check if the login works with correct credentials.

**Steps to reproduce:**
1. Go to site.com/login
2. Add correct user/pass
3. Press login button

**Expected result:**
User should be able to login and is taken to his profile page.

**Test data:**
User: test &
Pass: 12345678

---------------------------

**Title:**
Test login with incorrect credentials

**Description:**
Check if the login works with incorrect credentials.

**Steps to reproduce:**
1. Go to site.com/login
2. Add incorrect user/pass
3. Press login button

**Expected result:**
User shouldn't be able to login and the validation message: "Incorrect username or password" is displayed.

**Test data:**
User: test2 &
Pass: 45678901

---------------------------

**Title:**
Test login without credentials 

**Description:**
Check if the login works without credentials.

**Steps to reproduce:**
1. Go to site.com/login
2. Leave the username and password fields blank
3. Press login button

**Expected result:**
User shouldn't be able to login.This validation message should be displayed :"Username or password is incorrect."

**Test data:**

---------------------------

**Title:**
Test if password is hidden

**Description:**
Check if the password is in a masked form when typed in the password field.

**Steps to reproduce:**
1. Go to site.com/login
2. Add password in the password field
3. Observ if the password is masked

**Expected result:**
The password should be in a masked form.

**Test data:**
Pass: 12345678

--------------------------

**Title:**
Test back button after logging in

**Description:**
Check if once logged in, clicking the back button doesn't log out the user.

**Steps to reproduce:**
1. Go to site.com/login
2. Add correct user/pass
3. Press login button
4. Click back button

**Expected result:**
User shouldn't be logged out after clicking the back button.

**Test data:**
User: test &
Pass: 12345678

--------------------------

**Title:**
Test "remember me" checkbox

**Description:**
Check if the user is logged in after checking the "remember me" check box,logging in with correct credentials, leaving and accessing the page again.

**Steps to reproduce:**
1. Go to site.com/login
2. Add correct user/pass
3. Check "remember me" checkbox
4. Press login button
5. Leave the page without logging out
6. Visit the page again

**Expected result:**
User should be logged in if the session did not expire.

**Test data:**
User: test &
Pass: 12345678

--------------------------

**Title:**
Test login session timeout duration

**Description:**
Check the login session timeout duration so that once logged in a user cannot be authenticated for a life-time.

**Steps to reproduce:**
1. Go to site.com/login
2. Add correct user/pass
3. Press login button
4. Spend more time than the session timeout duration on that page

**Expected result:**
User should be logged out after the session expire and should take him to login page.
This message should be displayed: "Your session has expired.".

**Test data:**
User: test &
Pass: 12345678

--------------------------

**Title:**
Test login page responsiveness

**Description:**
Check if the login page is responsive.

**Steps to reproduce:**
1. Go to site.com/login
2. Right click on the page
3. Click on Inspect
4. Try different dimensions and devices

**Expected result:**
The login page should adjust to different screen resolutions and devices.

**Test data:**


--------------------------

**Title:**
Test access of a user profile without being logged in

**Description:**
Check if the user can access his profile page without being logged in.

**Steps to reproduce:**
1. Go to site.com/test

**Expected result:**
User should be redirected to the login page.

**Test data:**


--------------------------

**Title:**
Test the limit of unsuccessful login attempts

**Description:**
Check if there is a limit on the total number of unsuccessful login attempts so that the user cannot try all possible combinations of username-password.

**Steps to reproduce:**
1. Go to site.com/login
2. Add incorrect user/pass
3. Repeat step 2 multiple times

**Expected result:**
User shouldn't be able to try to login again until the specified time expires and this message should be displayed: "Too many failed login attempts.Please try again later."

**Test data:**
User: test2 &
Pass: 45678901

--------------------------

**Title:**
Test "lost your password?" link

**Description:**
Check if the lost your password? link is working corectly and landing on the correct page.

**Steps to reproduce:**
1. Go to site.com/login
2. Click on "lost your password?" link

**Expected result:**
User should be redirected on the forgot password page.

**Test data:**


--------------------------

**Title:**
Test if the login page elements are as per specification

**Description:**
Check if the size,color, and UI of the different elements are as per specifications.

**Steps to reproduce:**
1. Go to site.com/login
2. Observe the elements

**Expected result:**
All the elements should be how it was specified.

**Test data:**
*Specification*

--------------------------

## Search  ##

**Title:**
Test search with invalid search

**Description:**
Check if search is functional and displaying a suggestion message to help the user try to find what he is searching for and an error message by adding a invalid search.

**Steps to reproduce:**
1. Go to https://www.emag.ro/
2. Introduce a non-existing value in the search input
3. Press enter

**Expected result:**
This messages should be displayed:\

Error:\
"0 rezultate pentru 'value' "

Suggestion:\
"Pentru a gasi produsul dorit, incearca urmatoarele:
- Verifica daca ai scris corect termenii.
- Incearca sa folosesti sinonime.
- Incearca din nou, folosind o cautare mai generala."

**Test data:**
Value: sdfsdfsf

--------------------------

**Title:**
Test search with a valid search

**Description:**
Check if search is functional and generating the correct results by adding a valid search.

**Steps to reproduce:**
1. Go to https://www.emag.ro/
2. Introduce an existing product in the search input
3. Press enter

**Expected result:**
The right results should be shown for the searched product.

**Test data:**
Value: tricou dama

--------------------------

**Title:**
Test auto suggest

**Description:**
Check if suggestions are shown or not when adding a keyword in the search input.

**Steps to reproduce:**
1. Go to https://www.emag.ro/
2. Introduce a keyword in the search bar

**Expected result:**
Some suggestion should appear based on the keyword that was introduced.

**Test data:**
Value: tricou

--------------------------

**Title:**
Test autocomplete

**Description:**
Check if after typing at least three characters from the value you want to search for, it will be autocompleted.

**Steps to reproduce:**
1. Go to https://www.emag.ro/
2. Introduce at least three characters

**Expected result:**
When user starts typing the value in the search input and after introducing at least three characters, the value should be autocompleted.

**Test data:**
Value: telefon

--------------------------
