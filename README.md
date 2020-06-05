## Unit 14: Sequelize Homework
# Reverse Engineering Code

## Description:
This application allows users to create an account with secure login and logout capabilities using Passport and Sequelize to store the user data in a MySQL database while the application itself can authenticate every login with Express and track the login status with sessions.

## User Story:
As a user, I want to sign-up, login and logout to become a member of this application.

## Credits:
Express, Express-session, MySQL, Sequelize, Passport, Passport-Local, BCryptJS

## Files:

* isAuthenticated.js restricts routes, will either send the user to the login page or request to the restricted route.
* Config.json - configuration to connect to the server/databases
* Passport.js - sign in with email and password 
* Index.js - Imports user login data and connects to DB
* User.js - Uses bcryptjs for password hashing and creates a secure user model
* Login.js make sures there is login data values and does a post, and will redirect you to the members page
* Members.js does a get request to make sure user is logged in
* Signup.js pulls up the form, validates email and password requirements and calls the signUpUser function
* Api-routes.js - includes sign-in, log-in and log-out routes while getting appropriate data for the client
* Html-routes.js checks whether user is signed in and/or has an account
* Package.json - has all the packages/dependencies and their versions information
* Server.js - requires packages and routes, creates express and configures middleware, and syncs the database
