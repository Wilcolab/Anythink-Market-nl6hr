# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

### 1. Clone the repo

Clone the repo using the any of the following commands below:

```bash
git clone https://github.com/ObelusFamily/Anythink-Market-nl6hr.git
```

Or

```bash
git clone git@github.com:ObelusFamily/Anythink-Market-nl6hr.git
```

### 2. Install Docker

Follow the instructions [here](https://docs.docker.com/get-docker/) to install Docker on your machine.

You can verify docker is ready by running the following commands in your terminal:

```
$ docker -v
$ docker-compose -v
```

### 3. Run the app

Run `docker-compose up` from the project root directory to load Anythink's backend and frontend.

If Docker is working correctly, the backend should be running and able to connect to your local database. You can verify this by pointing your browser to http://localhost:3000/api/ping. You should see a `304` response with the body `{"msg":"Pong! Seems like Everythink is working, great job!"}`.

To check the frontend, open http://localhost:3001/register in your browser. You should be able to see the registration page.
