# npmdoc-koa-validate

#### basic api documentation for  [koa-validate (v1.0.7)](https://github.com/RocksonZeta/koa-validate#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-koa-validate.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-koa-validate) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-koa-validate.svg)](https://travis-ci.org/npmdoc/node-npmdoc-koa-validate)

#### A koa params validate middleware.

[![NPM](https://nodei.co/npm/koa-validate.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/koa-validate)

- [https://npmdoc.github.io/node-npmdoc-koa-validate/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-koa-validate/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-koa-validate/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-koa-validate/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-koa-validate/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-koa-validate/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/RocksonZeta/koa-validate/issues"
    },
    "dependencies": {
        "json-path": "^0.1.3",
        "validator": "^5.2.0"
    },
    "description": "A koa params validate middleware.",
    "devDependencies": {
        "coveralls": "*",
        "istanbul-harmony": "0",
        "koa": "*",
        "koa-body": "*",
        "koa-router": "*",
        "mocha": "*",
        "mocha-lcov-reporter": "*",
        "should": "*",
        "supertest": "^0.13.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0b7dd3feee83cae1b4694fa06376477d945eb430",
        "tarball": "https://registry.npmjs.org/koa-validate/-/koa-validate-1.0.7.tgz"
    },
    "engines": {
        "node": ">= 0.11.9"
    },
    "gitHead": "a44b4fb8738595530f729e5d9407b725c1a49537",
    "homepage": "https://github.com/RocksonZeta/koa-validate#readme",
    "keywords": [
        "web",
        "koa",
        "koa-validate",
        "validate",
        "validator",
        "format",
        "middleware"
    ],
    "license": "MIT",
    "main": "validate.js",
    "maintainers": [
        {
            "name": "rocksonzeta"
        }
    ],
    "name": "koa-validate",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/RocksonZeta/koa-validate.git"
    },
    "scripts": {
        "test": "NODE_ENV=test mocha --harmony --require should --reporter spec",
        "test-cov": "NODE_ENV=test node --harmony ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha -- --require should",
        "test-travis": "NODE_ENV=test node --harmony ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha --report lcovonly -- --require should"
    },
    "version": "1.0.7",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
