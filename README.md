# npmdoc-protocol-buffers

#### api documentation for  [protocol-buffers (v3.2.1)](https://github.com/mafintosh/protocol-buffers)  [![npm package](https://img.shields.io/npm/v/npmdoc-protocol-buffers.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-protocol-buffers) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-protocol-buffers.svg)](https://travis-ci.org/npmdoc/node-npmdoc-protocol-buffers)

#### Protocol Buffers for Node.js

[![NPM](https://nodei.co/npm/protocol-buffers.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/protocol-buffers)

- [https://npmdoc.github.io/node-npmdoc-protocol-buffers/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-protocol-buffers/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-protocol-buffers/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-protocol-buffers/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-protocol-buffers/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-protocol-buffers/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mathias Buus"
    },
    "browserify": {
        "transform": [
            "brfs"
        ]
    },
    "bugs": {
        "url": "https://github.com/mafintosh/protocol-buffers/issues"
    },
    "dependencies": {
        "brfs": "^1.4.0",
        "generate-function": "^2.0.0",
        "generate-object-property": "^1.2.0",
        "protocol-buffers-schema": "^3.1.1",
        "signed-varint": "^2.0.0",
        "varint": "^5.0.0"
    },
    "description": "Protocol Buffers for Node.js",
    "devDependencies": {
        "standard": "^5.4.1",
        "tape": "^3.0.3"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "37258e17e24a082f06ebb17731e92851d1c76889",
        "tarball": "https://registry.npmjs.org/protocol-buffers/-/protocol-buffers-3.2.1.tgz"
    },
    "gitHead": "1583634bda4b04a9a101ec5aace1953f3788449b",
    "homepage": "https://github.com/mafintosh/protocol-buffers",
    "keywords": [
        "protobuf",
        "protocol",
        "buffers",
        "protocolbuffers",
        "encode",
        "decode",
        "google",
        "serialize",
        "parse",
        "levelup",
        "encodings",
        "encoding"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mafintosh"
        }
    ],
    "name": "protocol-buffers",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mafintosh/protocol-buffers.git"
    },
    "scripts": {
        "bench": "node bench",
        "test": "standard && tape test/*.js"
    },
    "version": "3.2.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
