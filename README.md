# Payoff v0.0.1
Fixed-rate loan calculations made easy.

## Disclaimer
This library is in pre-alpha state, and is provided as-is, with no warranty or support of any kind. I am not a financial professional, and this library is not suggested for any production environments.

## Goals 
- Ease of use: A simple, dependency-free way to do basic loan payback calculations. It should help easily compare early payback situations on an existing loan, or different terms prospective loans for the same amount.
- *ES6* + *Babel*: This is my first attempt at using Ecmascript 6 (and Babel for legacy transpiling). Would like to make sure it’s making good use of the new features, while maintaining ES5 compatibility.
- *Docker* compilation: should be able to develop on any machine, using a containerized compiler defined in the repository.

## Development
The easiest way to compile this library's source code into the minified result is via *Docker* container. It will install the node application and all dependencies inside a virtual container. If you have *Docker* and *Docker Compose* installed, then a single command line...
```
# in root /payoff/ directory
docker-compose up
```
...will run a full build on the _/app/src_ source files, placing the result into _/app/dist_, and running the unit tests.

## TODO
- Implement the ability to add extra payments
- Asynchronous constructor option
- ~~Start generating documentation~~
- Figure out how to list via npm
- Create contribution guidelines
