# Server Docs

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

# Client Docs

The Flutter app of the Project.

## Features

- user gets automatically created on first launch
- UUID is persisted with cache.
- Add transaction with all given validations and constraints.
- Credit money from admin, Debit money to admin & Transfer money to other users.
- Sort and Filter transactions by date, amount, type.
- Swipe down to reload the List of transactions to see the latest transaction status.

## Local Setup

    flutter pub get
    flutter run

This will install all the dependencies and start the app on your device or emulator. I have built the entire app using my smart phone as the emulator. If you want to do so [better than emulator] please make sure that your smart phone and your computer are connected to the same network. Also, make sure that you have enabled the developer options and USB debugging on your smart phone.
