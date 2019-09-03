## Features

* Babel 7
* Environment Variables
* Express
* REST API

## Requirements

* [node & npm](https://nodejs.org/en/)
* [git](https://www.robinwieruch.de/git-essential-commands/)

## Installation

* `git clone git@github.com:rwieruch/node-express-server-rest-api.git`
* `cd node-express-server-rest-api`
* `npm install`
* `npm start`
* optional: include *.env* in your *.gitignore*

### GET Routes

* visit http://localhost:3000
  * /messages
  * /messages/1
  * /users
  * /users/1

### Beyond GET Routes

#### CURL

* Create a message with:
  * `curl -X POST -H "Content-Type:application/json" http://localhost:3000/messages -d '{"text":"Hi again, World"}'`
* Delete a message with:
  * `curl -X DELETE -H "Content-Type:application/json" http://localhost:3000/messages/1`

#### Postman

* Install [Postman](https://www.getpostman.com/apps) to interact with REST API
* Create a message with:
  * URL: http://localhost:3000/messages
  * Method: POST
  * Body: raw + JSON (application/json)
  * Body Content: `{ "text": "Hi again, World" }`
* Delete a message with:
  * URL: http://localhost:3000/messages/1
  * Method: DELETE
