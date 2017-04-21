# npmdoc-rollup-plugin-buble

#### api documentation for  rollup-plugin-buble (v0.15.0)  [![npm package](https://img.shields.io/npm/v/npmdoc-rollup-plugin-buble.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rollup-plugin-buble) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rollup-plugin-buble.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rollup-plugin-buble)

#### Compile ES2015 with buble

[![NPM](https://nodei.co/npm/rollup-plugin-buble.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/rollup-plugin-buble)

- [https://npmdoc.github.io/node-npmdoc-rollup-plugin-buble/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-rollup-plugin-buble/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rollup-plugin-buble/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rollup-plugin-buble/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rollup-plugin-buble/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rollup-plugin-buble/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "rollup-plugin-buble",
    "description": "Compile ES2015 with buble",
    "version": "0.15.0",
    "author": "Rich Harris",
    "repository": "https://gitlab.com/rich-harris/rollup-plugin-buble",
    "license": "MIT",
    "main": "dist/rollup-plugin-buble.cjs.js",
    "jsnext:main": "dist/rollup-plugin-buble.es.js",
    "scripts": {
        "build": "npm run build:cjs && npm run build:es",
        "build:cjs": "rollup -c -f cjs -o dist/rollup-plugin-buble.cjs.js",
        "build:es": "rollup -c -f es6 -o dist/rollup-plugin-buble.es.js",
        "test": "mocha test/test.js",
        "pretest": "npm run build:cjs",
        "prepublish": "npm run lint && rm -rf dist && npm test && npm run build:es",
        "lint": "eslint src"
    },
    "files": [
        "dist",
        "README.md"
    ],
    "devDependencies": {
        "eslint": "^3.3.1",
        "mocha": "^3.0.2",
        "rollup": "^0.37.0"
    },
    "dependencies": {
        "buble": "^0.15.0",
        "rollup-pluginutils": "^1.5.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
