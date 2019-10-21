# back-end

Hi guys! Here is some documentation to help you figure out the API

This is the full url that you will need as a prefix to every request:
    https://bw-bucketlist.herokuapp.com/api

These are the endpoints available to you:

Users

POST /users/register
returns: object
function: adds user to database
Data structure:
  username: "" *required*
  password: "" *required*
  email: "" *optional*

POST /users/login
returns: object
function: verifies user is registered in the database, provides token to allow access to protected material
Data structure:
  username: "" *required*
  password: "" *required*
  email: "" *optional*

GET /users
returns: array
function: shows list of all users in database *must be logged in to view

GET /users/:id
returns: object
function: returns specified user by id *must be logged in to view

PUT /users/:id
returns: object
function: updates specified user information **NOTE: password cannot be changed! *must be logged in to change

DELETE /users/:id
returns: object
function: removes user from database **NOTE: this is irreversible! *must be logged in to remove 




