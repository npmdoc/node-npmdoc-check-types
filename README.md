# npmdoc-check-types

#### api documentation for  [check-types (v7.1.5)](https://github.com/philbooth/check-types.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-check-types.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-check-types) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-check-types.svg)](https://travis-ci.org/npmdoc/node-npmdoc-check-types)

#### A little library for asserting types and values.

[![NPM](https://nodei.co/npm/check-types.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/check-types)

- [https://npmdoc.github.io/node-npmdoc-check-types/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-check-types/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-check-types/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-check-types/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-check-types/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-check-types/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Phil Booth",
        "url": "https://github.com/philbooth"
    },
    "bugs": {
        "url": "https://github.com/philbooth/check-types.js/issues"
    },
    "contributors": [
        {
            "name": "Phil Booth",
            "url": "https://github.com/philbooth"
        },
        {
            "name": "Rowan Manning",
            "url": "https://github.com/rowanmanning"
        },
        {
            "name": "Forbes Lindesay",
            "url": "https://github.com/ForbesLindesay"
        },
        {
            "name": "Fabrizio Moscon",
            "url": "https://github.com/fabriziomoscon"
        },
        {
            "name": "Marc-Olivier Ricard",
            "url": "https://github.com/ricardmo"
        },
        {
            "name": "Gleb Bahmutov",
            "url": "https://github.com/bahmutov"
        },
        {
            "name": "Steve Kinney",
            "url": "https://github.com/stevekinney"
        },
        {
            "name": "Gal Niv",
            "url": "https://github.com/galniv"
        },
        {
            "name": "Rodrigo González",
            "url": "https://github.com/roro89"
        },
        {
            "name": "Alejandro Villanueva",
            "url": "https://github.com/ialex"
        },
        {
            "name": "Clinton Skakun",
            "url": "https://github.com/clintonskakun"
        },
        {
            "name": "Paul Jolly",
            "url": "https://github.com/myitcv"
        },
        {
            "name": "Ryan Temple",
            "url": "https://github.com/ryantemple"
        },
        {
            "name": "Mark Herhold",
            "url": "https://github.com/MarkHerhold"
        },
        {
            "name": "Victor Bakke",
            "url": "https://github.com/Gipphe"
        }
    ],
    "dependencies": {},
    "description": "A little library for asserting types and values.",
    "devDependencies": {
        "chai": "3.5.x",
        "jshint": "2.9.x",
        "mocha": "3.2.x",
        "uglify-js": "2.7.x"
    },
    "directories": {},
    "dist": {
        "shasum": "a1d6b9d2fa3e7e80e3a2d373ffcc2cf10b7370c9",
        "tarball": "https://registry.npmjs.org/check-types/-/check-types-7.1.5.tgz"
    },
    "files": [
        "COPYING",
        "HISTORY.md",
        "src"
    ],
    "gitHead": "4744088cd6e7007d6d1020b9ed7658bf0b97e34d",
    "homepage": "https://github.com/philbooth/check-types.js",
    "keywords": [
        "type",
        "types",
        "type-check",
        "type-checking",
        "duck-typing",
        "arguments",
        "parameters",
        "values",
        "data",
        "contract",
        "assert",
        "check",
        "verify",
        "safe",
        "safety"
    ],
    "license": "MIT",
    "main": "./src/check-types",
    "maintainers": [
        {
            "name": "philbooth"
        }
    ],
    "name": "check-types",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/philbooth/check-types.js.git"
    },
    "scripts": {
        "lint": "jshint ./src/check-types.js",
        "minify": "uglifyjs ./src/check-types.js --compress --mangle --output ./src/check-types.min.js",
        "test": "mocha --ui tdd --reporter spec --colors ./test/check-types.js"
    },
    "version": "7.1.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
