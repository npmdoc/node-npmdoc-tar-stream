# npmdoc-tar-stream

#### api documentation for  [tar-stream (v1.5.2)](https://github.com/mafintosh/tar-stream)  [![npm package](https://img.shields.io/npm/v/npmdoc-tar-stream.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tar-stream) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tar-stream.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tar-stream)

#### tar-stream is a streaming tar parser and generator and nothing else. It is streams2 and operates purely using streams which means you can easily extract/parse tarballs without ever hitting the file system.

[![NPM](https://nodei.co/npm/tar-stream.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/tar-stream)

- [https://npmdoc.github.io/node-npmdoc-tar-stream/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-tar-stream/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tar-stream/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tar-stream/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tar-stream/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tar-stream/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mathias Buus"
    },
    "bugs": {
        "url": "https://github.com/mafintosh/tar-stream/issues"
    },
    "dependencies": {
        "bl": "^1.0.0",
        "end-of-stream": "^1.0.0",
        "readable-stream": "^2.0.0",
        "xtend": "^4.0.0"
    },
    "description": "tar-stream is a streaming tar parser and generator and nothing else. It is streams2 and operates purely using streams which means you can easily extract/parse tarballs without ever hitting the file system.",
    "devDependencies": {
        "concat-stream": "^1.4.6",
        "standard": "^5.3.1",
        "tape": "^3.0.3"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "fbc6c6e83c1a19d4cb48c7d96171fc248effc7bf",
        "tarball": "https://registry.npmjs.org/tar-stream/-/tar-stream-1.5.2.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "files": [
        "*.js",
        "LICENSE"
    ],
    "gitHead": "7c279d66989a3bdde45f1eb661edaa846540d984",
    "homepage": "https://github.com/mafintosh/tar-stream",
    "keywords": [
        "tar",
        "tarball",
        "parse",
        "parser",
        "generate",
        "generator",
        "stream",
        "stream2",
        "streams",
        "streams2",
        "streaming",
        "pack",
        "extract",
        "modify"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mafintosh"
        },
        {
            "name": "maxogden"
        }
    ],
    "name": "tar-stream",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mafintosh/tar-stream.git"
    },
    "scripts": {
        "test": "standard && tape test/*.js"
    },
    "version": "1.5.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
