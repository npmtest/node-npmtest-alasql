# npmtest-alasql

#### basic test coverage for  [alasql (v0.3.9)](https://github.com/agershun/alasql)  [![npm package](https://img.shields.io/npm/v/npmtest-alasql.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-alasql) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-alasql.svg)](https://travis-ci.org/npmtest/node-npmtest-alasql)

#### Versatile SQL database for browser or node. Handles relational data and nested JSON (noSQL). Export to and import from Excel, localStorage or IndexedDB

[![NPM](https://nodei.co/npm/alasql.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/alasql)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-alasql/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-alasql/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-alasql/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-alasql/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-alasql/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-alasql/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-alasql/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-alasql/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-alasql/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-alasql/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-alasql/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-alasql/build/test-report.html](https://npmtest.github.io/node-npmtest-alasql/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-alasql/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-alasql/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-alasql/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-alasql/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-alasql/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-alasql/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-alasql/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-alasql/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andrey Gershun"
    },
    "bin": {
        "alasql": "./bin/alasql-cli.js",
        "alaserver": "./bin/alaserver.js"
    },
    "bugs": {
        "url": "https://github.com/agershun/alasql/issues"
    },
    "contributors": [
        {
            "name": "Mathias Rangel Wulff"
        }
    ],
    "dependencies": {
        "dom-storage": "^2.0.1",
        "es6-promise": "^4.0.5",
        "lodash": "^4.17.4",
        "request": "^2.79.0",
        "xlsx": "^0.9.2",
        "yargs": "^5.0.0"
    },
    "description": "Versatile SQL database for browser or node. Handles relational data and nested JSON (noSQL). Export to and import from Excel, localStorage or IndexedDB",
    "devDependencies": {
        "blueimp-md5": "^2.7.0",
        "gulp": "^3.9.1",
        "gulp-concat": "^2.6.1",
        "gulp-dereserve": "^0.2.1",
        "gulp-exec": "^2.1.3",
        "gulp-jison": "^1.2.0",
        "gulp-rename": "^1.2.2",
        "gulp-replace": "^0.5.4",
        "gulp-shell": "^0.5.2",
        "gulp-uglify": "^2.0.1",
        "istanbul": "^0.4.5",
        "jison": "^0.4.17",
        "mocha": "^3.2.0",
        "mocha.parallel": "^0.15.0",
        "mversion": "^1.10.1",
        "npm-check": "^5.2.3",
        "open": "0.0.5",
        "strftime": "^0.10.0",
        "uglify-js": "^2.7.5"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "c407b8cb5ed018cd8c2d882f4386492ae1420908",
        "tarball": "https://registry.npmjs.org/alasql/-/alasql-0.3.9.tgz"
    },
    "engines": [
        "node"
    ],
    "gitHead": "65746661adabca0af5c4deb8572205d5236c616c",
    "homepage": "https://github.com/agershun/alasql",
    "keywords": [
        "sql",
        "nosql",
        "graph",
        "alasql",
        "javascript",
        "parser",
        "database",
        "DBMS",
        "data",
        "query",
        "localStorage",
        "IndexedDB",
        "DOM-storage",
        "SQLite",
        "JSON",
        "Excel",
        "XLSX",
        "XLS",
        "CSV",
        "worker"
    ],
    "license": "MIT",
    "main": "dist/alasql.fs.js",
    "maintainers": [
        {
            "name": "agershun"
        },
        {
            "name": "mathiasrw"
        }
    ],
    "name": "alasql",
    "optionalDependencies": {},
    "preferGlobal": true,
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/agershun/alasql.git"
    },
    "scripts": {
        "build": "gulp",
        "build:jison": "gulp --jison && gulp",
        "build:watch": "gulp watch",
        "bump": "mversion --no-prefix",
        "jison": "jison ./src/alasqlparser.jison -o ./src/alasqlparser.js",
        "release": "f='/TMP/alasql.tmp' && curl https://raw.githubusercontent.com/wiki/agershun/alasql/How-to-release.md > $f && sh $f ; rm $f",
        "test": "gulp && cd test && mocha . --reporter dot",
        "test:browser": "node test/browserTestRunner.js 7387",
        "test:cover": "istanbul cover  -x 'lib/zt/zt.js' --dir test/coverage _mocha",
        "test:only": "cd test && mocha . --reporter dot",
        "test:this": "gulp && cd test && mocha",
        "uptodate": "npm-check -u --skip-unused"
    },
    "testling": {
        "browsers": [
            "ie/6..latest",
            "chrome/22..latest",
            "firefox/16..latest",
            "safari/latest",
            "opera/11.0..latest",
            "iphone/4..latest",
            "ipad/4..latest",
            "android-browser/4..latest"
        ]
    },
    "typings": "./dist/alasql.d.ts",
    "version": "0.3.9"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
