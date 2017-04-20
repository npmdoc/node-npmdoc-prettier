# npmdoc-prettier

#### api documentation for  prettier (v1.2.2)  [![npm package](https://img.shields.io/npm/v/npmdoc-prettier.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-prettier) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-prettier.svg)](https://travis-ci.org/npmdoc/node-npmdoc-prettier)

#### Prettier is an opinionated JavaScript formatter

[![NPM](https://nodei.co/npm/prettier.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/prettier)

- [https://npmdoc.github.io/node-npmdoc-prettier/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-prettier/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-prettier/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-prettier/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-prettier/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-prettier/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "prettier",
    "version": "1.2.2",
    "description": "Prettier is an opinionated JavaScript formatter",
    "bin": {
        "prettier": "./bin/prettier.js"
    },
    "repository": "prettier/prettier",
    "author": "James Long",
    "license": "MIT",
    "main": "./index.js",
    "dependencies": {
        "ast-types": "0.9.8",
        "babel-code-frame": "6.22.0",
        "babylon": "7.0.0-beta.8",
        "chalk": "1.1.3",
        "esutils": "2.0.2",
        "flow-parser": "0.43.0",
        "get-stdin": "5.0.1",
        "glob": "7.1.1",
        "jest-validate": "19.0.0",
        "minimist": "1.2.0"
    },
    "devDependencies": {
        "diff": "3.2.0",
        "jest": "19.0.1",
        "mkdirp": "^0.5.1",
        "rimraf": "^2.6.1",
        "rollup": "0.41.1",
        "rollup-plugin-commonjs": "7.0.0",
        "rollup-plugin-json": "2.1.0",
        "rollup-plugin-node-builtins": "2.0.0",
        "rollup-plugin-node-globals": "1.1.0",
        "rollup-plugin-node-resolve": "2.0.0",
        "typescript": "2.2.1",
        "typescript-eslint-parser": "git://github.com/eslint/typescript-eslint-parser.git#bfb1506c48b625871ffeb67dbec7941d460f8941"
    },
    "scripts": {
        "test": "jest",
        "format": "./bin/prettier.js --write",
        "format:single": "npm run format -- src/printer.js",
        "format:all": "npm run format -- index.js src/*.js bin/*.js",
        "build:docs": "rollup -c docs/rollup.config.js"
    },
    "jest": {
        "setupFiles": [
            "<rootDir>/tests_config/run_spec.js"
        ],
        "snapshotSerializers": [
            "<rootDir>/tests_config/raw-serializer.js"
        ],
        "testRegex": "jsfmt\\.spec\\.js$",
        "testPathIgnorePatterns": [
            "tests/new_react",
            "tests/more_react"
        ]
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
