# reverse_Engineering.io

## --USER STORY--

As a user that has gone through security issues with passwords on web pages. This app allows the ability to login safely without any future issues with my privacy. This app safely store my personal information so that I don’t have to worry.  
 

## --TECH USED --

-BCRYPTJS -EXPRESS -EXPRESS-SESSION -MYSQL2 -PASSPORT -PASSPORT-LOCAL -SEQUELIZE

## --PASSWORD AUTHENTICATION--

This app allows users to log in and out safely and securely. Data is stored through the mysql database.   



# --GETTING STARTED--

## To start using this app, clone this repository into your local storage. Once you have done this follow these steps;

1)Clone repository to your local machine.

2)Create a mysql db called "passport_demo".

3)Open config.json within the config file, and insert your personal data username, password.

4)Open the terminal in current the repo and run "npm i" to install all node packages, double check to make sure everything is installed. 

5)Run "node server.js" in the terminal.

6)Open the browser and type "http://localhost:8080" in the search bar.

# --FILES EXPLAINED--

## CONFIG/MIDDLEWARE

isAuthenticated.js = [ 
    This javascript file restricts the user from using routes unless they are logged in. If the user is logged in the routes will work and process the request.];

config.json = [Configuration to connect to the server ];

passport.js = [this contains javascript logic that tells passport that we are trying to log in. It lets passport know that we are using an email and password to access the the page.];
________
## MODELS 

index.js = [Connects to the database and imports the users login data];

user.js = [ This requires "bcrypt" for password hashing. This makes our database secure even if it is compromised. In this file we hae a javascript that defines what all is stored in our database.];

___________________________________
## ROUTES

api-routes.js = [ This javascript file contains routes for signing in, logging out and getting users specific data to be displayed client side. ];

html-routes.js = [ This javascript file contains routes that check whether user is signed in. This also checks whether user already has account or not, and sends them to the correct html page ];

package.json = [ This javascript file contains all package info, version info, and node modules used];

server.js = [ This file: requires packages, sets up PORT, creates express and middleware. This file also creates routes and syncs to the database and it logs message in the terminal on successful connection to server ];

