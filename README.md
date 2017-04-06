# api documentation for  [check-types (v7.1.5)](https://github.com/philbooth/check-types.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-check-types.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-check-types) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-check-types.svg)](https://travis-ci.org/npmdoc/node-npmdoc-check-types)
#### A little library for asserting types and values.

[![NPM](https://nodei.co/npm/check-types.png?downloads=true)](https://www.npmjs.com/package/check-types)

[![apidoc](https://npmdoc.github.io/node-npmdoc-check-types/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-check-types_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-check-types/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-check-types/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-check-types/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Phil Booth",
        "email": "pmbooth@gmail.com",
        "url": "https://github.com/philbooth"
    },
    "bugs": {
        "url": "https://github.com/philbooth/check-types.js/issues"
    },
    "contributors": [
        {
            "name": "Phil Booth",
            "email": "pmbooth@gmail.com",
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
            "name": "philbooth",
            "email": "pmbooth@gmail.com"
        }
    ],
    "name": "check-types",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module check-types](#apidoc.module.check-types)
1.  [function <span class="apidocSignatureSpan">check-types.</span>all (data)](#apidoc.element.check-types.all)
1.  [function <span class="apidocSignatureSpan">check-types.</span>any (data)](#apidoc.element.check-types.any)
1.  [function <span class="apidocSignatureSpan">check-types.</span>apply (data, predicates)](#apidoc.element.check-types.apply)
1.  [function <span class="apidocSignatureSpan">check-types.</span>array (data)](#apidoc.element.check-types.array)
1.  [function <span class="apidocSignatureSpan">check-types.</span>arrayLike (data)](#apidoc.element.check-types.arrayLike)
1.  [function <span class="apidocSignatureSpan">check-types.</span>assert (value, message, ErrorType)](#apidoc.element.check-types.assert)
1.  [function <span class="apidocSignatureSpan">check-types.</span>assigned (data)](#apidoc.element.check-types.assigned)
1.  [function <span class="apidocSignatureSpan">check-types.</span>between (data, x, y)](#apidoc.element.check-types.between)
1.  [function <span class="apidocSignatureSpan">check-types.</span>boolean (data)](#apidoc.element.check-types.boolean)
1.  [function <span class="apidocSignatureSpan">check-types.</span>contains (data, substring)](#apidoc.element.check-types.contains)
1.  [function <span class="apidocSignatureSpan">check-types.</span>date (data)](#apidoc.element.check-types.date)
1.  [function <span class="apidocSignatureSpan">check-types.</span>emptyArray (data)](#apidoc.element.check-types.emptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.</span>emptyObject (data)](#apidoc.element.check-types.emptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.</span>emptyString (data)](#apidoc.element.check-types.emptyString)
1.  [function <span class="apidocSignatureSpan">check-types.</span>equal (lhs, rhs)](#apidoc.element.check-types.equal)
1.  [function <span class="apidocSignatureSpan">check-types.</span>even (data)](#apidoc.element.check-types.even)
1.  [function <span class="apidocSignatureSpan">check-types.</span>function (data)](#apidoc.element.check-types.function)
1.  [function <span class="apidocSignatureSpan">check-types.</span>greater (lhs, rhs)](#apidoc.element.check-types.greater)
1.  [function <span class="apidocSignatureSpan">check-types.</span>greaterOrEqual (lhs, rhs)](#apidoc.element.check-types.greaterOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.</span>hasLength (data, length)](#apidoc.element.check-types.hasLength)
1.  [function <span class="apidocSignatureSpan">check-types.</span>inRange (data, x, y)](#apidoc.element.check-types.inRange)
1.  [function <span class="apidocSignatureSpan">check-types.</span>includes (data, value)](#apidoc.element.check-types.includes)
1.  [function <span class="apidocSignatureSpan">check-types.</span>infinity (data)](#apidoc.element.check-types.infinity)
1.  [function <span class="apidocSignatureSpan">check-types.</span>instance (data, prototype)](#apidoc.element.check-types.instance)
1.  [function <span class="apidocSignatureSpan">check-types.</span>instanceStrict (data, prototype)](#apidoc.element.check-types.instanceStrict)
1.  [function <span class="apidocSignatureSpan">check-types.</span>integer (data)](#apidoc.element.check-types.integer)
1.  [function <span class="apidocSignatureSpan">check-types.</span>iterable (data)](#apidoc.element.check-types.iterable)
1.  [function <span class="apidocSignatureSpan">check-types.</span>less (lhs, rhs)](#apidoc.element.check-types.less)
1.  [function <span class="apidocSignatureSpan">check-types.</span>lessOrEqual (lhs, rhs)](#apidoc.element.check-types.lessOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.</span>like (data, archetype)](#apidoc.element.check-types.like)
1.  [function <span class="apidocSignatureSpan">check-types.</span>map (data, predicates)](#apidoc.element.check-types.map)
1.  [function <span class="apidocSignatureSpan">check-types.</span>match (data, regex)](#apidoc.element.check-types.match)
1.  [function <span class="apidocSignatureSpan">check-types.</span>maybe (value)](#apidoc.element.check-types.maybe)
1.  [function <span class="apidocSignatureSpan">check-types.</span>negative (data)](#apidoc.element.check-types.negative)
1.  [function <span class="apidocSignatureSpan">check-types.</span>nonEmptyArray (data)](#apidoc.element.check-types.nonEmptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.</span>nonEmptyObject (data)](#apidoc.element.check-types.nonEmptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.</span>nonEmptyString (data)](#apidoc.element.check-types.nonEmptyString)
1.  [function <span class="apidocSignatureSpan">check-types.</span>not (value)](#apidoc.element.check-types.not)
1.  [function <span class="apidocSignatureSpan">check-types.</span>null (data)](#apidoc.element.check-types.null)
1.  [function <span class="apidocSignatureSpan">check-types.</span>number (data)](#apidoc.element.check-types.number)
1.  [function <span class="apidocSignatureSpan">check-types.</span>object (data)](#apidoc.element.check-types.object)
1.  [function <span class="apidocSignatureSpan">check-types.</span>odd (data)](#apidoc.element.check-types.odd)
1.  [function <span class="apidocSignatureSpan">check-types.</span>positive (data)](#apidoc.element.check-types.positive)
1.  [function <span class="apidocSignatureSpan">check-types.</span>string (data)](#apidoc.element.check-types.string)
1.  [function <span class="apidocSignatureSpan">check-types.</span>undefined (data)](#apidoc.element.check-types.undefined)
1.  [function <span class="apidocSignatureSpan">check-types.</span>zero (data)](#apidoc.element.check-types.zero)
1.  object <span class="apidocSignatureSpan">check-types.</span>assert.maybe
1.  object <span class="apidocSignatureSpan">check-types.</span>assert.not

#### [module check-types.assert](#apidoc.module.check-types.assert)
1.  [function <span class="apidocSignatureSpan">check-types.</span>assert (value, message, ErrorType)](#apidoc.element.check-types.assert.assert)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>array ()](#apidoc.element.check-types.assert.array)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>arrayLike ()](#apidoc.element.check-types.assert.arrayLike)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>assigned ()](#apidoc.element.check-types.assert.assigned)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>between ()](#apidoc.element.check-types.assert.between)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>boolean ()](#apidoc.element.check-types.assert.boolean)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>contains ()](#apidoc.element.check-types.assert.contains)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>date ()](#apidoc.element.check-types.assert.date)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>emptyArray ()](#apidoc.element.check-types.assert.emptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>emptyObject ()](#apidoc.element.check-types.assert.emptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>emptyString ()](#apidoc.element.check-types.assert.emptyString)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>equal ()](#apidoc.element.check-types.assert.equal)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>even ()](#apidoc.element.check-types.assert.even)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>function ()](#apidoc.element.check-types.assert.function)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>greater ()](#apidoc.element.check-types.assert.greater)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>greaterOrEqual ()](#apidoc.element.check-types.assert.greaterOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>hasLength ()](#apidoc.element.check-types.assert.hasLength)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>inRange ()](#apidoc.element.check-types.assert.inRange)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>includes ()](#apidoc.element.check-types.assert.includes)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>infinity ()](#apidoc.element.check-types.assert.infinity)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>instance ()](#apidoc.element.check-types.assert.instance)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>instanceStrict ()](#apidoc.element.check-types.assert.instanceStrict)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>integer ()](#apidoc.element.check-types.assert.integer)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>iterable ()](#apidoc.element.check-types.assert.iterable)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>less ()](#apidoc.element.check-types.assert.less)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>lessOrEqual ()](#apidoc.element.check-types.assert.lessOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>like ()](#apidoc.element.check-types.assert.like)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>match ()](#apidoc.element.check-types.assert.match)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>negative ()](#apidoc.element.check-types.assert.negative)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>nonEmptyArray ()](#apidoc.element.check-types.assert.nonEmptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>nonEmptyObject ()](#apidoc.element.check-types.assert.nonEmptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>nonEmptyString ()](#apidoc.element.check-types.assert.nonEmptyString)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>null ()](#apidoc.element.check-types.assert.null)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>number ()](#apidoc.element.check-types.assert.number)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>object ()](#apidoc.element.check-types.assert.object)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>odd ()](#apidoc.element.check-types.assert.odd)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>positive ()](#apidoc.element.check-types.assert.positive)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>string ()](#apidoc.element.check-types.assert.string)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>undefined ()](#apidoc.element.check-types.assert.undefined)
1.  [function <span class="apidocSignatureSpan">check-types.assert.</span>zero ()](#apidoc.element.check-types.assert.zero)
1.  object <span class="apidocSignatureSpan">check-types.assert.</span>maybe
1.  object <span class="apidocSignatureSpan">check-types.assert.</span>not

#### [module check-types.assert.maybe](#apidoc.module.check-types.assert.maybe)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>array ()](#apidoc.element.check-types.assert.maybe.array)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>arrayLike ()](#apidoc.element.check-types.assert.maybe.arrayLike)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>assigned ()](#apidoc.element.check-types.assert.maybe.assigned)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>between ()](#apidoc.element.check-types.assert.maybe.between)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>boolean ()](#apidoc.element.check-types.assert.maybe.boolean)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>contains ()](#apidoc.element.check-types.assert.maybe.contains)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>date ()](#apidoc.element.check-types.assert.maybe.date)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>emptyArray ()](#apidoc.element.check-types.assert.maybe.emptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>emptyObject ()](#apidoc.element.check-types.assert.maybe.emptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>emptyString ()](#apidoc.element.check-types.assert.maybe.emptyString)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>equal ()](#apidoc.element.check-types.assert.maybe.equal)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>even ()](#apidoc.element.check-types.assert.maybe.even)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>function ()](#apidoc.element.check-types.assert.maybe.function)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>greater ()](#apidoc.element.check-types.assert.maybe.greater)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>greaterOrEqual ()](#apidoc.element.check-types.assert.maybe.greaterOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>hasLength ()](#apidoc.element.check-types.assert.maybe.hasLength)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>inRange ()](#apidoc.element.check-types.assert.maybe.inRange)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>includes ()](#apidoc.element.check-types.assert.maybe.includes)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>infinity ()](#apidoc.element.check-types.assert.maybe.infinity)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>instance ()](#apidoc.element.check-types.assert.maybe.instance)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>instanceStrict ()](#apidoc.element.check-types.assert.maybe.instanceStrict)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>integer ()](#apidoc.element.check-types.assert.maybe.integer)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>iterable ()](#apidoc.element.check-types.assert.maybe.iterable)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>less ()](#apidoc.element.check-types.assert.maybe.less)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>lessOrEqual ()](#apidoc.element.check-types.assert.maybe.lessOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>like ()](#apidoc.element.check-types.assert.maybe.like)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>match ()](#apidoc.element.check-types.assert.maybe.match)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>negative ()](#apidoc.element.check-types.assert.maybe.negative)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>nonEmptyArray ()](#apidoc.element.check-types.assert.maybe.nonEmptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>nonEmptyObject ()](#apidoc.element.check-types.assert.maybe.nonEmptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>nonEmptyString ()](#apidoc.element.check-types.assert.maybe.nonEmptyString)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>null ()](#apidoc.element.check-types.assert.maybe.null)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>number ()](#apidoc.element.check-types.assert.maybe.number)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>object ()](#apidoc.element.check-types.assert.maybe.object)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>odd ()](#apidoc.element.check-types.assert.maybe.odd)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>positive ()](#apidoc.element.check-types.assert.maybe.positive)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>string ()](#apidoc.element.check-types.assert.maybe.string)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>undefined ()](#apidoc.element.check-types.assert.maybe.undefined)
1.  [function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>zero ()](#apidoc.element.check-types.assert.maybe.zero)

#### [module check-types.assert.not](#apidoc.module.check-types.assert.not)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>array ()](#apidoc.element.check-types.assert.not.array)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>arrayLike ()](#apidoc.element.check-types.assert.not.arrayLike)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>assigned ()](#apidoc.element.check-types.assert.not.assigned)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>between ()](#apidoc.element.check-types.assert.not.between)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>boolean ()](#apidoc.element.check-types.assert.not.boolean)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>contains ()](#apidoc.element.check-types.assert.not.contains)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>date ()](#apidoc.element.check-types.assert.not.date)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>emptyArray ()](#apidoc.element.check-types.assert.not.emptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>emptyObject ()](#apidoc.element.check-types.assert.not.emptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>emptyString ()](#apidoc.element.check-types.assert.not.emptyString)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>equal ()](#apidoc.element.check-types.assert.not.equal)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>even ()](#apidoc.element.check-types.assert.not.even)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>function ()](#apidoc.element.check-types.assert.not.function)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>greater ()](#apidoc.element.check-types.assert.not.greater)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>greaterOrEqual ()](#apidoc.element.check-types.assert.not.greaterOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>hasLength ()](#apidoc.element.check-types.assert.not.hasLength)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>inRange ()](#apidoc.element.check-types.assert.not.inRange)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>includes ()](#apidoc.element.check-types.assert.not.includes)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>infinity ()](#apidoc.element.check-types.assert.not.infinity)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>instance ()](#apidoc.element.check-types.assert.not.instance)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>instanceStrict ()](#apidoc.element.check-types.assert.not.instanceStrict)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>integer ()](#apidoc.element.check-types.assert.not.integer)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>iterable ()](#apidoc.element.check-types.assert.not.iterable)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>less ()](#apidoc.element.check-types.assert.not.less)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>lessOrEqual ()](#apidoc.element.check-types.assert.not.lessOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>like ()](#apidoc.element.check-types.assert.not.like)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>match ()](#apidoc.element.check-types.assert.not.match)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>negative ()](#apidoc.element.check-types.assert.not.negative)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>nonEmptyArray ()](#apidoc.element.check-types.assert.not.nonEmptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>nonEmptyObject ()](#apidoc.element.check-types.assert.not.nonEmptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>nonEmptyString ()](#apidoc.element.check-types.assert.not.nonEmptyString)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>null ()](#apidoc.element.check-types.assert.not.null)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>number ()](#apidoc.element.check-types.assert.not.number)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>object ()](#apidoc.element.check-types.assert.not.object)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>odd ()](#apidoc.element.check-types.assert.not.odd)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>positive ()](#apidoc.element.check-types.assert.not.positive)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>string ()](#apidoc.element.check-types.assert.not.string)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>undefined ()](#apidoc.element.check-types.assert.not.undefined)
1.  [function <span class="apidocSignatureSpan">check-types.assert.not.</span>zero ()](#apidoc.element.check-types.assert.not.zero)

#### [module check-types.maybe](#apidoc.module.check-types.maybe)
1.  [function <span class="apidocSignatureSpan">check-types.</span>maybe (value)](#apidoc.element.check-types.maybe.maybe)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>array ()](#apidoc.element.check-types.maybe.array)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>arrayLike ()](#apidoc.element.check-types.maybe.arrayLike)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>assigned ()](#apidoc.element.check-types.maybe.assigned)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>between ()](#apidoc.element.check-types.maybe.between)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>boolean ()](#apidoc.element.check-types.maybe.boolean)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>contains ()](#apidoc.element.check-types.maybe.contains)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>date ()](#apidoc.element.check-types.maybe.date)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>emptyArray ()](#apidoc.element.check-types.maybe.emptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>emptyObject ()](#apidoc.element.check-types.maybe.emptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>emptyString ()](#apidoc.element.check-types.maybe.emptyString)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>equal ()](#apidoc.element.check-types.maybe.equal)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>even ()](#apidoc.element.check-types.maybe.even)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>function ()](#apidoc.element.check-types.maybe.function)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>greater ()](#apidoc.element.check-types.maybe.greater)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>greaterOrEqual ()](#apidoc.element.check-types.maybe.greaterOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>hasLength ()](#apidoc.element.check-types.maybe.hasLength)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>inRange ()](#apidoc.element.check-types.maybe.inRange)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>includes ()](#apidoc.element.check-types.maybe.includes)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>infinity ()](#apidoc.element.check-types.maybe.infinity)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>instance ()](#apidoc.element.check-types.maybe.instance)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>instanceStrict ()](#apidoc.element.check-types.maybe.instanceStrict)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>integer ()](#apidoc.element.check-types.maybe.integer)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>iterable ()](#apidoc.element.check-types.maybe.iterable)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>less ()](#apidoc.element.check-types.maybe.less)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>lessOrEqual ()](#apidoc.element.check-types.maybe.lessOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>like ()](#apidoc.element.check-types.maybe.like)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>match ()](#apidoc.element.check-types.maybe.match)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>negative ()](#apidoc.element.check-types.maybe.negative)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>nonEmptyArray ()](#apidoc.element.check-types.maybe.nonEmptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>nonEmptyObject ()](#apidoc.element.check-types.maybe.nonEmptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>nonEmptyString ()](#apidoc.element.check-types.maybe.nonEmptyString)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>null ()](#apidoc.element.check-types.maybe.null)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>number ()](#apidoc.element.check-types.maybe.number)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>object ()](#apidoc.element.check-types.maybe.object)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>odd ()](#apidoc.element.check-types.maybe.odd)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>positive ()](#apidoc.element.check-types.maybe.positive)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>string ()](#apidoc.element.check-types.maybe.string)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>undefined ()](#apidoc.element.check-types.maybe.undefined)
1.  [function <span class="apidocSignatureSpan">check-types.maybe.</span>zero ()](#apidoc.element.check-types.maybe.zero)

#### [module check-types.not](#apidoc.module.check-types.not)
1.  [function <span class="apidocSignatureSpan">check-types.</span>not (value)](#apidoc.element.check-types.not.not)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>array ()](#apidoc.element.check-types.not.array)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>arrayLike ()](#apidoc.element.check-types.not.arrayLike)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>assigned ()](#apidoc.element.check-types.not.assigned)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>between ()](#apidoc.element.check-types.not.between)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>boolean ()](#apidoc.element.check-types.not.boolean)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>contains ()](#apidoc.element.check-types.not.contains)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>date ()](#apidoc.element.check-types.not.date)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>emptyArray ()](#apidoc.element.check-types.not.emptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>emptyObject ()](#apidoc.element.check-types.not.emptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>emptyString ()](#apidoc.element.check-types.not.emptyString)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>equal ()](#apidoc.element.check-types.not.equal)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>even ()](#apidoc.element.check-types.not.even)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>function ()](#apidoc.element.check-types.not.function)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>greater ()](#apidoc.element.check-types.not.greater)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>greaterOrEqual ()](#apidoc.element.check-types.not.greaterOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>hasLength ()](#apidoc.element.check-types.not.hasLength)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>inRange ()](#apidoc.element.check-types.not.inRange)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>includes ()](#apidoc.element.check-types.not.includes)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>infinity ()](#apidoc.element.check-types.not.infinity)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>instance ()](#apidoc.element.check-types.not.instance)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>instanceStrict ()](#apidoc.element.check-types.not.instanceStrict)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>integer ()](#apidoc.element.check-types.not.integer)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>iterable ()](#apidoc.element.check-types.not.iterable)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>less ()](#apidoc.element.check-types.not.less)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>lessOrEqual ()](#apidoc.element.check-types.not.lessOrEqual)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>like ()](#apidoc.element.check-types.not.like)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>match ()](#apidoc.element.check-types.not.match)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>negative ()](#apidoc.element.check-types.not.negative)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>nonEmptyArray ()](#apidoc.element.check-types.not.nonEmptyArray)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>nonEmptyObject ()](#apidoc.element.check-types.not.nonEmptyObject)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>nonEmptyString ()](#apidoc.element.check-types.not.nonEmptyString)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>null ()](#apidoc.element.check-types.not.null)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>number ()](#apidoc.element.check-types.not.number)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>object ()](#apidoc.element.check-types.not.object)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>odd ()](#apidoc.element.check-types.not.odd)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>positive ()](#apidoc.element.check-types.not.positive)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>string ()](#apidoc.element.check-types.not.string)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>undefined ()](#apidoc.element.check-types.not.undefined)
1.  [function <span class="apidocSignatureSpan">check-types.not.</span>zero ()](#apidoc.element.check-types.not.zero)



# <a name="apidoc.module.check-types"></a>[module check-types](#apidoc.module.check-types)

#### <a name="apidoc.element.check-types.all"></a>[function <span class="apidocSignatureSpan">check-types.</span>all (data)](#apidoc.element.check-types.all)
- description and source-code
```javascript
function all(data) {
  if (array(data)) {
    return testArray(data, false);
  }

  assert.object(data);

  return testObject(data, false);
}
```
- example usage
```shell
...
Supports nested objects.
Passing a single predicate
instead of an object
applies all of the values
to the same predicate,
ignoring nested objects.

* 'check.all(results)':
Returns 'true'
if all the result values are true
in an array (returned from 'apply')
or object (returned from 'map').

* 'check.any(predicateResults)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.any"></a>[function <span class="apidocSignatureSpan">check-types.</span>any (data)](#apidoc.element.check-types.any)
- description and source-code
```javascript
function any(data) {
  if (array(data)) {
    return testArray(data, true);
  }

  assert.object(data);

  return testObject(data, true);
}
```
- example usage
```shell
...

* 'check.all(results)':
  Returns 'true'
  if all the result values are true
  in an array (returned from 'apply')
  or object (returned from 'map').

* 'check.any(predicateResults)':
  Returns 'true'
  if any result value is true
  in an array (returned from 'apply')
  or object (returned from 'map').

#### Some examples
...
```

#### <a name="apidoc.element.check-types.apply"></a>[function <span class="apidocSignatureSpan">check-types.</span>apply (data, predicates)](#apidoc.element.check-types.apply)
- description and source-code
```javascript
function apply(data, predicates) {
  assert.array(data);

  if (isFunction(predicates)) {
    return data.map(function (value) {
      return predicates(value);
    });
  }

  assert.array(predicates);
  assert.hasLength(data, predicates.length);

  return data.map(function (value, index) {
    return predicates[index](value);
  });
}
```
- example usage
```shell
...
that control
the message and type
of the thrown error object.
Also works with the 'not', 'maybe' and '...of' modifiers.

#### Batch operations

* 'check.apply(things, predicates)':
Applies each value from the 'things' array
to the corresponding predicate
and returns the array of results.
Passing a single predicate
instead of an array
applies all of the values
to the same predicate.
...
```

#### <a name="apidoc.element.check-types.array"></a>[function <span class="apidocSignatureSpan">check-types.</span>array (data)](#apidoc.element.check-types.array)
- description and source-code
```javascript
function array(data) {
  return Array.isArray(data);
}
```
- example usage
```shell
...
Duck-typing checker.
Returns 'true'
if 'thing' has all of the properties of 'duck',
'false' otherwise.

#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
...
```

#### <a name="apidoc.element.check-types.arrayLike"></a>[function <span class="apidocSignatureSpan">check-types.</span>arrayLike (data)](#apidoc.element.check-types.arrayLike)
- description and source-code
```javascript
function arrayLike(data) {
  return assigned(data) && number(data.length);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
...
```

#### <a name="apidoc.element.check-types.assert"></a>[function <span class="apidocSignatureSpan">check-types.</span>assert (value, message, ErrorType)](#apidoc.element.check-types.assert)
- description and source-code
```javascript
function assertImpl(value, message, ErrorType) {
  if (value === false) {
    throw new (ErrorType || Error)(message || 'Assertion failed');
  }
}
```
- example usage
```shell
...
except it operates on iterables.

* 'check.object.of.xxx(thing)':
The 'object.of' modifier
is synonymous with 'array.of',
except it operates on an object's properties.

* 'check.assert(value, message, ErrorType)':
Throws a 'TypeError'
if 'value' is 'false'.
'message' and 'ErrorType'
are optional arguments
that control
the message and type
of the thrown error object.
...
```

#### <a name="apidoc.element.check-types.assigned"></a>[function <span class="apidocSignatureSpan">check-types.</span>assigned (data)](#apidoc.element.check-types.assigned)
- description and source-code
```javascript
function assigned(data) {
  return ! isUndefined(data) && ! isNull(data);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
'null' or 'undefined',
'false' otherwise.

* 'check.hasLength(thing, value)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.between"></a>[function <span class="apidocSignatureSpan">check-types.</span>between (data, x, y)](#apidoc.element.check-types.between)
- description and source-code
```javascript
function between(data, x, y) {
  if (x < y) {
    return greater(data, x) && less(data, y);
  }

  return less(data, x) && greater(data, y);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.boolean"></a>[function <span class="apidocSignatureSpan">check-types.</span>boolean (data)](#apidoc.element.check-types.boolean)
- description and source-code
```javascript
function boolean(data) {
  return data === false || data === true;
}
```
- example usage
```shell
...
* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
  Returns 'true'
  if 'thing' is a boolean,
  'false' otherwise.

#### Object predicates

* 'check.object(thing)':
...
```

#### <a name="apidoc.element.check-types.contains"></a>[function <span class="apidocSignatureSpan">check-types.</span>contains (data, substring)](#apidoc.element.check-types.contains)
- description and source-code
```javascript
function contains(data, substring) {
  return string(data) && data.indexOf(substring) !== -1;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
that contains 'substring',
'false' otherwise.

* 'check.match(thing, regex)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.date"></a>[function <span class="apidocSignatureSpan">check-types.</span>date (data)](#apidoc.element.check-types.date)
- description and source-code
```javascript
function date(data) {
  try {
    return instance(data, Date) && integer(data.getTime());
  } catch (error) {
    return false;
  }
}
```
- example usage
```shell
...
* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
...
```

#### <a name="apidoc.element.check-types.emptyArray"></a>[function <span class="apidocSignatureSpan">check-types.</span>emptyArray (data)](#apidoc.element.check-types.emptyArray)
- description and source-code
```javascript
function emptyArray(data) {
  return array(data) && data.length === 0;
}
```
- example usage
```shell
...
#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
...
```

#### <a name="apidoc.element.check-types.emptyObject"></a>[function <span class="apidocSignatureSpan">check-types.</span>emptyObject (data)](#apidoc.element.check-types.emptyObject)
- description and source-code
```javascript
function emptyObject(data) {
  return object(data) && Object.keys(data).length === 0;
}
```
- example usage
```shell
...
#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
...
```

#### <a name="apidoc.element.check-types.emptyString"></a>[function <span class="apidocSignatureSpan">check-types.</span>emptyString (data)](#apidoc.element.check-types.emptyString)
- description and source-code
```javascript
function emptyString(data) {
  return data === '';
}
```
- example usage
```shell
...
#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
...
```

#### <a name="apidoc.element.check-types.equal"></a>[function <span class="apidocSignatureSpan">check-types.</span>equal (lhs, rhs)](#apidoc.element.check-types.equal)
- description and source-code
```javascript
function equal(lhs, rhs) {
  return lhs === rhs;
}
```
- example usage
```shell
...
'check.apply',
'check.map',
'check.any' and
'check.all'.

#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
...
```

#### <a name="apidoc.element.check-types.even"></a>[function <span class="apidocSignatureSpan">check-types.</span>even (data)](#apidoc.element.check-types.even)
- description and source-code
```javascript
function even(data) {
  return number(data) && data % 2 === 0;
}
```
- example usage
```shell
...
  'false' otherwise.

* 'check.odd(thing)':
  Returns 'true'
  if 'thing' is an odd number,
  'false' otherwise.

* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
...
```

#### <a name="apidoc.element.check-types.function"></a>[function <span class="apidocSignatureSpan">check-types.</span>function (data)](#apidoc.element.check-types.function)
- description and source-code
```javascript
function isFunction(data) {
  return typeof data === 'function';
}
```
- example usage
```shell
...
* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
  Returns 'true'
  if 'thing' is a function,
  'false' otherwise.

#### Modifiers

* 'check.not(value)':
...
```

#### <a name="apidoc.element.check-types.greater"></a>[function <span class="apidocSignatureSpan">check-types.</span>greater (lhs, rhs)](#apidoc.element.check-types.greater)
- description and source-code
```javascript
function greater(lhs, rhs) {
  return number(lhs) && lhs > rhs;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.greaterOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.</span>greaterOrEqual (lhs, rhs)](#apidoc.element.check-types.greaterOrEqual)
- description and source-code
```javascript
function greaterOrEqual(lhs, rhs) {
  return number(lhs) && lhs >= rhs;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
...
```

#### <a name="apidoc.element.check-types.hasLength"></a>[function <span class="apidocSignatureSpan">check-types.</span>hasLength (data, length)](#apidoc.element.check-types.hasLength)
- description and source-code
```javascript
function hasLength(data, length) {
  return assigned(data) && data.length === length;
}
```
- example usage
```shell
...

* 'check.assigned(thing)':
  Returns 'true'
  if 'thing' is not
  'null' or 'undefined',
  'false' otherwise.

* 'check.hasLength(thing, value)':
  Returns 'true'
  if 'thing' has a length property
  that equals 'value',
  'false' otherwise.

#### String predicates
...
```

#### <a name="apidoc.element.check-types.inRange"></a>[function <span class="apidocSignatureSpan">check-types.</span>inRange (data, x, y)](#apidoc.element.check-types.inRange)
- description and source-code
```javascript
function inRange(data, x, y) {
  if (x < y) {
    return greaterOrEqual(data, x) && lessOrEqual(data, y);
  }

  return lessOrEqual(data, x) && greaterOrEqual(data, y);
}
```
- example usage
```shell
...
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.inRange(thing, a, b)':
Returns 'true' if 'thing' is a number
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.includes"></a>[function <span class="apidocSignatureSpan">check-types.</span>includes (data, value)](#apidoc.element.check-types.includes)
- description and source-code
```javascript
function includes(data, value) {
  var iterator, iteration;

  if (not.assigned(data)) {
    return false;
  }

  try {
    if (typeof Symbol !== 'undefined' && data[Symbol.iterator] && isFunction(data.values)) {
      iterator = data.values();

      do {
        iteration = iterator.next();

        if (iteration.value === value) {
          return true;
        }
      } while (! iteration.done);

      return false;
    }

    Object.keys(data).forEach(function (key) {
      if (data[key] === value) {
        throw 0;
      }
    });
  } catch (ignore) {
    return true;
  }

  return false;
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' implements the iterable protocol,
  'false' otherwise.
  In pre-ES6 environments,
  this predicate falls back
  to 'arrayLike' behaviour.

* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
...
```

#### <a name="apidoc.element.check-types.infinity"></a>[function <span class="apidocSignatureSpan">check-types.</span>infinity (data)](#apidoc.element.check-types.infinity)
- description and source-code
```javascript
function infinity(data) {
  return data === Number.POSITIVE_INFINITY || data === Number.NEGATIVE_INFINITY;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
...
```

#### <a name="apidoc.element.check-types.instance"></a>[function <span class="apidocSignatureSpan">check-types.</span>instance (data, prototype)](#apidoc.element.check-types.instance)
- description and source-code
```javascript
function instance(data, prototype) {
  try {
    return instanceStrict(data, prototype) ||
      data.constructor.name === prototype.name ||
      Object.prototype.toString.call(data) === '[object ' + prototype.name + ']';
  } catch (error) {
    return false;
  }
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.
Falls back to testing
'constructor.name' and 'Object.prototype.toString'
if the 'instanceof' test fails.
...
```

#### <a name="apidoc.element.check-types.instanceStrict"></a>[function <span class="apidocSignatureSpan">check-types.</span>instanceStrict (data, prototype)](#apidoc.element.check-types.instanceStrict)
- description and source-code
```javascript
function instanceStrict(data, prototype) {
  try {
    return data instanceof prototype;
  } catch (error) {
    return false;
  }
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.integer"></a>[function <span class="apidocSignatureSpan">check-types.</span>integer (data)](#apidoc.element.check-types.integer)
- description and source-code
```javascript
function integer(data) {
  return number(data) && data % 1 === 0;
}
```
- example usage
```shell
...
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
...
```

#### <a name="apidoc.element.check-types.iterable"></a>[function <span class="apidocSignatureSpan">check-types.</span>iterable (data)](#apidoc.element.check-types.iterable)
- description and source-code
```javascript
function iterable(data) {
  if (typeof Symbol === 'undefined') {
    // Fall back to 'arrayLike' predicate in pre-ES6 environments.
    return arrayLike(data);
  }

  return assigned(data) && isFunction(data[Symbol.iterator]);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
'false' otherwise.
In pre-ES6 environments,
this predicate falls back
to 'arrayLike' behaviour.
...
```

#### <a name="apidoc.element.check-types.less"></a>[function <span class="apidocSignatureSpan">check-types.</span>less (lhs, rhs)](#apidoc.element.check-types.less)
- description and source-code
```javascript
function less(lhs, rhs) {
  return number(lhs) && lhs < rhs;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.lessOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.</span>lessOrEqual (lhs, rhs)](#apidoc.element.check-types.lessOrEqual)
- description and source-code
```javascript
function lessOrEqual(lhs, rhs) {
  return number(lhs) && lhs <= rhs;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
...
```

#### <a name="apidoc.element.check-types.like"></a>[function <span class="apidocSignatureSpan">check-types.</span>like (data, archetype)](#apidoc.element.check-types.like)
- description and source-code
```javascript
function like(data, archetype) {
  var name;

  for (name in archetype) {
    if (archetype.hasOwnProperty(name)) {
      if (data.hasOwnProperty(name) === false || typeof data[name] !== typeof archetype[name]) {
        return false;
      }

      if (object(data[name]) && like(data[name], archetype[name]) === false) {
        return false;
      }
    }
  }

  return true;
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' is an instance of 'prototype',
  'false' otherwise.
  Falls back to testing
  'constructor.name' and 'Object.prototype.toString'
  if the 'instanceof' test fails.

* 'check.like(thing, duck)':
  Duck-typing checker.
  Returns 'true'
  if 'thing' has all of the properties of 'duck',
  'false' otherwise.

#### Array predicates
...
```

#### <a name="apidoc.element.check-types.map"></a>[function <span class="apidocSignatureSpan">check-types.</span>map (data, predicates)](#apidoc.element.check-types.map)
- description and source-code
```javascript
function map(data, predicates) {
  assert.object(data);

  if (isFunction(predicates)) {
    return mapSimple(data, predicates);
  }

  assert.object(predicates);

  return mapComplex(data, predicates);
}
```
- example usage
```shell
...
to the corresponding predicate
and returns the array of results.
Passing a single predicate
instead of an array
applies all of the values
to the same predicate.

* 'check.map(things, predicates)':
Maps each value from the 'things' object
to the corresponding predicate
and returns an object
containing the results.
Supports nested objects.
Passing a single predicate
instead of an object
...
```

#### <a name="apidoc.element.check-types.match"></a>[function <span class="apidocSignatureSpan">check-types.</span>match (data, regex)](#apidoc.element.check-types.match)
- description and source-code
```javascript
function match(data, regex) {
  return string(data) && !! data.match(regex);
}
```
- example usage
```shell
...

* 'check.contains(thing, substring)':
  Returns 'true'
  if 'thing' is a string
  that contains 'substring',
  'false' otherwise.

* 'check.match(thing, regex)':
  Returns 'true'
  if 'thing' is a string
  that matches 'regex',
  'false' otherwise.

#### Number predicates
...
```

#### <a name="apidoc.element.check-types.maybe"></a>[function <span class="apidocSignatureSpan">check-types.</span>maybe (value)](#apidoc.element.check-types.maybe)
- description and source-code
```javascript
function maybeImpl(value) {
  if (assigned(value) === false) {
    return true;
  }

  return value;
}
```
- example usage
```shell
...
Returns the negation
of 'value'.

* 'check.not.xxx(...)':
Returns the negation
of the predicate.

* 'check.maybe(value)':
Returns 'true'
if 'value' is 'null' or 'undefined',
otherwise it returns 'value'.

* 'check.maybe.xxx(...)':
Returns 'true'
if 'thing' is 'null' or 'undefined',
...
```

#### <a name="apidoc.element.check-types.negative"></a>[function <span class="apidocSignatureSpan">check-types.</span>negative (data)](#apidoc.element.check-types.negative)
- description and source-code
```javascript
function negative(data) {
  return less(data, 0);
}
```
- example usage
```shell
...
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.nonEmptyArray"></a>[function <span class="apidocSignatureSpan">check-types.</span>nonEmptyArray (data)](#apidoc.element.check-types.nonEmptyArray)
- description and source-code
```javascript
function nonEmptyArray(data) {
  return array(data) && data.length > 0;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
...
```

#### <a name="apidoc.element.check-types.nonEmptyObject"></a>[function <span class="apidocSignatureSpan">check-types.</span>nonEmptyObject (data)](#apidoc.element.check-types.nonEmptyObject)
- description and source-code
```javascript
function nonEmptyObject(data) {
  return object(data) && Object.keys(data).length > 0;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.nonEmptyString"></a>[function <span class="apidocSignatureSpan">check-types.</span>nonEmptyString (data)](#apidoc.element.check-types.nonEmptyString)
- description and source-code
```javascript
function nonEmptyString(data) {
  return string(data) && data !== '';
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
...
```

#### <a name="apidoc.element.check-types.not"></a>[function <span class="apidocSignatureSpan">check-types.</span>not (value)](#apidoc.element.check-types.not)
- description and source-code
```javascript
function notImpl(value) {
  return !value;
}
```
- example usage
```shell
...
* 'check.function(thing)':
Returns 'true'
if 'thing' is a function,
'false' otherwise.

#### Modifiers

* 'check.not(value)':
Returns the negation
of 'value'.

* 'check.not.xxx(...)':
Returns the negation
of the predicate.
...
```

#### <a name="apidoc.element.check-types.null"></a>[function <span class="apidocSignatureSpan">check-types.</span>null (data)](#apidoc.element.check-types.null)
- description and source-code
```javascript
function isNull(data) {
  return data === null;
}
```
- example usage
```shell
...
#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
...
```

#### <a name="apidoc.element.check-types.number"></a>[function <span class="apidocSignatureSpan">check-types.</span>number (data)](#apidoc.element.check-types.number)
- description and source-code
```javascript
function number(data) {
  return typeof data === 'number' &&
    isNaN(data) === false &&
    data !== Number.POSITIVE_INFINITY &&
    data !== Number.NEGATIVE_INFINITY;
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' is a string
that matches 'regex',
'false' otherwise.

#### Number predicates

* 'check.number(thing)':
Returns 'true'
if 'thing' is a number,
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
...
```

#### <a name="apidoc.element.check-types.object"></a>[function <span class="apidocSignatureSpan">check-types.</span>object (data)](#apidoc.element.check-types.object)
- description and source-code
```javascript
function object(data) {
  return Object.prototype.toString.call(data) === '[object Object]';
}
```
- example usage
```shell
...
* 'check.boolean(thing)':
Returns 'true'
if 'thing' is a boolean,
'false' otherwise.

#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
...
```

#### <a name="apidoc.element.check-types.odd"></a>[function <span class="apidocSignatureSpan">check-types.</span>odd (data)](#apidoc.element.check-types.odd)
- description and source-code
```javascript
function odd(data) {
  return integer(data) && !even(data);
}
```
- example usage
```shell
...

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
if 'thing' is an odd number,
'false' otherwise.

* 'check.even(thing)':
Returns 'true'
if 'thing' is an even number,
...
```

#### <a name="apidoc.element.check-types.positive"></a>[function <span class="apidocSignatureSpan">check-types.</span>positive (data)](#apidoc.element.check-types.positive)
- description and source-code
```javascript
function positive(data) {
  return greater(data, 0);
}
```
- example usage
```shell
...
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
...
```

#### <a name="apidoc.element.check-types.string"></a>[function <span class="apidocSignatureSpan">check-types.</span>string (data)](#apidoc.element.check-types.string)
- description and source-code
```javascript
function string(data) {
  return typeof data === 'string';
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' has a length property
that equals 'value',
'false' otherwise.

#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
...
```

#### <a name="apidoc.element.check-types.undefined"></a>[function <span class="apidocSignatureSpan">check-types.</span>undefined (data)](#apidoc.element.check-types.undefined)
- description and source-code
```javascript
function isUndefined(data) {
  return data === undefined;
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
...
```

#### <a name="apidoc.element.check-types.zero"></a>[function <span class="apidocSignatureSpan">check-types.</span>zero (data)](#apidoc.element.check-types.zero)
- description and source-code
```javascript
function zero(data) {
  return data === 0;
}
```
- example usage
```shell
...
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
...
```



# <a name="apidoc.module.check-types.assert"></a>[module check-types.assert](#apidoc.module.check-types.assert)

#### <a name="apidoc.element.check-types.assert.assert"></a>[function <span class="apidocSignatureSpan">check-types.</span>assert (value, message, ErrorType)](#apidoc.element.check-types.assert.assert)
- description and source-code
```javascript
function assertImpl(value, message, ErrorType) {
  if (value === false) {
    throw new (ErrorType || Error)(message || 'Assertion failed');
  }
}
```
- example usage
```shell
...
except it operates on iterables.

* 'check.object.of.xxx(thing)':
The 'object.of' modifier
is synonymous with 'array.of',
except it operates on an object's properties.

* 'check.assert(value, message, ErrorType)':
Throws a 'TypeError'
if 'value' is 'false'.
'message' and 'ErrorType'
are optional arguments
that control
the message and type
of the thrown error object.
...
```

#### <a name="apidoc.element.check-types.assert.array"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>array ()](#apidoc.element.check-types.assert.array)
- description and source-code
```javascript
array = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Duck-typing checker.
Returns 'true'
if 'thing' has all of the properties of 'duck',
'false' otherwise.

#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
...
```

#### <a name="apidoc.element.check-types.assert.arrayLike"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>arrayLike ()](#apidoc.element.check-types.assert.arrayLike)
- description and source-code
```javascript
arrayLike = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
...
```

#### <a name="apidoc.element.check-types.assert.assigned"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>assigned ()](#apidoc.element.check-types.assert.assigned)
- description and source-code
```javascript
assigned = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
'null' or 'undefined',
'false' otherwise.

* 'check.hasLength(thing, value)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.between"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>between ()](#apidoc.element.check-types.assert.between)
- description and source-code
```javascript
between = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.assert.boolean"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>boolean ()](#apidoc.element.check-types.assert.boolean)
- description and source-code
```javascript
boolean = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
  Returns 'true'
  if 'thing' is a boolean,
  'false' otherwise.

#### Object predicates

* 'check.object(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.contains"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>contains ()](#apidoc.element.check-types.assert.contains)
- description and source-code
```javascript
contains = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
that contains 'substring',
'false' otherwise.

* 'check.match(thing, regex)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.date"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>date ()](#apidoc.element.check-types.assert.date)
- description and source-code
```javascript
date = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.emptyArray"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>emptyArray ()](#apidoc.element.check-types.assert.emptyArray)
- description and source-code
```javascript
emptyArray = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
...
```

#### <a name="apidoc.element.check-types.assert.emptyObject"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>emptyObject ()](#apidoc.element.check-types.assert.emptyObject)
- description and source-code
```javascript
emptyObject = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
...
```

#### <a name="apidoc.element.check-types.assert.emptyString"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>emptyString ()](#apidoc.element.check-types.assert.emptyString)
- description and source-code
```javascript
emptyString = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
...
```

#### <a name="apidoc.element.check-types.assert.equal"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>equal ()](#apidoc.element.check-types.assert.equal)
- description and source-code
```javascript
equal = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'check.apply',
'check.map',
'check.any' and
'check.all'.

#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
...
```

#### <a name="apidoc.element.check-types.assert.even"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>even ()](#apidoc.element.check-types.assert.even)
- description and source-code
```javascript
even = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  'false' otherwise.

* 'check.odd(thing)':
  Returns 'true'
  if 'thing' is an odd number,
  'false' otherwise.

* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.function"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>function ()](#apidoc.element.check-types.assert.function)
- description and source-code
```javascript
function = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
  Returns 'true'
  if 'thing' is a function,
  'false' otherwise.

#### Modifiers

* 'check.not(value)':
...
```

#### <a name="apidoc.element.check-types.assert.greater"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>greater ()](#apidoc.element.check-types.assert.greater)
- description and source-code
```javascript
greater = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.assert.greaterOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>greaterOrEqual ()](#apidoc.element.check-types.assert.greaterOrEqual)
- description and source-code
```javascript
greaterOrEqual = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
...
```

#### <a name="apidoc.element.check-types.assert.hasLength"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>hasLength ()](#apidoc.element.check-types.assert.hasLength)
- description and source-code
```javascript
hasLength = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.assigned(thing)':
  Returns 'true'
  if 'thing' is not
  'null' or 'undefined',
  'false' otherwise.

* 'check.hasLength(thing, value)':
  Returns 'true'
  if 'thing' has a length property
  that equals 'value',
  'false' otherwise.

#### String predicates
...
```

#### <a name="apidoc.element.check-types.assert.inRange"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>inRange ()](#apidoc.element.check-types.assert.inRange)
- description and source-code
```javascript
inRange = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.inRange(thing, a, b)':
Returns 'true' if 'thing' is a number
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.assert.includes"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>includes ()](#apidoc.element.check-types.assert.includes)
- description and source-code
```javascript
includes = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' implements the iterable protocol,
  'false' otherwise.
  In pre-ES6 environments,
  this predicate falls back
  to 'arrayLike' behaviour.

* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.infinity"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>infinity ()](#apidoc.element.check-types.assert.infinity)
- description and source-code
```javascript
infinity = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
...
```

#### <a name="apidoc.element.check-types.assert.instance"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>instance ()](#apidoc.element.check-types.assert.instance)
- description and source-code
```javascript
instance = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.
Falls back to testing
'constructor.name' and 'Object.prototype.toString'
if the 'instanceof' test fails.
...
```

#### <a name="apidoc.element.check-types.assert.instanceStrict"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>instanceStrict ()](#apidoc.element.check-types.assert.instanceStrict)
- description and source-code
```javascript
instanceStrict = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.assert.integer"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>integer ()](#apidoc.element.check-types.assert.integer)
- description and source-code
```javascript
integer = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
...
```

#### <a name="apidoc.element.check-types.assert.iterable"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>iterable ()](#apidoc.element.check-types.assert.iterable)
- description and source-code
```javascript
iterable = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
'false' otherwise.
In pre-ES6 environments,
this predicate falls back
to 'arrayLike' behaviour.
...
```

#### <a name="apidoc.element.check-types.assert.less"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>less ()](#apidoc.element.check-types.assert.less)
- description and source-code
```javascript
less = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.assert.lessOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>lessOrEqual ()](#apidoc.element.check-types.assert.lessOrEqual)
- description and source-code
```javascript
lessOrEqual = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
...
```

#### <a name="apidoc.element.check-types.assert.like"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>like ()](#apidoc.element.check-types.assert.like)
- description and source-code
```javascript
like = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' is an instance of 'prototype',
  'false' otherwise.
  Falls back to testing
  'constructor.name' and 'Object.prototype.toString'
  if the 'instanceof' test fails.

* 'check.like(thing, duck)':
  Duck-typing checker.
  Returns 'true'
  if 'thing' has all of the properties of 'duck',
  'false' otherwise.

#### Array predicates
...
```

#### <a name="apidoc.element.check-types.assert.match"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>match ()](#apidoc.element.check-types.assert.match)
- description and source-code
```javascript
match = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.contains(thing, substring)':
  Returns 'true'
  if 'thing' is a string
  that contains 'substring',
  'false' otherwise.

* 'check.match(thing, regex)':
  Returns 'true'
  if 'thing' is a string
  that matches 'regex',
  'false' otherwise.

#### Number predicates
...
```

#### <a name="apidoc.element.check-types.assert.negative"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>negative ()](#apidoc.element.check-types.assert.negative)
- description and source-code
```javascript
negative = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.nonEmptyArray"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>nonEmptyArray ()](#apidoc.element.check-types.assert.nonEmptyArray)
- description and source-code
```javascript
nonEmptyArray = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
...
```

#### <a name="apidoc.element.check-types.assert.nonEmptyObject"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>nonEmptyObject ()](#apidoc.element.check-types.assert.nonEmptyObject)
- description and source-code
```javascript
nonEmptyObject = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.assert.nonEmptyString"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>nonEmptyString ()](#apidoc.element.check-types.assert.nonEmptyString)
- description and source-code
```javascript
nonEmptyString = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
...
```

#### <a name="apidoc.element.check-types.assert.null"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>null ()](#apidoc.element.check-types.assert.null)
- description and source-code
```javascript
null = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
...
```

#### <a name="apidoc.element.check-types.assert.number"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>number ()](#apidoc.element.check-types.assert.number)
- description and source-code
```javascript
number = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' is a string
that matches 'regex',
'false' otherwise.

#### Number predicates

* 'check.number(thing)':
Returns 'true'
if 'thing' is a number,
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
...
```

#### <a name="apidoc.element.check-types.assert.object"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>object ()](#apidoc.element.check-types.assert.object)
- description and source-code
```javascript
object = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.boolean(thing)':
Returns 'true'
if 'thing' is a boolean,
'false' otherwise.

#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
...
```

#### <a name="apidoc.element.check-types.assert.odd"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>odd ()](#apidoc.element.check-types.assert.odd)
- description and source-code
```javascript
odd = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
if 'thing' is an odd number,
'false' otherwise.

* 'check.even(thing)':
Returns 'true'
if 'thing' is an even number,
...
```

#### <a name="apidoc.element.check-types.assert.positive"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>positive ()](#apidoc.element.check-types.assert.positive)
- description and source-code
```javascript
positive = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
...
```

#### <a name="apidoc.element.check-types.assert.string"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>string ()](#apidoc.element.check-types.assert.string)
- description and source-code
```javascript
string = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' has a length property
that equals 'value',
'false' otherwise.

#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
...
```

#### <a name="apidoc.element.check-types.assert.undefined"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>undefined ()](#apidoc.element.check-types.assert.undefined)
- description and source-code
```javascript
undefined = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
...
```

#### <a name="apidoc.element.check-types.assert.zero"></a>[function <span class="apidocSignatureSpan">check-types.assert.</span>zero ()](#apidoc.element.check-types.assert.zero)
- description and source-code
```javascript
zero = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
...
```



# <a name="apidoc.module.check-types.assert.maybe"></a>[module check-types.assert.maybe](#apidoc.module.check-types.assert.maybe)

#### <a name="apidoc.element.check-types.assert.maybe.array"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>array ()](#apidoc.element.check-types.assert.maybe.array)
- description and source-code
```javascript
array = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Duck-typing checker.
Returns 'true'
if 'thing' has all of the properties of 'duck',
'false' otherwise.

#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.arrayLike"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>arrayLike ()](#apidoc.element.check-types.assert.maybe.arrayLike)
- description and source-code
```javascript
arrayLike = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.assigned"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>assigned ()](#apidoc.element.check-types.assert.maybe.assigned)
- description and source-code
```javascript
assigned = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
'null' or 'undefined',
'false' otherwise.

* 'check.hasLength(thing, value)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.maybe.between"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>between ()](#apidoc.element.check-types.assert.maybe.between)
- description and source-code
```javascript
between = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.assert.maybe.boolean"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>boolean ()](#apidoc.element.check-types.assert.maybe.boolean)
- description and source-code
```javascript
boolean = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
  Returns 'true'
  if 'thing' is a boolean,
  'false' otherwise.

#### Object predicates

* 'check.object(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.maybe.contains"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>contains ()](#apidoc.element.check-types.assert.maybe.contains)
- description and source-code
```javascript
contains = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
that contains 'substring',
'false' otherwise.

* 'check.match(thing, regex)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.maybe.date"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>date ()](#apidoc.element.check-types.assert.maybe.date)
- description and source-code
```javascript
date = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.maybe.emptyArray"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>emptyArray ()](#apidoc.element.check-types.assert.maybe.emptyArray)
- description and source-code
```javascript
emptyArray = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.emptyObject"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>emptyObject ()](#apidoc.element.check-types.assert.maybe.emptyObject)
- description and source-code
```javascript
emptyObject = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.emptyString"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>emptyString ()](#apidoc.element.check-types.assert.maybe.emptyString)
- description and source-code
```javascript
emptyString = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.equal"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>equal ()](#apidoc.element.check-types.assert.maybe.equal)
- description and source-code
```javascript
equal = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'check.apply',
'check.map',
'check.any' and
'check.all'.

#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.even"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>even ()](#apidoc.element.check-types.assert.maybe.even)
- description and source-code
```javascript
even = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  'false' otherwise.

* 'check.odd(thing)':
  Returns 'true'
  if 'thing' is an odd number,
  'false' otherwise.

* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.maybe.function"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>function ()](#apidoc.element.check-types.assert.maybe.function)
- description and source-code
```javascript
function = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
  Returns 'true'
  if 'thing' is a function,
  'false' otherwise.

#### Modifiers

* 'check.not(value)':
...
```

#### <a name="apidoc.element.check-types.assert.maybe.greater"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>greater ()](#apidoc.element.check-types.assert.maybe.greater)
- description and source-code
```javascript
greater = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.greaterOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>greaterOrEqual ()](#apidoc.element.check-types.assert.maybe.greaterOrEqual)
- description and source-code
```javascript
greaterOrEqual = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.hasLength"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>hasLength ()](#apidoc.element.check-types.assert.maybe.hasLength)
- description and source-code
```javascript
hasLength = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.assigned(thing)':
  Returns 'true'
  if 'thing' is not
  'null' or 'undefined',
  'false' otherwise.

* 'check.hasLength(thing, value)':
  Returns 'true'
  if 'thing' has a length property
  that equals 'value',
  'false' otherwise.

#### String predicates
...
```

#### <a name="apidoc.element.check-types.assert.maybe.inRange"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>inRange ()](#apidoc.element.check-types.assert.maybe.inRange)
- description and source-code
```javascript
inRange = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.inRange(thing, a, b)':
Returns 'true' if 'thing' is a number
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.assert.maybe.includes"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>includes ()](#apidoc.element.check-types.assert.maybe.includes)
- description and source-code
```javascript
includes = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' implements the iterable protocol,
  'false' otherwise.
  In pre-ES6 environments,
  this predicate falls back
  to 'arrayLike' behaviour.

* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.maybe.infinity"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>infinity ()](#apidoc.element.check-types.assert.maybe.infinity)
- description and source-code
```javascript
infinity = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.instance"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>instance ()](#apidoc.element.check-types.assert.maybe.instance)
- description and source-code
```javascript
instance = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.
Falls back to testing
'constructor.name' and 'Object.prototype.toString'
if the 'instanceof' test fails.
...
```

#### <a name="apidoc.element.check-types.assert.maybe.instanceStrict"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>instanceStrict ()](#apidoc.element.check-types.assert.maybe.instanceStrict)
- description and source-code
```javascript
instanceStrict = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.integer"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>integer ()](#apidoc.element.check-types.assert.maybe.integer)
- description and source-code
```javascript
integer = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.iterable"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>iterable ()](#apidoc.element.check-types.assert.maybe.iterable)
- description and source-code
```javascript
iterable = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
'false' otherwise.
In pre-ES6 environments,
this predicate falls back
to 'arrayLike' behaviour.
...
```

#### <a name="apidoc.element.check-types.assert.maybe.less"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>less ()](#apidoc.element.check-types.assert.maybe.less)
- description and source-code
```javascript
less = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.lessOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>lessOrEqual ()](#apidoc.element.check-types.assert.maybe.lessOrEqual)
- description and source-code
```javascript
lessOrEqual = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.like"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>like ()](#apidoc.element.check-types.assert.maybe.like)
- description and source-code
```javascript
like = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' is an instance of 'prototype',
  'false' otherwise.
  Falls back to testing
  'constructor.name' and 'Object.prototype.toString'
  if the 'instanceof' test fails.

* 'check.like(thing, duck)':
  Duck-typing checker.
  Returns 'true'
  if 'thing' has all of the properties of 'duck',
  'false' otherwise.

#### Array predicates
...
```

#### <a name="apidoc.element.check-types.assert.maybe.match"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>match ()](#apidoc.element.check-types.assert.maybe.match)
- description and source-code
```javascript
match = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.contains(thing, substring)':
  Returns 'true'
  if 'thing' is a string
  that contains 'substring',
  'false' otherwise.

* 'check.match(thing, regex)':
  Returns 'true'
  if 'thing' is a string
  that matches 'regex',
  'false' otherwise.

#### Number predicates
...
```

#### <a name="apidoc.element.check-types.assert.maybe.negative"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>negative ()](#apidoc.element.check-types.assert.maybe.negative)
- description and source-code
```javascript
negative = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.maybe.nonEmptyArray"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>nonEmptyArray ()](#apidoc.element.check-types.assert.maybe.nonEmptyArray)
- description and source-code
```javascript
nonEmptyArray = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.nonEmptyObject"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>nonEmptyObject ()](#apidoc.element.check-types.assert.maybe.nonEmptyObject)
- description and source-code
```javascript
nonEmptyObject = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.nonEmptyString"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>nonEmptyString ()](#apidoc.element.check-types.assert.maybe.nonEmptyString)
- description and source-code
```javascript
nonEmptyString = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
...
```

#### <a name="apidoc.element.check-types.assert.maybe.null"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>null ()](#apidoc.element.check-types.assert.maybe.null)
- description and source-code
```javascript
null = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
...
```

#### <a name="apidoc.element.check-types.assert.maybe.number"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>number ()](#apidoc.element.check-types.assert.maybe.number)
- description and source-code
```javascript
number = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' is a string
that matches 'regex',
'false' otherwise.

#### Number predicates

* 'check.number(thing)':
Returns 'true'
if 'thing' is a number,
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
...
```

#### <a name="apidoc.element.check-types.assert.maybe.object"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>object ()](#apidoc.element.check-types.assert.maybe.object)
- description and source-code
```javascript
object = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.boolean(thing)':
Returns 'true'
if 'thing' is a boolean,
'false' otherwise.

#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.odd"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>odd ()](#apidoc.element.check-types.assert.maybe.odd)
- description and source-code
```javascript
odd = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
if 'thing' is an odd number,
'false' otherwise.

* 'check.even(thing)':
Returns 'true'
if 'thing' is an even number,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.positive"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>positive ()](#apidoc.element.check-types.assert.maybe.positive)
- description and source-code
```javascript
positive = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
...
```

#### <a name="apidoc.element.check-types.assert.maybe.string"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>string ()](#apidoc.element.check-types.assert.maybe.string)
- description and source-code
```javascript
string = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' has a length property
that equals 'value',
'false' otherwise.

#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
...
```

#### <a name="apidoc.element.check-types.assert.maybe.undefined"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>undefined ()](#apidoc.element.check-types.assert.maybe.undefined)
- description and source-code
```javascript
undefined = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
...
```

#### <a name="apidoc.element.check-types.assert.maybe.zero"></a>[function <span class="apidocSignatureSpan">check-types.assert.maybe.</span>zero ()](#apidoc.element.check-types.assert.maybe.zero)
- description and source-code
```javascript
zero = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
...
```



# <a name="apidoc.module.check-types.assert.not"></a>[module check-types.assert.not](#apidoc.module.check-types.assert.not)

#### <a name="apidoc.element.check-types.assert.not.array"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>array ()](#apidoc.element.check-types.assert.not.array)
- description and source-code
```javascript
array = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Duck-typing checker.
Returns 'true'
if 'thing' has all of the properties of 'duck',
'false' otherwise.

#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
...
```

#### <a name="apidoc.element.check-types.assert.not.arrayLike"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>arrayLike ()](#apidoc.element.check-types.assert.not.arrayLike)
- description and source-code
```javascript
arrayLike = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
...
```

#### <a name="apidoc.element.check-types.assert.not.assigned"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>assigned ()](#apidoc.element.check-types.assert.not.assigned)
- description and source-code
```javascript
assigned = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
'null' or 'undefined',
'false' otherwise.

* 'check.hasLength(thing, value)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.not.between"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>between ()](#apidoc.element.check-types.assert.not.between)
- description and source-code
```javascript
between = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.assert.not.boolean"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>boolean ()](#apidoc.element.check-types.assert.not.boolean)
- description and source-code
```javascript
boolean = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
  Returns 'true'
  if 'thing' is a boolean,
  'false' otherwise.

#### Object predicates

* 'check.object(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.not.contains"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>contains ()](#apidoc.element.check-types.assert.not.contains)
- description and source-code
```javascript
contains = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
that contains 'substring',
'false' otherwise.

* 'check.match(thing, regex)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.not.date"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>date ()](#apidoc.element.check-types.assert.not.date)
- description and source-code
```javascript
date = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.not.emptyArray"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>emptyArray ()](#apidoc.element.check-types.assert.not.emptyArray)
- description and source-code
```javascript
emptyArray = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
...
```

#### <a name="apidoc.element.check-types.assert.not.emptyObject"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>emptyObject ()](#apidoc.element.check-types.assert.not.emptyObject)
- description and source-code
```javascript
emptyObject = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
...
```

#### <a name="apidoc.element.check-types.assert.not.emptyString"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>emptyString ()](#apidoc.element.check-types.assert.not.emptyString)
- description and source-code
```javascript
emptyString = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
...
```

#### <a name="apidoc.element.check-types.assert.not.equal"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>equal ()](#apidoc.element.check-types.assert.not.equal)
- description and source-code
```javascript
equal = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'check.apply',
'check.map',
'check.any' and
'check.all'.

#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
...
```

#### <a name="apidoc.element.check-types.assert.not.even"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>even ()](#apidoc.element.check-types.assert.not.even)
- description and source-code
```javascript
even = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  'false' otherwise.

* 'check.odd(thing)':
  Returns 'true'
  if 'thing' is an odd number,
  'false' otherwise.

* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.not.function"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>function ()](#apidoc.element.check-types.assert.not.function)
- description and source-code
```javascript
function = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
  Returns 'true'
  if 'thing' is a function,
  'false' otherwise.

#### Modifiers

* 'check.not(value)':
...
```

#### <a name="apidoc.element.check-types.assert.not.greater"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>greater ()](#apidoc.element.check-types.assert.not.greater)
- description and source-code
```javascript
greater = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.assert.not.greaterOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>greaterOrEqual ()](#apidoc.element.check-types.assert.not.greaterOrEqual)
- description and source-code
```javascript
greaterOrEqual = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
...
```

#### <a name="apidoc.element.check-types.assert.not.hasLength"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>hasLength ()](#apidoc.element.check-types.assert.not.hasLength)
- description and source-code
```javascript
hasLength = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.assigned(thing)':
  Returns 'true'
  if 'thing' is not
  'null' or 'undefined',
  'false' otherwise.

* 'check.hasLength(thing, value)':
  Returns 'true'
  if 'thing' has a length property
  that equals 'value',
  'false' otherwise.

#### String predicates
...
```

#### <a name="apidoc.element.check-types.assert.not.inRange"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>inRange ()](#apidoc.element.check-types.assert.not.inRange)
- description and source-code
```javascript
inRange = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.inRange(thing, a, b)':
Returns 'true' if 'thing' is a number
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.assert.not.includes"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>includes ()](#apidoc.element.check-types.assert.not.includes)
- description and source-code
```javascript
includes = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' implements the iterable protocol,
  'false' otherwise.
  In pre-ES6 environments,
  this predicate falls back
  to 'arrayLike' behaviour.

* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
...
```

#### <a name="apidoc.element.check-types.assert.not.infinity"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>infinity ()](#apidoc.element.check-types.assert.not.infinity)
- description and source-code
```javascript
infinity = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
...
```

#### <a name="apidoc.element.check-types.assert.not.instance"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>instance ()](#apidoc.element.check-types.assert.not.instance)
- description and source-code
```javascript
instance = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.
Falls back to testing
'constructor.name' and 'Object.prototype.toString'
if the 'instanceof' test fails.
...
```

#### <a name="apidoc.element.check-types.assert.not.instanceStrict"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>instanceStrict ()](#apidoc.element.check-types.assert.not.instanceStrict)
- description and source-code
```javascript
instanceStrict = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.assert.not.integer"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>integer ()](#apidoc.element.check-types.assert.not.integer)
- description and source-code
```javascript
integer = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
...
```

#### <a name="apidoc.element.check-types.assert.not.iterable"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>iterable ()](#apidoc.element.check-types.assert.not.iterable)
- description and source-code
```javascript
iterable = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
'false' otherwise.
In pre-ES6 environments,
this predicate falls back
to 'arrayLike' behaviour.
...
```

#### <a name="apidoc.element.check-types.assert.not.less"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>less ()](#apidoc.element.check-types.assert.not.less)
- description and source-code
```javascript
less = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.assert.not.lessOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>lessOrEqual ()](#apidoc.element.check-types.assert.not.lessOrEqual)
- description and source-code
```javascript
lessOrEqual = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
...
```

#### <a name="apidoc.element.check-types.assert.not.like"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>like ()](#apidoc.element.check-types.assert.not.like)
- description and source-code
```javascript
like = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' is an instance of 'prototype',
  'false' otherwise.
  Falls back to testing
  'constructor.name' and 'Object.prototype.toString'
  if the 'instanceof' test fails.

* 'check.like(thing, duck)':
  Duck-typing checker.
  Returns 'true'
  if 'thing' has all of the properties of 'duck',
  'false' otherwise.

#### Array predicates
...
```

#### <a name="apidoc.element.check-types.assert.not.match"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>match ()](#apidoc.element.check-types.assert.not.match)
- description and source-code
```javascript
match = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.contains(thing, substring)':
  Returns 'true'
  if 'thing' is a string
  that contains 'substring',
  'false' otherwise.

* 'check.match(thing, regex)':
  Returns 'true'
  if 'thing' is a string
  that matches 'regex',
  'false' otherwise.

#### Number predicates
...
```

#### <a name="apidoc.element.check-types.assert.not.negative"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>negative ()](#apidoc.element.check-types.assert.not.negative)
- description and source-code
```javascript
negative = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.assert.not.nonEmptyArray"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>nonEmptyArray ()](#apidoc.element.check-types.assert.not.nonEmptyArray)
- description and source-code
```javascript
nonEmptyArray = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
...
```

#### <a name="apidoc.element.check-types.assert.not.nonEmptyObject"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>nonEmptyObject ()](#apidoc.element.check-types.assert.not.nonEmptyObject)
- description and source-code
```javascript
nonEmptyObject = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.assert.not.nonEmptyString"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>nonEmptyString ()](#apidoc.element.check-types.assert.not.nonEmptyString)
- description and source-code
```javascript
nonEmptyString = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
...
```

#### <a name="apidoc.element.check-types.assert.not.null"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>null ()](#apidoc.element.check-types.assert.not.null)
- description and source-code
```javascript
null = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
...
```

#### <a name="apidoc.element.check-types.assert.not.number"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>number ()](#apidoc.element.check-types.assert.not.number)
- description and source-code
```javascript
number = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' is a string
that matches 'regex',
'false' otherwise.

#### Number predicates

* 'check.number(thing)':
Returns 'true'
if 'thing' is a number,
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
...
```

#### <a name="apidoc.element.check-types.assert.not.object"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>object ()](#apidoc.element.check-types.assert.not.object)
- description and source-code
```javascript
object = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
* 'check.boolean(thing)':
Returns 'true'
if 'thing' is a boolean,
'false' otherwise.

#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
...
```

#### <a name="apidoc.element.check-types.assert.not.odd"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>odd ()](#apidoc.element.check-types.assert.not.odd)
- description and source-code
```javascript
odd = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
if 'thing' is an odd number,
'false' otherwise.

* 'check.even(thing)':
Returns 'true'
if 'thing' is an even number,
...
```

#### <a name="apidoc.element.check-types.assert.not.positive"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>positive ()](#apidoc.element.check-types.assert.not.positive)
- description and source-code
```javascript
positive = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
...
```

#### <a name="apidoc.element.check-types.assert.not.string"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>string ()](#apidoc.element.check-types.assert.not.string)
- description and source-code
```javascript
string = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' has a length property
that equals 'value',
'false' otherwise.

#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
...
```

#### <a name="apidoc.element.check-types.assert.not.undefined"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>undefined ()](#apidoc.element.check-types.assert.not.undefined)
- description and source-code
```javascript
undefined = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
...
```

#### <a name="apidoc.element.check-types.assert.not.zero"></a>[function <span class="apidocSignatureSpan">check-types.assert.not.</span>zero ()](#apidoc.element.check-types.assert.not.zero)
- description and source-code
```javascript
zero = function () {
  assertPredicate(predicate, arguments, defaultMessage);
}
```
- example usage
```shell
...
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
...
```



# <a name="apidoc.module.check-types.maybe"></a>[module check-types.maybe](#apidoc.module.check-types.maybe)

#### <a name="apidoc.element.check-types.maybe.maybe"></a>[function <span class="apidocSignatureSpan">check-types.</span>maybe (value)](#apidoc.element.check-types.maybe.maybe)
- description and source-code
```javascript
function maybeImpl(value) {
  if (assigned(value) === false) {
    return true;
  }

  return value;
}
```
- example usage
```shell
...
Returns the negation
of 'value'.

* 'check.not.xxx(...)':
Returns the negation
of the predicate.

* 'check.maybe(value)':
Returns 'true'
if 'value' is 'null' or 'undefined',
otherwise it returns 'value'.

* 'check.maybe.xxx(...)':
Returns 'true'
if 'thing' is 'null' or 'undefined',
...
```

#### <a name="apidoc.element.check-types.maybe.array"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>array ()](#apidoc.element.check-types.maybe.array)
- description and source-code
```javascript
array = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
Duck-typing checker.
Returns 'true'
if 'thing' has all of the properties of 'duck',
'false' otherwise.

#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
...
```

#### <a name="apidoc.element.check-types.maybe.arrayLike"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>arrayLike ()](#apidoc.element.check-types.maybe.arrayLike)
- description and source-code
```javascript
arrayLike = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
...
```

#### <a name="apidoc.element.check-types.maybe.assigned"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>assigned ()](#apidoc.element.check-types.maybe.assigned)
- description and source-code
```javascript
assigned = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
'null' or 'undefined',
'false' otherwise.

* 'check.hasLength(thing, value)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.maybe.between"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>between ()](#apidoc.element.check-types.maybe.between)
- description and source-code
```javascript
between = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.maybe.boolean"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>boolean ()](#apidoc.element.check-types.maybe.boolean)
- description and source-code
```javascript
boolean = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
  Returns 'true'
  if 'thing' is a boolean,
  'false' otherwise.

#### Object predicates

* 'check.object(thing)':
...
```

#### <a name="apidoc.element.check-types.maybe.contains"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>contains ()](#apidoc.element.check-types.maybe.contains)
- description and source-code
```javascript
contains = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
that contains 'substring',
'false' otherwise.

* 'check.match(thing, regex)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.maybe.date"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>date ()](#apidoc.element.check-types.maybe.date)
- description and source-code
```javascript
date = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
...
```

#### <a name="apidoc.element.check-types.maybe.emptyArray"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>emptyArray ()](#apidoc.element.check-types.maybe.emptyArray)
- description and source-code
```javascript
emptyArray = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
...
```

#### <a name="apidoc.element.check-types.maybe.emptyObject"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>emptyObject ()](#apidoc.element.check-types.maybe.emptyObject)
- description and source-code
```javascript
emptyObject = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
...
```

#### <a name="apidoc.element.check-types.maybe.emptyString"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>emptyString ()](#apidoc.element.check-types.maybe.emptyString)
- description and source-code
```javascript
emptyString = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
...
```

#### <a name="apidoc.element.check-types.maybe.equal"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>equal ()](#apidoc.element.check-types.maybe.equal)
- description and source-code
```javascript
equal = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'check.apply',
'check.map',
'check.any' and
'check.all'.

#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
...
```

#### <a name="apidoc.element.check-types.maybe.even"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>even ()](#apidoc.element.check-types.maybe.even)
- description and source-code
```javascript
even = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
  'false' otherwise.

* 'check.odd(thing)':
  Returns 'true'
  if 'thing' is an odd number,
  'false' otherwise.

* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
...
```

#### <a name="apidoc.element.check-types.maybe.function"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>function ()](#apidoc.element.check-types.maybe.function)
- description and source-code
```javascript
function = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
  Returns 'true'
  if 'thing' is a function,
  'false' otherwise.

#### Modifiers

* 'check.not(value)':
...
```

#### <a name="apidoc.element.check-types.maybe.greater"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>greater ()](#apidoc.element.check-types.maybe.greater)
- description and source-code
```javascript
greater = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.maybe.greaterOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>greaterOrEqual ()](#apidoc.element.check-types.maybe.greaterOrEqual)
- description and source-code
```javascript
greaterOrEqual = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
...
```

#### <a name="apidoc.element.check-types.maybe.hasLength"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>hasLength ()](#apidoc.element.check-types.maybe.hasLength)
- description and source-code
```javascript
hasLength = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...

* 'check.assigned(thing)':
  Returns 'true'
  if 'thing' is not
  'null' or 'undefined',
  'false' otherwise.

* 'check.hasLength(thing, value)':
  Returns 'true'
  if 'thing' has a length property
  that equals 'value',
  'false' otherwise.

#### String predicates
...
```

#### <a name="apidoc.element.check-types.maybe.inRange"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>inRange ()](#apidoc.element.check-types.maybe.inRange)
- description and source-code
```javascript
inRange = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.inRange(thing, a, b)':
Returns 'true' if 'thing' is a number
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.maybe.includes"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>includes ()](#apidoc.element.check-types.maybe.includes)
- description and source-code
```javascript
includes = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' implements the iterable protocol,
  'false' otherwise.
  In pre-ES6 environments,
  this predicate falls back
  to 'arrayLike' behaviour.

* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
...
```

#### <a name="apidoc.element.check-types.maybe.infinity"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>infinity ()](#apidoc.element.check-types.maybe.infinity)
- description and source-code
```javascript
infinity = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
...
```

#### <a name="apidoc.element.check-types.maybe.instance"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>instance ()](#apidoc.element.check-types.maybe.instance)
- description and source-code
```javascript
instance = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.
Falls back to testing
'constructor.name' and 'Object.prototype.toString'
if the 'instanceof' test fails.
...
```

#### <a name="apidoc.element.check-types.maybe.instanceStrict"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>instanceStrict ()](#apidoc.element.check-types.maybe.instanceStrict)
- description and source-code
```javascript
instanceStrict = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.maybe.integer"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>integer ()](#apidoc.element.check-types.maybe.integer)
- description and source-code
```javascript
integer = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
...
```

#### <a name="apidoc.element.check-types.maybe.iterable"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>iterable ()](#apidoc.element.check-types.maybe.iterable)
- description and source-code
```javascript
iterable = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
'false' otherwise.
In pre-ES6 environments,
this predicate falls back
to 'arrayLike' behaviour.
...
```

#### <a name="apidoc.element.check-types.maybe.less"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>less ()](#apidoc.element.check-types.maybe.less)
- description and source-code
```javascript
less = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.maybe.lessOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>lessOrEqual ()](#apidoc.element.check-types.maybe.lessOrEqual)
- description and source-code
```javascript
lessOrEqual = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
...
```

#### <a name="apidoc.element.check-types.maybe.like"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>like ()](#apidoc.element.check-types.maybe.like)
- description and source-code
```javascript
like = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' is an instance of 'prototype',
  'false' otherwise.
  Falls back to testing
  'constructor.name' and 'Object.prototype.toString'
  if the 'instanceof' test fails.

* 'check.like(thing, duck)':
  Duck-typing checker.
  Returns 'true'
  if 'thing' has all of the properties of 'duck',
  'false' otherwise.

#### Array predicates
...
```

#### <a name="apidoc.element.check-types.maybe.match"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>match ()](#apidoc.element.check-types.maybe.match)
- description and source-code
```javascript
match = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...

* 'check.contains(thing, substring)':
  Returns 'true'
  if 'thing' is a string
  that contains 'substring',
  'false' otherwise.

* 'check.match(thing, regex)':
  Returns 'true'
  if 'thing' is a string
  that matches 'regex',
  'false' otherwise.

#### Number predicates
...
```

#### <a name="apidoc.element.check-types.maybe.negative"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>negative ()](#apidoc.element.check-types.maybe.negative)
- description and source-code
```javascript
negative = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.maybe.nonEmptyArray"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>nonEmptyArray ()](#apidoc.element.check-types.maybe.nonEmptyArray)
- description and source-code
```javascript
nonEmptyArray = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
...
```

#### <a name="apidoc.element.check-types.maybe.nonEmptyObject"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>nonEmptyObject ()](#apidoc.element.check-types.maybe.nonEmptyObject)
- description and source-code
```javascript
nonEmptyObject = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.maybe.nonEmptyString"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>nonEmptyString ()](#apidoc.element.check-types.maybe.nonEmptyString)
- description and source-code
```javascript
nonEmptyString = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
...
```

#### <a name="apidoc.element.check-types.maybe.null"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>null ()](#apidoc.element.check-types.maybe.null)
- description and source-code
```javascript
null = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
...
```

#### <a name="apidoc.element.check-types.maybe.number"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>number ()](#apidoc.element.check-types.maybe.number)
- description and source-code
```javascript
number = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' is a string
that matches 'regex',
'false' otherwise.

#### Number predicates

* 'check.number(thing)':
Returns 'true'
if 'thing' is a number,
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
...
```

#### <a name="apidoc.element.check-types.maybe.object"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>object ()](#apidoc.element.check-types.maybe.object)
- description and source-code
```javascript
object = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
* 'check.boolean(thing)':
Returns 'true'
if 'thing' is a boolean,
'false' otherwise.

#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
...
```

#### <a name="apidoc.element.check-types.maybe.odd"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>odd ()](#apidoc.element.check-types.maybe.odd)
- description and source-code
```javascript
odd = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
if 'thing' is an odd number,
'false' otherwise.

* 'check.even(thing)':
Returns 'true'
if 'thing' is an even number,
...
```

#### <a name="apidoc.element.check-types.maybe.positive"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>positive ()](#apidoc.element.check-types.maybe.positive)
- description and source-code
```javascript
positive = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
...
```

#### <a name="apidoc.element.check-types.maybe.string"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>string ()](#apidoc.element.check-types.maybe.string)
- description and source-code
```javascript
string = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' has a length property
that equals 'value',
'false' otherwise.

#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
...
```

#### <a name="apidoc.element.check-types.maybe.undefined"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>undefined ()](#apidoc.element.check-types.maybe.undefined)
- description and source-code
```javascript
undefined = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
...
```

#### <a name="apidoc.element.check-types.maybe.zero"></a>[function <span class="apidocSignatureSpan">check-types.maybe.</span>zero ()](#apidoc.element.check-types.maybe.zero)
- description and source-code
```javascript
zero = function () {
  if (not.assigned(arguments[0])) {
    return true;
  }

  return predicate.apply(null, arguments);
}
```
- example usage
```shell
...
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
...
```



# <a name="apidoc.module.check-types.not"></a>[module check-types.not](#apidoc.module.check-types.not)

#### <a name="apidoc.element.check-types.not.not"></a>[function <span class="apidocSignatureSpan">check-types.</span>not (value)](#apidoc.element.check-types.not.not)
- description and source-code
```javascript
function notImpl(value) {
  return !value;
}
```
- example usage
```shell
...
* 'check.function(thing)':
Returns 'true'
if 'thing' is a function,
'false' otherwise.

#### Modifiers

* 'check.not(value)':
Returns the negation
of 'value'.

* 'check.not.xxx(...)':
Returns the negation
of the predicate.
...
```

#### <a name="apidoc.element.check-types.not.array"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>array ()](#apidoc.element.check-types.not.array)
- description and source-code
```javascript
array = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
Duck-typing checker.
Returns 'true'
if 'thing' has all of the properties of 'duck',
'false' otherwise.

#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
...
```

#### <a name="apidoc.element.check-types.not.arrayLike"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>arrayLike ()](#apidoc.element.check-types.not.arrayLike)
- description and source-code
```javascript
arrayLike = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
...
```

#### <a name="apidoc.element.check-types.not.assigned"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>assigned ()](#apidoc.element.check-types.not.assigned)
- description and source-code
```javascript
assigned = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
'null' or 'undefined',
'false' otherwise.

* 'check.hasLength(thing, value)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.not.between"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>between ()](#apidoc.element.check-types.not.between)
- description and source-code
```javascript
between = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.not.boolean"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>boolean ()](#apidoc.element.check-types.not.boolean)
- description and source-code
```javascript
boolean = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
  Returns 'true'
  if 'thing' is a boolean,
  'false' otherwise.

#### Object predicates

* 'check.object(thing)':
...
```

#### <a name="apidoc.element.check-types.not.contains"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>contains ()](#apidoc.element.check-types.not.contains)
- description and source-code
```javascript
contains = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
that contains 'substring',
'false' otherwise.

* 'check.match(thing, regex)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.not.date"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>date ()](#apidoc.element.check-types.not.date)
- description and source-code
```javascript
date = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
...
```

#### <a name="apidoc.element.check-types.not.emptyArray"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>emptyArray ()](#apidoc.element.check-types.not.emptyArray)
- description and source-code
```javascript
emptyArray = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
#### Array predicates

* 'check.array(thing)':
Returns 'true'
if 'thing' is an array,
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
...
```

#### <a name="apidoc.element.check-types.not.emptyObject"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>emptyObject ()](#apidoc.element.check-types.not.emptyObject)
- description and source-code
```javascript
emptyObject = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
...
```

#### <a name="apidoc.element.check-types.not.emptyString"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>emptyString ()](#apidoc.element.check-types.not.emptyString)
- description and source-code
```javascript
emptyString = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
...
```

#### <a name="apidoc.element.check-types.not.equal"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>equal ()](#apidoc.element.check-types.not.equal)
- description and source-code
```javascript
equal = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'check.apply',
'check.map',
'check.any' and
'check.all'.

#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
...
```

#### <a name="apidoc.element.check-types.not.even"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>even ()](#apidoc.element.check-types.not.even)
- description and source-code
```javascript
even = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
  'false' otherwise.

* 'check.odd(thing)':
  Returns 'true'
  if 'thing' is an odd number,
  'false' otherwise.

* 'check.even(thing)':
  Returns 'true'
  if 'thing' is an even number,
  'false' otherwise.

#### Boolean predicates

* 'check.boolean(thing)':
...
```

#### <a name="apidoc.element.check-types.not.function"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>function ()](#apidoc.element.check-types.not.function)
- description and source-code
```javascript
function = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
* 'check.date(thing)':
  Returns 'true'
  if 'thing' is a valid date,
  'false' otherwise.

#### Function predicates

* 'check.function(thing)':
  Returns 'true'
  if 'thing' is a function,
  'false' otherwise.

#### Modifiers

* 'check.not(value)':
...
```

#### <a name="apidoc.element.check-types.not.greater"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>greater ()](#apidoc.element.check-types.not.greater)
- description and source-code
```javascript
greater = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.not.greaterOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>greaterOrEqual ()](#apidoc.element.check-types.not.greaterOrEqual)
- description and source-code
```javascript
greaterOrEqual = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
...
```

#### <a name="apidoc.element.check-types.not.hasLength"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>hasLength ()](#apidoc.element.check-types.not.hasLength)
- description and source-code
```javascript
hasLength = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...

* 'check.assigned(thing)':
  Returns 'true'
  if 'thing' is not
  'null' or 'undefined',
  'false' otherwise.

* 'check.hasLength(thing, value)':
  Returns 'true'
  if 'thing' has a length property
  that equals 'value',
  'false' otherwise.

#### String predicates
...
```

#### <a name="apidoc.element.check-types.not.inRange"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>inRange ()](#apidoc.element.check-types.not.inRange)
- description and source-code
```javascript
inRange = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
between than 'a' and 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.inRange(thing, a, b)':
Returns 'true' if 'thing' is a number
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.
...
```

#### <a name="apidoc.element.check-types.not.includes"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>includes ()](#apidoc.element.check-types.not.includes)
- description and source-code
```javascript
includes = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' implements the iterable protocol,
  'false' otherwise.
  In pre-ES6 environments,
  this predicate falls back
  to 'arrayLike' behaviour.

* 'check.includes(thing, value)':
  Returns 'true'
  if 'thing' includes 'value',
  'false' otherwise.

#### Date predicates

* 'check.date(thing)':
...
```

#### <a name="apidoc.element.check-types.not.infinity"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>infinity ()](#apidoc.element.check-types.not.infinity)
- description and source-code
```javascript
infinity = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
'false' otherwise.

* 'check.greater(thing, value)':
Returns 'true' if 'thing' is a number
greater than 'value',
...
```

#### <a name="apidoc.element.check-types.not.instance"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>instance ()](#apidoc.element.check-types.not.instance)
- description and source-code
```javascript
instance = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.
Falls back to testing
'constructor.name' and 'Object.prototype.toString'
if the 'instanceof' test fails.
...
```

#### <a name="apidoc.element.check-types.not.instanceStrict"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>instanceStrict ()](#apidoc.element.check-types.not.instanceStrict)
- description and source-code
```javascript
instanceStrict = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
'false' otherwise.

* 'check.instance(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.not.integer"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>integer ()](#apidoc.element.check-types.not.integer)
- description and source-code
```javascript
integer = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
...
```

#### <a name="apidoc.element.check-types.not.iterable"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>iterable ()](#apidoc.element.check-types.not.iterable)
- description and source-code
```javascript
iterable = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
'false' otherwise.

* 'check.iterable(thing)':
Returns 'true'
if 'thing' implements the iterable protocol,
'false' otherwise.
In pre-ES6 environments,
this predicate falls back
to 'arrayLike' behaviour.
...
```

#### <a name="apidoc.element.check-types.not.less"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>less ()](#apidoc.element.check-types.not.less)
- description and source-code
```javascript
less = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.greaterOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
greater than or equal to 'value',
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
...
```

#### <a name="apidoc.element.check-types.not.lessOrEqual"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>lessOrEqual ()](#apidoc.element.check-types.not.lessOrEqual)
- description and source-code
```javascript
lessOrEqual = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.less(thing, value)':
Returns 'true' if 'thing' is a number
less than 'value',
'false' otherwise.

* 'check.lessOrEqual(thing, value)':
Returns 'true' if 'thing' is a number
less than or equal to 'value',
'false' otherwise.

* 'check.between(thing, a, b)':
Returns 'true' if 'thing' is a number
between than 'a' and 'b',
...
```

#### <a name="apidoc.element.check-types.not.like"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>like ()](#apidoc.element.check-types.not.like)
- description and source-code
```javascript
like = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
  Returns 'true'
  if 'thing' is an instance of 'prototype',
  'false' otherwise.
  Falls back to testing
  'constructor.name' and 'Object.prototype.toString'
  if the 'instanceof' test fails.

* 'check.like(thing, duck)':
  Duck-typing checker.
  Returns 'true'
  if 'thing' has all of the properties of 'duck',
  'false' otherwise.

#### Array predicates
...
```

#### <a name="apidoc.element.check-types.not.match"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>match ()](#apidoc.element.check-types.not.match)
- description and source-code
```javascript
match = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...

* 'check.contains(thing, substring)':
  Returns 'true'
  if 'thing' is a string
  that contains 'substring',
  'false' otherwise.

* 'check.match(thing, regex)':
  Returns 'true'
  if 'thing' is a string
  that matches 'regex',
  'false' otherwise.

#### Number predicates
...
```

#### <a name="apidoc.element.check-types.not.negative"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>negative ()](#apidoc.element.check-types.not.negative)
- description and source-code
```javascript
negative = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
...
```

#### <a name="apidoc.element.check-types.not.nonEmptyArray"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>nonEmptyArray ()](#apidoc.element.check-types.not.nonEmptyArray)
- description and source-code
```javascript
nonEmptyArray = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyArray(thing)':
Returns 'true'
if 'thing' is an empty array,
'false' otherwise.

* 'check.nonEmptyArray(thing)':
Returns 'true'
if 'thing' is a non-empty array,
'false' otherwise.

* 'check.arrayLike(thing)':
Returns 'true'
if 'thing' has a numeric length property,
...
```

#### <a name="apidoc.element.check-types.not.nonEmptyObject"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>nonEmptyObject ()](#apidoc.element.check-types.not.nonEmptyObject)
- description and source-code
```javascript
nonEmptyObject = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
'false' otherwise.

* 'check.nonEmptyObject(thing)':
Returns 'true'
if 'thing' is a non-empty object,
'false' otherwise.

* 'check.instanceStrict(thing, prototype)':
Returns 'true'
if 'thing' is an instance of 'prototype',
...
```

#### <a name="apidoc.element.check-types.not.nonEmptyString"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>nonEmptyString ()](#apidoc.element.check-types.not.nonEmptyString)
- description and source-code
```javascript
nonEmptyString = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
'false' otherwise.

* 'check.nonEmptyString(thing)':
Returns 'true'
if 'thing' is a non-empty string,
'false' otherwise.

* 'check.contains(thing, substring)':
Returns 'true'
if 'thing' is a string
...
```

#### <a name="apidoc.element.check-types.not.null"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>null ()](#apidoc.element.check-types.not.null)
- description and source-code
```javascript
null = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
#### General predicates

* 'check.equal(thing, thang)':
Returns 'true'
if 'thing === thang',
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
...
```

#### <a name="apidoc.element.check-types.not.number"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>number ()](#apidoc.element.check-types.not.number)
- description and source-code
```javascript
number = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' is a string
that matches 'regex',
'false' otherwise.

#### Number predicates

* 'check.number(thing)':
Returns 'true'
if 'thing' is a number,
'false' otherwise.
Note that
'NaN',
'Number.POSITIVE_INFINITY' and
'Number.NEGATIVE_INFINITY'
...
```

#### <a name="apidoc.element.check-types.not.object"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>object ()](#apidoc.element.check-types.not.object)
- description and source-code
```javascript
object = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
* 'check.boolean(thing)':
Returns 'true'
if 'thing' is a boolean,
'false' otherwise.

#### Object predicates

* 'check.object(thing)':
Returns 'true'
if 'thing' is a plain-old JavaScript object,
'false' otherwise.

* 'check.emptyObject(thing)':
Returns 'true'
if 'thing' is an empty object,
...
```

#### <a name="apidoc.element.check-types.not.odd"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>odd ()](#apidoc.element.check-types.not.odd)
- description and source-code
```javascript
odd = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
less than zero,
'false' otherwise.

* 'check.odd(thing)':
Returns 'true'
if 'thing' is an odd number,
'false' otherwise.

* 'check.even(thing)':
Returns 'true'
if 'thing' is an even number,
...
```

#### <a name="apidoc.element.check-types.not.positive"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>positive ()](#apidoc.element.check-types.not.positive)
- description and source-code
```javascript
positive = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
in the range 'a' .. 'b',
'false' otherwise.
The arguments 'a' and 'b'
may be in any order,
it doesn't matter
which is greater.

* 'check.positive(thing)':
Returns 'true' if 'thing' is a number
greater than zero,
'false' otherwise.

* 'check.negative(thing)':
Returns 'true'
if 'thing' is a number
...
```

#### <a name="apidoc.element.check-types.not.string"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>string ()](#apidoc.element.check-types.not.string)
- description and source-code
```javascript
string = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
Returns 'true'
if 'thing' has a length property
that equals 'value',
'false' otherwise.

#### String predicates

* 'check.string(thing)':
Returns 'true'
if 'thing' is a string,
'false' otherwise.

* 'check.emptyString(thing)':
Returns 'true'
if 'thing' is the empty string,
...
```

#### <a name="apidoc.element.check-types.not.undefined"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>undefined ()](#apidoc.element.check-types.not.undefined)
- description and source-code
```javascript
undefined = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
'false' otherwise.

* 'check.null(thing)':
Returns 'true'
if 'thing' is 'null',
'false' otherwise.

* 'check.undefined(thing)':
Returns 'true'
if 'thing' is 'undefined',
'false' otherwise.

* 'check.assigned(thing)':
Returns 'true'
if 'thing' is not
...
```

#### <a name="apidoc.element.check-types.not.zero"></a>[function <span class="apidocSignatureSpan">check-types.not.</span>zero ()](#apidoc.element.check-types.not.zero)
- description and source-code
```javascript
zero = function () {
  return notImpl(predicate.apply(null, arguments));
}
```
- example usage
```shell
...
are not considered numbers here.

* 'check.integer(thing)':
Returns 'true'
if 'thing' is an integer,
'false' otherwise.

* 'check.zero(thing)':
Returns 'true'
if 'thing' is zero,
'false' otherwise.

* 'check.infinity(thing)':
Returns 'true'
if 'thing' is positive or negative infinity,
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
