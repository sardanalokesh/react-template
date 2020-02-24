Empty React application wrapped in Docker. 

## What it is?

React project with Typescript bootstrapped by [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm run docker:dev:build`

Build docker configuration to run the app in the development mode. 

### `npm run docker:dev:up`

Run the app in the development mode.

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm run docker:prod:build`

Build the app for production.

Docker image ``react-ui`` will be the result of the build operation.

 > NOTE: ``BACKEND`` env variable is required to be set

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

## Other scripts

This scripts used in docker run/build processes.

### `npm start`

Run the app in the development mode.

### `npm run build`

Builds the app for production.
