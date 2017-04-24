# npmtest-sweet-scroll

#### basic test coverage for  [sweet-scroll (v2.2.0)](https://github.com/tsuyoshiwada/sweet-scroll)  [![npm package](https://img.shields.io/npm/v/npmtest-sweet-scroll.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-sweet-scroll) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-sweet-scroll.svg)](https://travis-ci.org/npmtest/node-npmtest-sweet-scroll)

#### Modern and the sweet smooth scroll library.

[![NPM](https://nodei.co/npm/sweet-scroll.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/sweet-scroll)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-sweet-scroll/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-sweet-scroll/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-sweet-scroll/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-sweet-scroll/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-sweet-scroll/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-sweet-scroll/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-sweet-scroll/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-sweet-scroll/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-sweet-scroll/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-sweet-scroll/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-sweet-scroll/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-sweet-scroll/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-sweet-scroll/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-sweet-scroll/build/test-report.html](https://npmtest.github.io/node-npmtest-sweet-scroll/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-sweet-scroll/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-sweet-scroll/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-sweet-scroll/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-sweet-scroll/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sweet-scroll/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sweet-scroll/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-sweet-scroll/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-sweet-scroll/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "tsuyoshiwada"
    },
    "bugs": {
        "url": "https://github.com/tsuyoshiwada/sweet-scroll/issues"
    },
    "dependencies": {},
    "description": "Modern and the sweet smooth scroll library.",
    "devDependencies": {
        "autoprefixer": "^6.5.3",
        "babel-eslint": "^7.1.0",
        "babel-plugin-espower": "^2.3.1",
        "babel-plugin-external-helpers": "^6.18.0",
        "babel-preset-es2015": "^6.18.0",
        "babel-preset-stage-0": "^6.16.0",
        "babelify": "^7.3.0",
        "browser-sync": "^2.17.5",
        "browserify": "^13.1.1",
        "copyfiles": "^1.0.0",
        "eslint": "^3.9.1",
        "karma": "^1.3.0",
        "karma-browserify": "^5.1.0",
        "karma-cli": "^1.0.1",
        "karma-fixture": "^0.2.6",
        "karma-html2js-preprocessor": "^1.1.0",
        "karma-mocha": "^1.3.0",
        "karma-phantomjs-launcher": "^1.0.2",
        "karma-phantomjs-shim": "^1.4.0",
        "mocha": "^3.1.2",
        "node-sass": "^3.11.2",
        "npm-run-all": "^3.1.1",
        "onchange": "^3.0.2",
        "phantomjs-prebuilt": "^2.1.13",
        "postcss-cli": "^2.6.0",
        "power-assert": "^1.4.2",
        "rollup": "^0.36.3",
        "rollup-plugin-babel": "^2.6.1",
        "sinon": "^1.17.6",
        "uglify-js": "^2.7.4",
        "watchify": "^3.7.0"
    },
    "directories": {},
    "dist": {
        "shasum": "5085d6cab3317702b6f9a6c6a0ce9e9faf256982",
        "tarball": "https://registry.npmjs.org/sweet-scroll/-/sweet-scroll-2.2.0.tgz"
    },
    "files": [
        "src",
        "test",
        "sweet-scroll.js",
        "sweet-scroll.min.js"
    ],
    "gitHead": "8ec93da4d7a0e13090e8f80da1ab25efe1868b8b",
    "homepage": "https://github.com/tsuyoshiwada/sweet-scroll",
    "keywords": [
        "smooth scroll",
        "scroll",
        "animation"
    ],
    "license": "MIT",
    "main": "sweet-scroll.js",
    "maintainers": [
        {
            "name": "tsuyoshiwada"
        }
    ],
    "name": "sweet-scroll",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tsuyoshiwada/sweet-scroll.git"
    },
    "scripts": {
        "build": "npm-run-all build:* docs:build",
        "build:js": "NODE_ENV=production rollup -c rollup.config.js && uglifyjs --compress --mangle -o sweet-scroll.min.js --comments -- sweet-scroll.js",
        "docs": "npm-run-all --parallel docs:watch:*",
        "docs:build": "npm run docs:build:js && npm run docs:build:sass",
        "docs:build:js": "copyfiles sweet-scroll.js docs/js/",
        "docs:build:sass": "node-sass docs/sass/ -o docs/css/ --output-style compressed && postcss --use autoprefixer docs/css/*.css -d docs/css/",
        "docs:watch:js": "onchange 'sweet-scroll.js' -- npm run docs:build:js",
        "docs:watch:sass": "onchange 'docs/sass/**/*.scss' -- npm run docs:build:sass",
        "docs:watch:server": "browser-sync start -s 'docs/' -f 'docs/**/*,!docs/sass/**/*' --no-notify --no-open --no-ghost-mode",
        "karma": "NODE_ENV=test karma start karma.conf.js --single-run",
        "lint": "eslint src/**/*.js test/**/*.js .eslintrc.js --no-ignore",
        "start": "npm-run-all --parallel watch docs",
        "test": "npm-run-all lint karma",
        "watch": "npm-run-all --parallel watch:*",
        "watch:js": "onchange 'src/**/*.js' -- npm run build:js",
        "watch:test": "onchange 'test/**/*.js' -- npm run karma"
    },
    "version": "2.2.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
