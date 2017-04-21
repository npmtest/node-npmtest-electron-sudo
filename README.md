# npmtest-electron-sudo

#### basic test coverage for  [electron-sudo (v4.0.12)](https://github.com/automation-stack/electron-sudo#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-electron-sudo.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-electron-sudo) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-electron-sudo.svg)](https://travis-ci.org/npmtest/node-npmtest-electron-sudo)

#### Electron subprocess with administrative privileges, prompting the user with an OS dialog if necessary.

[![NPM](https://nodei.co/npm/electron-sudo.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/electron-sudo)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-electron-sudo/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-electron-sudo/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-electron-sudo/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-electron-sudo/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-electron-sudo/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-electron-sudo/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-electron-sudo/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-electron-sudo/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-electron-sudo/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-electron-sudo/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-electron-sudo/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-electron-sudo/build/test-report.html](https://npmtest.github.io/node-npmtest-electron-sudo/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-electron-sudo/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-electron-sudo/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-electron-sudo/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-electron-sudo/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-sudo/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-sudo/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-electron-sudo/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-electron-sudo/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "electron-sudo",
    "version": "4.0.12",
    "description": "Electron subprocess with administrative privileges, prompting the user with an OS dialog if necessary.",
    "main": "./dist/index.js",
    "author": "Aleksandr Komlev",
    "license": "MIT",
    "repository": {
        "type": "git",
        "url": "git@github.com:automation-stack/electron-sudo.git"
    },
    "keywords": [
        "sudo",
        "os",
        "dialog",
        "prompt",
        "command",
        "exec",
        "ui",
        "electron",
        "elevate",
        "administrative",
        "privileges",
        "UAC",
        "subprocess"
    ],
    "bugs": {
        "url": "https://github.com/automation-stack/electron-sudo/issues"
    },
    "homepage": "https://github.com/automation-stack/electron-sudo#readme",
    "scripts": {
        "build": "node_modules/webpack/bin/webpack.js --config ./webpack/config.babel.js",
        "build-win32": "node node_modules\\webpack\\bin\\webpack.js --config webpack\\config.babel.js",
        "prepublish": "npm run test",
        "lint": "node_modules/eslint/bin/eslint.js -c .eslintrc ./src",
        "test-win32": "npm run build-win32 && node node_modules\\mocha\\bin\\mocha --compilers js:babel-core/register tests",
        "test": "npm run build && node_modules/mocha/bin/mocha --compilers js:babel-core/register ./tests"
    },
    "devDependencies": {
        "babel-cli": "^6.10.1",
        "babel-core": "^6.10.4",
        "babel-eslint": "^6.0.0",
        "babel-loader": "^6.2.4",
        "babel-plugin-array-includes": "^2.0.3",
        "babel-plugin-lodash": "^2.2.1",
        "babel-plugin-module-alias": "^1.2.0",
        "babel-plugin-syntax-async-functions": "^6.5.0",
        "babel-plugin-syntax-decorators": "^6.5.0",
        "babel-plugin-syntax-flow": "^6.8.0",
        "babel-plugin-syntax-object-rest-spread": "^6.5.0",
        "babel-plugin-transform-async-to-module-method": "^6.7.0",
        "babel-plugin-transform-class-properties": "^6.6.0",
        "babel-plugin-transform-decorators-legacy": "^1.3.4",
        "babel-plugin-transform-flow-strip-types": "^6.8.0",
        "babel-plugin-transform-regenerator": "^6.6.5",
        "babel-plugin-transform-runtime": "^6.6.0",
        "babel-polyfill": "^6.16.0",
        "babel-preset-es2015": "^6.9.0",
        "babel-preset-stage-0": "^6.5.0",
        "babel-runtime": "^6.9.2",
        "chai": "^3.5.0",
        "copy-webpack-plugin": "^3.0.1",
        "dirty-chai": "^1.2.2",
        "eslint": "^2.6.0",
        "eslint-loader": "^1.3.0",
        "eslint-plugin-babel": "^3.2.0",
        "estraverse-fb": "^1.3.1",
        "json-loader": "^0.5.4",
        "mocha": "^2.4.5",
        "raw-loader": "^0.5.1",
        "source-map-support": "^0.4.0",
        "webpack": "^1.12.14",
        "webpack-dev-server": "^1.14.1",
        "webpack-module-hot-accept": "^1.0.4",
        "webpack-shell-plugin": "^0.4.2"
    },
    "dependencies": {
        "babel-runtime": "^6.18.0",
        "bluebird": "^3.4.6"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
