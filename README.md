# api documentation for  [protocol-buffers (v3.2.1)](https://github.com/mafintosh/protocol-buffers)  [![npm package](https://img.shields.io/npm/v/npmdoc-protocol-buffers.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-protocol-buffers) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-protocol-buffers.svg)](https://travis-ci.org/npmdoc/node-npmdoc-protocol-buffers)
#### Protocol Buffers for Node.js

[![NPM](https://nodei.co/npm/protocol-buffers.png?downloads=true)](https://www.npmjs.com/package/protocol-buffers)

[![apidoc](https://npmdoc.github.io/node-npmdoc-protocol-buffers/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-protocol-buffers_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-protocol-buffers/build/apidoc.html)

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
            "name": "mafintosh",
            "email": "mathiasbuus@gmail.com"
        }
    ],
    "name": "protocol-buffers",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module protocol-buffers](#apidoc.module.protocol-buffers)
1.  object <span class="apidocSignatureSpan">protocol-buffers.</span>encodings

#### [module protocol-buffers.encodings](#apidoc.module.protocol-buffers.encodings)
1.  [function <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>make (type, encode, decode, encodingLength)](#apidoc.element.protocol-buffers.encodings.make)
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>bool
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>bytes
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>double
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>enum
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>fixed32
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>fixed64
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>float
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>int32
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>int64
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>sfixed32
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>sfixed64
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>sint32
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>sint64
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>string
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>uint32
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>uint64
1.  object <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>varint



# <a name="apidoc.module.protocol-buffers"></a>[module protocol-buffers](#apidoc.module.protocol-buffers)



# <a name="apidoc.module.protocol-buffers.encodings"></a>[module protocol-buffers.encodings](#apidoc.module.protocol-buffers.encodings)

#### <a name="apidoc.element.protocol-buffers.encodings.make"></a>[function <span class="apidocSignatureSpan">protocol-buffers.encodings.</span>make (type, encode, decode, encodingLength)](#apidoc.element.protocol-buffers.encodings.make)
- description and source-code
```javascript
make = function (type, encode, decode, encodingLength) {
  encode.bytes = decode.bytes = 0

  return {
    type: type,
    encode: encode,
    decode: decode,
    encodingLength: encodingLength
  }
}
```
- example usage
```shell
...
      ('decode.bytes = varint.decode.bytes')
      ('return val')
    ('}')
    .toFunction({
      varint: varint
    })

  return encodings.make(0, encode, decode, varint.encodingLength)
}

var compileMessage = function (m, exports) {
  m.messages.forEach(function (nested) {
    exports[nested.name] = resolve(nested.name, m.id)
  })
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
