# simple-node-app
A simple example node.js application to demonstrate my project structuring, coding patterns, and testing methodology.

## Getting Started

Prerequisites:
- Node.js installed natively on your computer ([download here](https://nodejs.org/)).
- Grab the repo and install node modules:

```shell
# clone the repo and install dependencies
$ git clone git@github.com:joshuarwynn/simple-node-app-again.git
$ cd simple-node-app-again && npm install
```
- Start the Node.js app by executing the following:

```shell
# run the node app
$ npm start
```

- Begin hitting the [routes](#routes) with `curl` or your favorite API testing tool.

## Testing

To run the full integration test suite, execute the following:

```shell
# run all integration tests
$ npm test
```

To run the full integration test suite with code coverage, execute the following:

```shell
# run all integration tests and generate coverage report
$ npm run coverage
```

To run the linter on all code, execute the following:

```shell
# run linter on all code
$ npm run lint
```

## Routes

### GET `/health`

A basic health check endpoint. Useful for system monitoring purposes.

#### Success Response

Sample Call: `curl localhost:3000/health`

Status Code: `200`

Response Body:
```
{
	"status": "healthy"
}
```
