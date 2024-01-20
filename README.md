# CRUD_Proglint

A simple Crud operation using React with html and css


This Crud application named 'Shoppyfy' is an  react application which consist of Login page, sign up page followed by (List,Create,Update,Delete) of all the products with the help of Crudcrud.com


Only an authenticated user's alone can access the Crud application (Shoppyfy).

For Authentication i've used Jwt token based authentication by storing all the registered users in mongodb atlas cloud database and to validate the authenticated user as well.


Once the User successfully loggned into the application a token will be set in the local storage with expiration of 1day, once the user logout the token will be removed and it will redirect to the login page.

(auto login)
If the user  loggned into the landing page (main page) he/she can't go back to the login page, until they logout or token get's expired.


This application consist of Browser router to navigate through different sections of the application ( Add, update, login, signup, home, logout )




To run this application:-

Download the ZIP code

It consist of two folder client and server

open an individual terminal for each client and server and give the command to install node modules "npm i"

after the command 'npm i' --> npm run start. data base will gets connected and frontend also starts to run




--> Create a new credentials with the sign up page and login into the system (Token will gets generated)

---> Add product drives you to add the product  to the product list 
---> Edit drives you to the updates particular product  to the product list 
---> home component consist of list of products
---> Delete -> deletes specific product from the list





note : while running server if it throughs error like 'DeprecationWarning: The `punycode` module is deprecated. Please use a userland alternative instead.'


follow this step:

go to node modules of server application
search - tr46 - tr46 (index.js) -> replace with const punycode = require("punycode/");



