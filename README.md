# npmdoc-basscss

#### api documentation for  [basscss (v8.0.3)](https://github.com/basscss/basscss)  [![npm package](https://img.shields.io/npm/v/npmdoc-basscss.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-basscss) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-basscss.svg)](https://travis-ci.org/npmdoc/node-npmdoc-basscss)

#### Low-level CSS toolkit

[![NPM](https://nodei.co/npm/basscss.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/basscss)

- [https://npmdoc.github.io/node-npmdoc-basscss/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-basscss/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-basscss/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-basscss/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-basscss/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-basscss/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "basscss",
    "version": "8.0.3",
    "description": "Low-level CSS toolkit",
    "style": "src/basscss.css",
    "scripts": {
        "build": "postcss -c postcss.config.js",
        "minify": "postcss -u cssnano css/basscss.css -o css/basscss.min.css",
        "important": "postcss -u postcss-importantly css/basscss.css -o css/basscss-important.css",
        "important:min": "postcss -u postcss-importantly -u cssnano css/basscss.css -o css/basscss-important.min.css",
        "custom-props": "postcss -u postcss-import -u postcss-custom-media src/basscss.css -o css/basscss-cp.css",
        "custom-props:min": "postcss -u postcss-import -u postcss-custom-media -u cssnano src/basscss.css -o css/basscss-cp.min.css",
        "prepublish": "mkdir -p css && npm run build && npm run important && npm run custom-props && npm run minify && npm run important:min && npm run custom-props:min",
        "start": "postcss -c postcss.config.js -w",
        "karma": "karma start",
        "karma:watch": "karma start --no-single-run",
        "mocha": "mocha test/test",
        "test": "npm run mocha && npm run karma"
    },
    "dependencies": {
        "basscss-align": "^1.0.2",
        "basscss-border": "^4.0.2",
        "basscss-flexbox": "^1.0.1",
        "basscss-grid": "^2.0.0",
        "basscss-hide": "^1.0.1",
        "basscss-layout": "^3.1.0",
        "basscss-margin": "^1.0.7",
        "basscss-padding": "^1.1.3",
        "basscss-position": "^2.0.3",
        "basscss-type-scale": "^1.0.5",
        "basscss-typography": "^3.0.3"
    },
    "devDependencies": {
        "autoprefixer": "^6.1.2",
        "babel": "^6.3.26",
        "babel-core": "^6.4.5",
        "babel-loader": "^6.2.1",
        "babel-preset-es2015": "^6.3.13",
        "chai": "^3.5.0",
        "css-loader": "^0.23.1",
        "css-mixed-properties": "^1.1.0",
        "cssnano": "^3.4.0",
        "cssstats": "^2.1.2",
        "json-loader": "^0.5.4",
        "karma": "^0.13.19",
        "karma-chai": "^0.1.0",
        "karma-chai-plugins": "^0.6.1",
        "karma-cli": "^0.1.2",
        "karma-firefox-launcher": "^0.1.7",
        "karma-mocha": "^0.2.1",
        "karma-mocha-reporter": "^1.1.5",
        "karma-webpack": "^1.7.0",
        "mocha": "^2.2.1",
        "postcss": "^5.0.14",
        "postcss-calc": "^5.2.0",
        "postcss-cli": "^2.5.0",
        "postcss-color-function": "^2.0.0",
        "postcss-custom-media": "^5.0.0",
        "postcss-custom-properties": "^5.0.0",
        "postcss-discard-comments": "^1.1.1",
        "postcss-import": "^7.1.3",
        "postcss-importantly": "0.0.7",
        "postcss-loader": "^0.8.0",
        "postcss-remove-root": "0.0.2",
        "postcss-reporter": "^1.3.0",
        "style-loader": "^0.13.0",
        "webpack": "^1.12.12"
    },
    "author": "Brent Jackson",
    "license": "MIT",
    "keywords": [
        "atomic css",
        "functional css",
        "css",
        "framework",
        "oocss",
        "basscss"
    ],
    "repository": {
        "type": "git",
        "url": "https://github.com/basscss/basscss.git"
    },
    "bugs": {
        "url": "https://github.com/basscss/basscss/issues"
    },
    "homepage": "https://github.com/basscss/basscss",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
