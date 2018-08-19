# Origin Branch

Based on CoreUI React Template.

## Installation

``` bash
# clone the repo
# cd into app's directory
# install app's dependencies
$ npm install
```

### Basic usage

``` bash
# dev server  with hot reload at http://localhost:3000
$ npm start
```

Navigate to [http://localhost:3000](http://localhost:3000). The app will automatically reload if you change any of the source files.

### Build

Run `build` to build the project. The build artifacts will be stored in the `build/` directory.

```bash
# build for production with minification
$ npm run build
```

### Deploy

```bash
$ npm run deploy
```

https://github.com/gitname/react-gh-pages
 - the master branch holds the source code
 - the gh-pages branch holds the built app code.
 - package.json > scripts >
   - "predeploy": "npm run build",
   - "deploy": "gh-pages -d build"

## Command Summary

| Command               | Description                                               |
| :-------------------- | :-------------------------------------------------------- |
| npm start             | start a development server for the demo app               |
| npm test              | run tests                                                 |
| npm run test:coverage | run tests and produce a code coverage report in coverage/ |
| npm run test:watch    | start a test server and re-run tests on every change      |
| npm run build         | prepare for publishing to npm                             |
| npm run clean         | delete built resources                                    |

## What's included

Within the download you'll find the following directories and files, logically grouping common assets and providing both compiled and minified variations. You'll see something like this:

```
CoreUI-React#v2.0.0
├── public/          #static files
│   ├── assets/      #assets
│   └── index.html   #html temlpate
│
├── src/             #project root
│   ├── containers/  #container source
│   ├── scss/        #user scss/css source
│   ├── views/       #views source
│   ├── App.js
│   ├── App.test.js
│   ├── index.js
│   ├── _nav.js      #sidebar config
│   └── routes.js    #routes config
│
└── package.json
```

## Troubleshooting

- If `npm test` produces `Error: EMFILE: too many open files, watch`, then to fix: `brew install watchman`. Reference: https://github.com/facebook/create-react-app/issues/4540
