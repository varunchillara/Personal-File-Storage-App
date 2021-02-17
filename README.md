# Personal File Storage Application
Personal File Storage is an application that allows the user to store and retrieve files and personal notes.

1. **File Storage:** Upload/download/remove files
2. **Note Management:** Add/update/remove text notes
3. **User Credential Management:** Save, edit, and delete website credentials.

## Tech/framework used

**Built With**
- Java 8
- Spring Boot
- Spring Security
- MyBatis
- Junit
- Selenium

### The Back-End
The back-end of the application works to connect the front end to the database and neatly helps to communicate the two.

1. The application uses Spring Security to manage user authorization
- Using Spring Security, the application restricts everyone to the login and signup pages until they make an account.

2. The application handles front-end calls using controllers
- The controllers for the application bind data and functionality to the front-end.
- The controllers are also responsible for determining what error messages the application displays to the user if there is any kind of error.

3. The application makes calls to the database with the use of the MyBatis framework
- MyBatis is used to map the POJO classes into the database.


### The Front-End
The front-end uses html, css, javascript and thymleaf to create a seamless interface which allows the user to manage files, notes and credentials.

1. Login page
- Everyone has access to the login page. If the user already has an account the user can log in directly.
- This page shows log in errors if an error occurs.


2. Sign Up page
- Everyone has access to the sign up page. This page allows users to create an account which is then added to the database.
- The signup page stores the password encrypted and stores the key along with it.


3. Home page
   The home page hosts the file service, note service and credential service.

i. Files
- The user is able to upload files and is able to see any files that have been previously uploaded.
- The user can delete any files that have been uploaded under the user's account.

ii. Notes
- The user can upload personal notes and see a list of the user's notes.
- The use can edit and delete any note that has been created under the user's account.

iii. Credentials
- The user can create credentials for websites.
- When the user inputs a password it in encrypted.
- The user is able to edit and delete credentials.
- When the user views the credential the password is decrypted.

### Build Project
These commands are used to run the project in a mac or linux environment.
 - clean - `make __clean`
 - package - `make package`
 - run selenium tests - `make run-selenium-tests`
 - run locally - `make run-local`

These commands are used to run the project in a window's environment.
- clean - `make __clean-win`
- package - `make package-win`
- run selenium tests - `make run-selenium-tests-win`
- run locally - `make run-local-win`




