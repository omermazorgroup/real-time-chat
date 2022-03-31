# Real Time Chat

Real Time Chat Application created with VueJS, Express, Socket IO and MongoDB/Mongoose/Mongo Altas.

## Features

- [Express](https://expressjs.com/) as the web framework on the server
- Implements stateless authentication with [JWT](https://jwt.io/) tokens
- Authenticates [JWT](https://jwt.io/) and social authentication using [Passport](http://www.passportjs.org/)
- Hashes passwords using the [bcryptjs](https://www.npmjs.com/package/bcryptjs) package
- Enables real time communication to the server using [Socket IO](https://socket.io/)
- [MongoDB](https://www.mongodb.com/) and [Mongo Atlas](https://www.mongodb.com/cloud/atlas) is used for storing and querying data
- [Concurrently](https://www.npmjs.com/package/concurrently) is used to run both the server and client at the same time
- [Vue JS](https://vuejs.org/) is used as the frontend framework
- [Heroku](https://www.heroku.com) is used for production deployment

## Installation

### Running Locally

_Ensure [Node.js](https://nodejs.org/en/) and [NPM](https://www.npmjs.com/) are installed_

1. Clone or Download the repository (Depending on whether you are using SSH or HTTPS)

```bash
$ git clone https://github.com/omermazorgroup/real-time-chat.git
$ cd real-time-chat
```

2. Install dependencies for root, client and server

> You will need to npm install in each directory in order to install the node module needed for each part of the project

> Directories Include: Root, Server & Client

3. Add .env file to server folder and fill out details according to the .env.example. See [configuration details](#configuration-setup) for social auth and database setup: **Note, this is mandatory for the application to run**

4. Set **NODE_ENV=development** and **HEROKU_DEPLOYMENT=false**

5. Start the application

```bash
$ npm run dev
```

Your app should now be running on [localhost:8080](localhost:8080).

## Configuration Setup

These configuration setups are necessary for the app to function correctly as intended. These configuration setups will be required to be added as environment variables for the server to make use of.

### Local Environment Variables (.env file)

For development you will need a .env file for environmental variables.

**_Note: These are required for the application to be setup correctly_**

```bash
NODE_ENV=development
HEROKU_DEPLOYMENT=false

DATABASE_URL=DATABASE_URL

EXPRESS_SESSION_KEY=EXPRESS_SESSION_KEY
JWT_SECRET=JWT_SECRET

GOOGLE_CLIENT_ID=GOOGLE_CLIENT_ID
GOOGLE_CLIENT_SECRET=GOOGLE_CLIENT_SECRET

FACEBOOK_CLIENT_ID=FACEBOOK_CLIENT_ID
FACEBOOK_CLIENT_SECRET=FACEBOOK_CLIENT_SECRET

PORT=PORT
```
