# Server

This is the server of the Project. It is an express server with Typescript and Mongoose.

## Features

- add user with unique UUID
- fetch user with UUID
- create transaction with all given validations and constraints
- credit money from admin, Debit money to admin & Transfer money to other users.
- sort and Filter transactions by date, amount, type.
- fetch all the transactions of a certain user

## Important

in case you do not have a mongoDB server running on your local machine then add a .env file in the root directory of the server and add connect from mongo atlas.

## Local Setup

    yarn
    yarn dev

this will install all the dependencies and start the server on [localhost:8080](http://localhost:8080).
Then we need to create the admin user and set there balance to 1000000. To do that we need to go to <http://localhost:8080/api/users> and add a record with uuid as "admin" and update the balance to "1000000" (you can use postman for this).
