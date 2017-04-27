# npmdoc-fantasy-land

#### basic api documentation for  [fantasy-land (v3.2.0)](https://github.com/fantasyland/fantasy-land)  [![npm package](https://img.shields.io/npm/v/npmdoc-fantasy-land.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fantasy-land) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fantasy-land.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fantasy-land)

#### Specification for interoperability of common algebraic structures in JavaScript

[![NPM](https://nodei.co/npm/fantasy-land.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/fantasy-land)

- [https://npmdoc.github.io/node-npmdoc-fantasy-land/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fantasy-land/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brian McKenna"
    },
    "bugs": {
        "url": "https://github.com/fantasyland/fantasy-land/issues"
    },
    "dependencies": {
        "daggy": "0.0.x",
        "fantasy-combinators": "0.0.x"
    },
    "description": "Specification for interoperability of common algebraic structures in JavaScript",
    "devDependencies": {
        "eslint": "3.8.x",
        "nodeunit": "0.9.x",
        "sanctuary-style": "0.2.x",
        "xyz": "2.0.x"
    },
    "directories": {},
    "dist": {
        "shasum": "cf9ee50bd96fc1c1562556f9c0363f5ec0ca2cd2",
        "tarball": "https://registry.npmjs.org/fantasy-land/-/fantasy-land-3.2.0.tgz"
    },
    "files": [
        "index.js",
        "internal/*.js",
        "laws/*.js"
    ],
    "gitHead": "a5d90e8520b448835df3cd2f932284353a3f06e6",
    "homepage": "https://github.com/fantasyland/fantasy-land",
    "issues": {
        "url": "https://github.com/fantasyland/fantasy-land/issues"
    },
    "keywords": [
        "algebraic",
        "monad",
        "applicative",
        "functor",
        "monoid",
        "semigroup",
        "chain",
        "apply"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "davidchambers"
        },
        {
            "name": "joneshf"
        },
        {
            "name": "kennknowles"
        },
        {
            "name": "laiff"
        },
        {
            "name": "puffnfresh"
        },
        {
            "name": "stickupkid"
        }
    ],
    "name": "fantasy-land",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/fantasyland/fantasy-land.git"
    },
    "scripts": {
        "lint": "eslint --config node_modules/sanctuary-style/eslint-es6.json --env es6 --env node --rule 'max-len: [off]' -- *.js laws/*.js internal/*.js",
        "release-major": "xyz --repo git@github.com:fantasyland/fantasy-land.git --increment major",
        "release-minor": "xyz --repo git@github.com:fantasyland/fantasy-land.git --increment minor",
        "release-patch": "xyz --repo git@github.com:fantasyland/fantasy-land.git --increment patch",
        "test": "npm run-script lint && npm run-script unit",
        "unit": "nodeunit test.js"
    },
    "version": "3.2.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
