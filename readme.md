# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

<!-- **[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_ -->
# To run the application locally on your desktop

### 1. Install Docker

You can install Docker for your system on [this link](https://docs.docker.com/get-docker/).

### 2. Once you have installed Docker

- Verify docker is ready by running the following commands in your terminal: 

``` docker -v ```
``` docker-compose -v```

- Then, run the given command from the project root directory to load Anythink's backend and frontend.

``` docker-compose up ```

- If Docker is working correctly, the backend should be running and able to connect to your local database.
- Test this by pointing your browser to [http://localhost:3000/api/ping](http://localhost:3000/api/ping).

### 3. Check Front-end

- To check the frontend and make sure it’s connected to the backend, visit [http://localhost:3001/register](http://localhost:3001/register)

- If everything is working properly, you’ll be able to create a new user on the given link.

- NOTE: Make sure that you run all scripts in the next quests on one of the containers created by ```docker-compose up```.  Also, you can use ```docker exec ``` to run commands on a running container.
