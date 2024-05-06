# geodatacube API

**[API Documentation](https://m-mohr.github.io/geodatacube-api/)**

## Repository

This repository contains a set of files formally describing the geodatacube API, each with a human-readable and easily browseable version:

* [openapi.yaml](openapi.yaml) provides the [OpenAPI](https://www.openapis.org/) 3.0 definition of the geodatacube API. See the table above for human-readable versions of the OpenAPI definition.
* The [assets](assets/) folder contains some useful additional files such as examples, crosswalks, or schemas. All of these are non-binding additions. The source of truth are the top-level specification files.

# Development

The `master` branch is the latest version and is the one to create Pull Requests against.

For development some tools can be used:

1. Install [node and npm](https://nodejs.org) - should run with any recent version
2. Run `npm install` in this folder to install the dependencies
3. Run the linter for the OpenAPI file with `npm test`. This will lint the files and check against some best-practices. It uses `spectral` in the background.
4. To show the files nicely formatted in a web browser, run `npm start`. It starts a server and opens the API specification rendered with ReDoc in a web browser.
5. To create a static HTML page (e.g. for hosting it on GitHub Pages), you can run `npm run build` and it will create a `redoc.html` in this folder.
