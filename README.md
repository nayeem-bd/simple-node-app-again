# simple-node-app
A simple example node.js application to demonstrate my project structuring, coding patterns, and testing methodology.

## Getting Started

Prerequisites:
- Node.js installed natively on your computer ([download here](https://nodejs.org/)).
- Grab the repo and install node modules:

```shell
# clone the repo and install dependencies
$ git clone git@github.com:joshuarwynn/simple-node-app.git
$ cd simple-node-app && npm install
```

- Create a Twitter account and app ([create a Twitter app here](https://apps.twitter.com/)).
- Once your Twitter app is created, you'll need to grab the `Consumer Key (API Key)`, `Consumer Secret (API Secret)`, `Access Token`, and `Access Token Secret` from the "Keys and Access Tokens" tab in your Twitter app portal. Place these values into the respective properties in the `twitter` object within `src/config/default.json`. You can leave `src/config/test.json` as is.
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
