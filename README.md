# npmtest-koa-better-body

#### basic test coverage for  koa-better-body (v3.0.2)  [![npm package](https://img.shields.io/npm/v/npmtest-koa-better-body.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-koa-better-body) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-koa-better-body.svg)](https://travis-ci.org/npmtest/node-npmtest-koa-better-body)

#### Full-featured [koa][] body parser! Support parsing text, buffer, json, json patch, json api, csp-report, multipart, form and urlencoded bodies. Works for koa@1, koa@2 and will work for koa@3.

[![NPM](https://nodei.co/npm/koa-better-body.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/koa-better-body)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-koa-better-body/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-koa-better-body/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-koa-better-body/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-koa-better-body/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-koa-better-body/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-koa-better-body/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-koa-better-body/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-koa-better-body/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-koa-better-body/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-koa-better-body/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-koa-better-body/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-koa-better-body/build/test-report.html](https://npmtest.github.io/node-npmtest-koa-better-body/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-koa-better-body/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-koa-better-body/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-koa-better-body/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-koa-better-body/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-koa-better-body/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-koa-better-body/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-koa-better-body/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-koa-better-body/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "koa-better-body",
    "version": "3.0.2",
    "description": "Full-featured [koa][] body parser! Support parsing text, buffer, json, json patch, json api, csp-report, multipart, form and urlencoded bodies. Works for koa@1, koa@2 and will work for koa@3.",
    "repository": "tunnckoCore/koa-better-body",
    "author": "Charlike Mike Reagent <@tunnckoCore> (http://www.tunnckocore.tk)",
    "main": "index.js",
    "license": "MIT",
    "scripts": {
        "lint": "standard --verbose",
        "pretest": "npm run lint",
        "test": "npm run coverage",
        "posttest": "npm run lint:coverage",
        "coverage": "nyc node test.js",
        "lint:coverage": "nyc check-coverage --lines 100 --branches 85 --statements 100 --functions 90",
        "report-coverage": "nyc report --reporter=text-lcov | coveralls",
        "prerelease": "npm test",
        "release": "standard-version --sign --no-verify",
        "precommit": "git add --all",
        "commit": "git-cz"
    },
    "dependencies": {
        "extend-shallow": "^2.0.1",
        "formidable": "^1.0.17",
        "koa-body-parsers": "git+https://github.com/tunnckoCore/body-parsers.git",
        "lazy-cache": "^2.0.1"
    },
    "devDependencies": {
        "commitizen": "^2.8.6",
        "coveralls": "^2.11.12",
        "cz-conventional-changelog": "^1.2.0",
        "is-buffer": "^1.1.3",
        "koa": "^1.2.4",
        "koa-route": "^2.4.2",
        "mukla": "^0.4.1",
        "nyc": "^8.1.0",
        "qs": "^6.2.1",
        "pre-commit": "^1.1.3",
        "standard": "^8.0.0",
        "standard-version": "^2.4.0",
        "supertest": "^2.0.0"
    },
    "files": [
        "index.js",
        "utils.js"
    ],
    "keywords": [
        "api",
        "awesome",
        "better",
        "body",
        "body-parser",
        "buffer",
        "csp",
        "csp-report",
        "error",
        "error-handling",
        "extendable",
        "feature",
        "features",
        "flexible",
        "form",
        "forms",
        "full",
        "full-feature",
        "handling",
        "json",
        "json-api",
        "json-patch",
        "json-strict",
        "jsonstrict",
        "koa",
        "koa-better-body",
        "multipart",
        "parse",
        "parser",
        "patch",
        "report",
        "rfc",
        "standard",
        "strict",
        "text",
        "unopinionated",
        "urlencoded"
    ],
    "verb": {
        "run": true,
        "toc": false,
        "layout": "empty",
        "tasks": [
            "readme"
        ],
        "related": {
            "list": [
                "koa",
                "koa-ip-filter",
                "ip-filter",
                "formidable",
                "koa-body-parsers",
                "koa-bodyparser",
                "koala"
            ]
        },
        "reflinks": [
            "bytes",
            "formidable",
            "koa",
            "koa-body-parsers",
            "koa-convert",
            "lazy-cache",
            "raw-body",
            "koa-router",
            "micromatch",
            "qs"
        ],
        "lint": {
            "reflinks": true
        }
    },
    "config": {
        "commitizen": {
            "path": "./node_modules/cz-conventional-changelog"
        }
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
