# Express API template

See application on Heroku: https://express-ame.herokuapp.com/v1/

[![Build Status](https://travis-ci.com/amezyane/express-api-template.svg?branch=master)](https://travis-ci.com/amezyane/express-api-template)
[![Coverage Status](https://coveralls.io/repos/github/amezyane/express-api-template/badge.svg?branch=master)](https://coveralls.io/github/amezyane/express-api-template?branch=master)
[![Maintainability](https://api.codeclimate.com/v1/badges/002953e899b88f88c10d/maintainability)](https://codeclimate.com/github/amezyane/express-api-template/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/002953e899b88f88c10d/test_coverage)](https://codeclimate.com/github/amezyane/express-api-template/test_coverage)
[![Build status](https://ci.appveyor.com/api/projects/status/9gtromynmdfju6l9?svg=true)](https://ci.appveyor.com/project/amezyane/express-api-template)

From the turorial: [How To Set Up An Express API Backend Project With PostgreSQL](https://www.smashingmagazine.com/2020/04/express-api-backend-project-postgresql/)

## How to run the app

1. Clone the repo.
1. To install the dependencies, run the command `yarn` if Yarn is installed on your computer, or, `npm i`, at the root of the project.
1. Open a terminal in the project root and run `yarn startdev`.

## How to test

Run `yarn test`.

## Commands 

`yarn prestart`: Build the content of the src folder.

`yarn start`: Start server from the build folder.

`yarn startdev `: Start server in development mode.

`yarn lint`: Shows linting issues found in JS files (see config in the file `.eslintrc.json`).

`yarn pretty`: Prettifies our code.

`yarn postpretty`: Runs the `lint` command with the `--fix` flag appended. This flag tells ESLint to automatically fix common linting issues.

See `package.json` for the detailed command lines. 

## NPM packages

### Transpiling ES6 to ES5

`@babel/cli`: A required install for using `babel`. It allows the use of Babel from the terminal and is available as ./node_modules/.bin/babel.

`@babel/core`: Core Babel functionality.

`@babel/node`: This works exactly like the Node.js CLI, with the added benefit of compiling with `babel` presets and plugins. This is required for use with nodemon.

`@babel/plugin-transform-runtime`: This helps to avoid duplication in the compiled output.

`@babel/preset-env`: A collection of plugins that are responsible for carrying out code transformations.

`@babel/register`: This compiles files on the fly and is specified as a requirement during tests.

`@babel/runtime`: This works in conjunction with `@babel/plugin-transform-runtime`.

### Linting

`eslint`: Check that the code respects syntax rules (defined in the config file `.eslintrc.json`) and reports errors in the console.

`eslint-config-airbnb-base`: Adds the style rules used by Airbnb.

`eslint-plugin-import`: Supports linting of ES2015+ (ES6+) import/export syntax, and prevent issues with misspelling of file paths and import names." (Required to use the plugin `eslint-config-airbnb-base`.)

`prettier`: Apply formatting rules to the code (these are defined in the config file `.prettierrc` ).

### Testing

`mocha`: Test runner.

`chai`: Used to make assertions.

`nyc`: Collect test coverage report.

`sinon-chai`: Extends chai’s assertions.

`supertest`: Used to make HTTP calls to our API endpoints.

`coveralls`: For uploading test coverage to coveralls.io.

### Others 

`nodemon`: Monitors our project source code and automatically restarts our server whenever it observes any changes.

`dotenv`: Reads an .env file and gives access to the environment variables defined inside.