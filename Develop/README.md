# Kequelize Kreverse Kengineering 14


[![Github Badge](https://img.shields.io/badge/GitHub-Profile-blueviolet?style=plastic&logo=appveyor)](https://github.com/KBrazier2)


## Table of Contents


[Description](#Description)

[Installation](#Installation)

[Usage](#Usage)

[Licenses](#Licenses)

[Explanation](#Explanation)

[Contributors](#Contributors)

[Tests](#Tests)

[Questions](#Questions)

[Link](#Link)

[Screenshots](#Screenshots)

## Description

For this assignment, we were tasked with reverse engineering the starter code provided and to create a tutorial for the code.

This application allows users to create an account, log into said account, and sign out securely. All user data is stored in a MySQL database.


## Installation

To begin using this application, please clone repository into your local storage. Once this is complete, please follow the following steps:

- Create a MySQL database called "passport_demo"
- Open config.json and insert personal data such as username, password, etc.
- Install "npm i" and node packages
- Run "node server.js" to connect to server
- Open "http://localhost:8080" in browser address bar


## Usage

AS A user who wants to safely log into "x" site

I WANT to be ensured that my personal data is securely stored

SO THAT I do not have to worry about using "x" site.


## Licenses

N/A

## Explanation

CONFIG

MIDDLEWARE

isAuthenticated.js {Restricts user's routes without proper log in credentials. Once proper credentials provided, restrictions are lifted.}

config.json {Connection configuration to connect to server.}

passport.js {Contains Javascript logic which informs passport of request to log in with proper credentials.}

MODELS

index.js {Connects to database and imports user's credential data}

user.js {Requires "bcyrpt" for password hashing. Allows database to be secure even if compromised. Includes Javascript which defines what is stored to database.}

ROUTES

api-routes.js {Contains routes for logging in, logging out, and obtaining user's specific data to be displayed client side.}

html-routes.js {Routes confirming proper user log in, otherwise redirected.}

package.json {Contains all package info, node modules, version info, etc.}

server.js {Requires npm packages, sets up PORT, creates express and middleware, creates routes and syncs database / logs message in terminal on successful connection.}


## Contributors

Kyle Brazier


## Tests

N/A


## Questions

You may reach me at kylebrazier@gmail.com for further questions.

## Link

https://youtu.be/JVxnj04HOQs

## Screenshots
![screenshot1](./2020-10-04.png)

