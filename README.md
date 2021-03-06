# Reaktor preassignment 2020 backend

a REST api created using NodeJS, that parses the `status.real`-file
and exposes it in JSON format.

## API usage:
Send `GET` requests to `address`/api/`packageName`, replacing `packageName` with the name of the package, or leaving it empty to get a list of all indexed packages.
If the package is not found, the API will return a **404** and a JSON object containing the error message.
If the request is not a GET request the API will return a **405** error.
### Example calls:
Address: `http://localhost:9001/`

Get all packages : `GET` `http://localhost:9001/api/`

Get a package called 'at' : `GET` `http://localhost:9001/api/at`

### Run project: `npm start`
**NOTE:** The server requires the environment variable `PORT` to be set to a port number that you want the server to listen to.

### [Frontend demo site](https://reaktor-preassignment-frontend.herokuapp.com/)
### [Backend demo site](https://reaktor-preassignment-backend.herokuapp.com/api/)

