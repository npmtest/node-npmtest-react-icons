# npmtest-react-icons

#### basic test coverage for  [react-icons (v2.2.3)](https://github.com/gorangajic/react-icons#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-react-icons.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-icons) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-icons.svg)](https://travis-ci.org/npmtest/node-npmtest-react-icons)

#### svg react icons of popular icon packs using ES6 imports

[![NPM](https://nodei.co/npm/react-icons.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-icons)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-icons/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-icons/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-icons/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-icons/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-icons/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-icons/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-icons/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-icons/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-icons/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-icons/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-icons/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-icons/build/test-report.html](https://npmtest.github.io/node-npmtest-react-icons/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-icons/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-icons/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-icons/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-icons/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-icons/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-icons/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-icons/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-icons/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Goran Gajic"
    },
    "bugs": {
        "url": "https://github.com/gorangajic/react-icons/issues"
    },
    "config": {
        "ghooks": {
            "commit-msg": "validate-commit-msg"
        },
        "commitizen": {
            "path": "./node_modules/cz-conventional-changelog"
        },
        "validate-commit-msg": {
            "types": [
                "issue",
                "master",
                "revert"
            ],
            "warnOnFail": false,
            "maxSubjectLength": 100,
            "subjectPattern": ".+",
            "subjectPatternErrorMsg": "subject does not match subject pattern!",
            "helpMessage": ""
        }
    },
    "dependencies": {
        "react-icon-base": "2.0.4"
    },
    "description": "svg react icons of popular icon packs using ES6 imports",
    "devDependencies": {
        "babel": "6.5.2",
        "babel-cli": "6.7.5",
        "babel-eslint": "^5.0.0-beta6",
        "babel-plugin-add-module-exports": "0.1.2",
        "babel-preset-es2015": "6.6.0",
        "babel-preset-react": "6.5.0",
        "babel-preset-stage-0": "6.5.0",
        "camelcase": "^2.0.1",
        "capitalize": "^1.0.0",
        "cheerio": "^0.19.0",
        "classnames": "^2.2.3",
        "commitizen": "^2.8.2",
        "cz-conventional-changelog": "^1.1.6",
        "decamelize": "1.1.2",
        "eslint": "^1.10.3",
        "eslint-config-airbnb": "^3.1.0",
        "eslint-plugin-react": "^3.15.0",
        "ghooks": "^1.3.2",
        "glob": "^6.0.4",
        "gulp": "^3.9.0",
        "marky-markdown": "git+https://github.com/npm/marky-markdown.git",
        "material-design-lite": "^1.0.6",
        "svg-scaler": "github:gorangajic/svg-scaler#take-size-viewbox",
        "underscore": "^1.8.3",
        "validate-commit-msg": "^2.6.1"
    },
    "directories": {},
    "dist": {
        "shasum": "3b4847923065ecb09f8ba7f7e422112de0195196",
        "tarball": "https://registry.npmjs.org/react-icons/-/react-icons-2.2.3.tgz"
    },
    "gitHead": "396b4d9241a61b6d22f3907273158b6a91aea2fd",
    "homepage": "https://github.com/gorangajic/react-icons#readme",
    "keywords": [
        "react",
        "icons",
        "inline",
        "svg",
        "font",
        "awesome",
        "material",
        "design"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "feroc1ty"
        }
    ],
    "name": "react-icons",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0",
        "react-dom": "^0.14.0 || ^15.0.0"
    },
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/gorangajic/react-icons.git"
    },
    "scripts": {
        "build": "node ./bin/create | xargs babel --out-dir lib",
        "docs": "babel-node ./bin/generate-docs",
        "eslint": "eslint .",
        "prepublish": "npm run build"
    },
    "version": "2.2.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
