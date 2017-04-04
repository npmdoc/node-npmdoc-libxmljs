# api documentation for  [libxmljs (v0.18.4)](https://github.com/libxmljs/libxmljs)  [![npm package](https://img.shields.io/npm/v/npmdoc-libxmljs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-libxmljs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-libxmljs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-libxmljs)
#### libxml bindings for v8 javascript engine

[![NPM](https://nodei.co/npm/libxmljs.png?downloads=true)](https://www.npmjs.com/package/libxmljs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-libxmljs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-libxmljs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-libxmljs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-libxmljs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-libxmljs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Marco Rogers"
    },
    "binary": {
        "module_name": "xmljs",
        "module_path": "./build/Release/",
        "host": "https://github.com",
        "remote_path": "./libxmljs/libxmljs/releases/download/v{version}/",
        "package_name": "{node_abi}-{platform}-{arch}.tar.gz"
    },
    "bugs": {
        "url": "http://github.com/libxmljs/libxmljs/issues"
    },
    "contributors": [
        {
            "name": "Jeff Smick"
        }
    ],
    "dependencies": {
        "bindings": "1.2.1",
        "nan": "~2.5.0",
        "node-pre-gyp": "~0.6.32"
    },
    "description": "libxml bindings for v8 javascript engine",
    "devDependencies": {
        "nodeunit": "0.9.0"
    },
    "directories": {},
    "dist": {
        "shasum": "253028925900e9f8d454418034a25b8af4e1507f",
        "tarball": "https://registry.npmjs.org/libxmljs/-/libxmljs-0.18.4.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "homepage": "https://github.com/libxmljs/libxmljs",
    "license": "MIT",
    "main": "./index",
    "maintainers": [
        {
            "name": "defunctzombie",
            "email": "shtylman@gmail.com"
        },
        {
            "name": "polotek",
            "email": "marco.rogers@gmail.com"
        },
        {
            "name": "rchipka",
            "email": "chipka01@email.franklin.edu"
        }
    ],
    "name": "libxmljs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/libxmljs/libxmljs.git"
    },
    "scripts": {
        "install": "node-pre-gyp install --fallback-to-build --loglevel http",
        "test": "node --expose_gc ./node_modules/.bin/nodeunit test"
    },
    "version": "0.18.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module libxmljs](#apidoc.module.libxmljs)
1.  boolean <span class="apidocSignatureSpan">libxmljs.</span>libxml_debug_enabled
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>Comment (doc, content)](#apidoc.element.libxmljs.Comment)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>Document (version, encoding)](#apidoc.element.libxmljs.Document)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>Element (doc, name, content)](#apidoc.element.libxmljs.Element)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>SaxParser (callbacks)](#apidoc.element.libxmljs.SaxParser)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>SaxPushParser (callbacks)](#apidoc.element.libxmljs.SaxPushParser)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>Text (doc, content)](#apidoc.element.libxmljs.Text)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>memoryUsage ()](#apidoc.element.libxmljs.memoryUsage)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>nodeCount ()](#apidoc.element.libxmljs.nodeCount)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>parseHtml (string, opts)](#apidoc.element.libxmljs.parseHtml)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>parseHtmlFragment (string, opts)](#apidoc.element.libxmljs.parseHtmlFragment)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>parseHtmlString (string, opts)](#apidoc.element.libxmljs.parseHtmlString)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>parseXml (string, options)](#apidoc.element.libxmljs.parseXml)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>parseXmlString (string, options)](#apidoc.element.libxmljs.parseXmlString)
1.  object <span class="apidocSignatureSpan">libxmljs.</span>Comment.prototype
1.  object <span class="apidocSignatureSpan">libxmljs.</span>Document.prototype
1.  object <span class="apidocSignatureSpan">libxmljs.</span>Element.prototype
1.  object <span class="apidocSignatureSpan">libxmljs.</span>Text.prototype
1.  object <span class="apidocSignatureSpan">libxmljs.</span>bindings
1.  object <span class="apidocSignatureSpan">libxmljs.</span>features
1.  object <span class="apidocSignatureSpan">libxmljs.</span>sax_parser
1.  string <span class="apidocSignatureSpan">libxmljs.</span>libxml_parser_version
1.  string <span class="apidocSignatureSpan">libxmljs.</span>libxml_version
1.  string <span class="apidocSignatureSpan">libxmljs.</span>version

#### [module libxmljs.Comment](#apidoc.module.libxmljs.Comment)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>Comment (doc, content)](#apidoc.element.libxmljs.Comment.Comment)

#### [module libxmljs.Comment.prototype](#apidoc.module.libxmljs.Comment.prototype)
1.  [function <span class="apidocSignatureSpan">libxmljs.Comment.prototype.</span>text ()](#apidoc.element.libxmljs.Comment.prototype.text)

#### [module libxmljs.Document](#apidoc.module.libxmljs.Document)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>Document (version, encoding)](#apidoc.element.libxmljs.Document.Document)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromHtml (string, opts)](#apidoc.element.libxmljs.Document.fromHtml)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromHtmlFragment (string, opts)](#apidoc.element.libxmljs.Document.fromHtmlFragment)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromHtmlString (string, opts)](#apidoc.element.libxmljs.Document.fromHtmlString)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromXml (string, options)](#apidoc.element.libxmljs.Document.fromXml)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromXmlString (string, options)](#apidoc.element.libxmljs.Document.fromXmlString)

#### [module libxmljs.Document.prototype](#apidoc.module.libxmljs.Document.prototype)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_encoding ()](#apidoc.element.libxmljs.Document.prototype._encoding)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_getDtd ()](#apidoc.element.libxmljs.Document.prototype._getDtd)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_rngValidate ()](#apidoc.element.libxmljs.Document.prototype._rngValidate)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_root ()](#apidoc.element.libxmljs.Document.prototype._root)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_setDtd ()](#apidoc.element.libxmljs.Document.prototype._setDtd)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_toString ()](#apidoc.element.libxmljs.Document.prototype._toString)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_validate ()](#apidoc.element.libxmljs.Document.prototype._validate)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_version ()](#apidoc.element.libxmljs.Document.prototype._version)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>child (id)](#apidoc.element.libxmljs.Document.prototype.child)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>childNodes ()](#apidoc.element.libxmljs.Document.prototype.childNodes)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>encoding (encoding)](#apidoc.element.libxmljs.Document.prototype.encoding)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>find (xpath, ns_uri)](#apidoc.element.libxmljs.Document.prototype.find)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>get (xpath, ns_uri)](#apidoc.element.libxmljs.Document.prototype.get)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>getDtd ()](#apidoc.element.libxmljs.Document.prototype.getDtd)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>namespaces ()](#apidoc.element.libxmljs.Document.prototype.namespaces)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>node (name, content)](#apidoc.element.libxmljs.Document.prototype.node)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>rngValidate (rng)](#apidoc.element.libxmljs.Document.prototype.rngValidate)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>root (elem)](#apidoc.element.libxmljs.Document.prototype.root)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>setDtd (name, ext, sys)](#apidoc.element.libxmljs.Document.prototype.setDtd)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>toString (formatted)](#apidoc.element.libxmljs.Document.prototype.toString)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>type ()](#apidoc.element.libxmljs.Document.prototype.type)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>validate (xsd)](#apidoc.element.libxmljs.Document.prototype.validate)
1.  [function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>version ()](#apidoc.element.libxmljs.Document.prototype.version)

#### [module libxmljs.Element](#apidoc.module.libxmljs.Element)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>Element (doc, name, content)](#apidoc.element.libxmljs.Element.Element)

#### [module libxmljs.Element.prototype](#apidoc.module.libxmljs.Element.prototype)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>_attr ()](#apidoc.element.libxmljs.Element.prototype._attr)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>addCData ()](#apidoc.element.libxmljs.Element.prototype.addCData)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>addChild ()](#apidoc.element.libxmljs.Element.prototype.addChild)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>addNextSibling ()](#apidoc.element.libxmljs.Element.prototype.addNextSibling)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>addPrevSibling ()](#apidoc.element.libxmljs.Element.prototype.addPrevSibling)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>attr ()](#apidoc.element.libxmljs.Element.prototype.attr)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>attrs ()](#apidoc.element.libxmljs.Element.prototype.attrs)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>cdata (content)](#apidoc.element.libxmljs.Element.prototype.cdata)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>child ()](#apidoc.element.libxmljs.Element.prototype.child)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>childNodes ()](#apidoc.element.libxmljs.Element.prototype.childNodes)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>defineNamespace (prefix, href)](#apidoc.element.libxmljs.Element.prototype.defineNamespace)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>find ()](#apidoc.element.libxmljs.Element.prototype.find)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>get ()](#apidoc.element.libxmljs.Element.prototype.get)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>name ()](#apidoc.element.libxmljs.Element.prototype.name)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>nextElement ()](#apidoc.element.libxmljs.Element.prototype.nextElement)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>node (name, content)](#apidoc.element.libxmljs.Element.prototype.node)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>path ()](#apidoc.element.libxmljs.Element.prototype.path)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>prevElement ()](#apidoc.element.libxmljs.Element.prototype.prevElement)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>replace ()](#apidoc.element.libxmljs.Element.prototype.replace)
1.  [function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>text ()](#apidoc.element.libxmljs.Element.prototype.text)

#### [module libxmljs.Text](#apidoc.module.libxmljs.Text)
1.  [function <span class="apidocSignatureSpan">libxmljs.</span>Text (doc, content)](#apidoc.element.libxmljs.Text.Text)

#### [module libxmljs.Text.prototype](#apidoc.module.libxmljs.Text.prototype)
1.  [function <span class="apidocSignatureSpan">libxmljs.Text.prototype.</span>nextElement ()](#apidoc.element.libxmljs.Text.prototype.nextElement)
1.  [function <span class="apidocSignatureSpan">libxmljs.Text.prototype.</span>prevElement ()](#apidoc.element.libxmljs.Text.prototype.prevElement)
1.  [function <span class="apidocSignatureSpan">libxmljs.Text.prototype.</span>replace ()](#apidoc.element.libxmljs.Text.prototype.replace)
1.  [function <span class="apidocSignatureSpan">libxmljs.Text.prototype.</span>text ()](#apidoc.element.libxmljs.Text.prototype.text)

#### [module libxmljs.bindings](#apidoc.module.libxmljs.bindings)
1.  boolean <span class="apidocSignatureSpan">libxmljs.bindings.</span>libxml_debug_enabled
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Attribute ()](#apidoc.element.libxmljs.bindings.Attribute)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Comment ()](#apidoc.element.libxmljs.bindings.Comment)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Document ()](#apidoc.element.libxmljs.bindings.Document)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Element ()](#apidoc.element.libxmljs.bindings.Element)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Namespace ()](#apidoc.element.libxmljs.bindings.Namespace)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>SaxParser ()](#apidoc.element.libxmljs.bindings.SaxParser)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>SaxPushParser ()](#apidoc.element.libxmljs.bindings.SaxPushParser)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Text ()](#apidoc.element.libxmljs.bindings.Text)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>fromHtml ()](#apidoc.element.libxmljs.bindings.fromHtml)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>fromXml ()](#apidoc.element.libxmljs.bindings.fromXml)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>xmlMemUsed ()](#apidoc.element.libxmljs.bindings.xmlMemUsed)
1.  [function <span class="apidocSignatureSpan">libxmljs.bindings.</span>xmlNodeCount ()](#apidoc.element.libxmljs.bindings.xmlNodeCount)
1.  object <span class="apidocSignatureSpan">libxmljs.bindings.</span>features
1.  object <span class="apidocSignatureSpan">libxmljs.bindings.</span>libxml
1.  string <span class="apidocSignatureSpan">libxmljs.bindings.</span>libxml_parser_version
1.  string <span class="apidocSignatureSpan">libxmljs.bindings.</span>libxml_version
1.  string <span class="apidocSignatureSpan">libxmljs.bindings.</span>path

#### [module libxmljs.sax_parser](#apidoc.module.libxmljs.sax_parser)
1.  [function <span class="apidocSignatureSpan">libxmljs.sax_parser.</span>SaxParser (callbacks)](#apidoc.element.libxmljs.sax_parser.SaxParser)
1.  [function <span class="apidocSignatureSpan">libxmljs.sax_parser.</span>SaxPushParser (callbacks)](#apidoc.element.libxmljs.sax_parser.SaxPushParser)



# <a name="apidoc.module.libxmljs"></a>[module libxmljs](#apidoc.module.libxmljs)

#### <a name="apidoc.element.libxmljs.Comment"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>Comment (doc, content)](#apidoc.element.libxmljs.Comment)
- description and source-code
```javascript
Comment = function (doc, content) {
    if (!doc) {
        throw new Error('document argument required');
    } else if (! (doc instanceof bindings.Document)) {
        throw new Error('document argument must be an ' +
                        'instance of Document');
    }

    return new bindings.Comment(doc, content);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>Document (version, encoding)](#apidoc.element.libxmljs.Document)
- description and source-code
```javascript
function Document(version, encoding) {
    version = version || '1.0';
    var doc = new bindings.Document(version);
    doc.encoding(encoding || 'utf8');
    return doc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>Element (doc, name, content)](#apidoc.element.libxmljs.Element)
- description and source-code
```javascript
function Element(doc, name, content) {
    if (!doc) {
        throw new Error('document argument required');
    } else if (! (doc instanceof bindings.Document)) {
        throw new Error('document argument must be an ' +
                        'instance of Document');
    } else if (!name) {
        throw new Error('name argument required');
    }

    return new bindings.Element(doc, name, content);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.SaxParser"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>SaxParser (callbacks)](#apidoc.element.libxmljs.SaxParser)
- description and source-code
```javascript
SaxParser = function (callbacks) {
    var parser = new bindings.SaxParser();

    // attach callbacks
    for (var callback in callbacks) {
        parser.on(callback, callbacks[callback]);
    }

    return parser;
}
```
- example usage
```shell
...


var events = require('events');

var bindings = require('./bindings');

var SaxParser = function(callbacks) {
var parser = new bindings.SaxParser();

// attach callbacks
for (var callback in callbacks) {
    parser.on(callback, callbacks[callback]);
}

return parser;
...
```

#### <a name="apidoc.element.libxmljs.SaxPushParser"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>SaxPushParser (callbacks)](#apidoc.element.libxmljs.SaxPushParser)
- description and source-code
```javascript
SaxPushParser = function (callbacks) {
    var parser = new bindings.SaxPushParser();

    // attach callbacks
    for (var callback in callbacks) {
        parser.on(callback, callbacks[callback]);
    }

    return parser;
}
```
- example usage
```shell
...

// Overriding the prototype, like util.inherit, wipes out the native binding.
// Copy over the methods instead.
for (var k in events.EventEmitter.prototype)
bindings.SaxParser.prototype[k] = events.EventEmitter.prototype[k];

var SaxPushParser = function(callbacks) {
var parser = new bindings.SaxPushParser();

// attach callbacks
for (var callback in callbacks) {
    parser.on(callback, callbacks[callback]);
}

return parser;
...
```

#### <a name="apidoc.element.libxmljs.Text"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>Text (doc, content)](#apidoc.element.libxmljs.Text)
- description and source-code
```javascript
function Text(doc, content) {
    if (!doc) {
        throw new Error('document argument required');
    }

    if (!(doc instanceof bindings.Document)) {
        throw new Error('document argument must be an instance of Document');
    }

    if (!content) {
        throw new Error('content argument required');
    }

    return new bindings.Text(doc, content);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.memoryUsage"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>memoryUsage ()](#apidoc.element.libxmljs.memoryUsage)
- description and source-code
```javascript
function xmlMemUsed() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.nodeCount"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>nodeCount ()](#apidoc.element.libxmljs.nodeCount)
- description and source-code
```javascript
function xmlNodeCount() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.parseHtml"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>parseHtml (string, opts)](#apidoc.element.libxmljs.parseHtml)
- description and source-code
```javascript
parseHtml = function (string, opts) {
    opts = opts || {};

    // if for some reason user did not specify an object for the options
    if (typeof(opts) !== 'object') {
        throw new Error('fromHtml options must be an object');
    }

    return bindings.fromHtml(string, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.parseHtmlFragment"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>parseHtmlFragment (string, opts)](#apidoc.element.libxmljs.parseHtmlFragment)
- description and source-code
```javascript
parseHtmlFragment = function (string, opts) {
    opts = opts || {};

    // if for some reason user did not specify an object for the options
    if (typeof(opts) !== 'object') {
        throw new Error('fromHtmlFragment options must be an object');
    }

    opts.doctype = false;
    opts.implied = false;

    return bindings.fromHtml(string, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.parseHtmlString"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>parseHtmlString (string, opts)](#apidoc.element.libxmljs.parseHtmlString)
- description and source-code
```javascript
parseHtmlString = function (string, opts) {
    opts = opts || {};

    // if for some reason user did not specify an object for the options
    if (typeof(opts) !== 'object') {
        throw new Error('fromHtml options must be an object');
    }

    return bindings.fromHtml(string, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.parseXml"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>parseXml (string, options)](#apidoc.element.libxmljs.parseXml)
- description and source-code
```javascript
parseXml = function (string, options) {
    return bindings.fromXml(string, options || {});
}
```
- example usage
```shell
...
           '<root>' +
               '<child foo="bar">' +
                   '<grandchild baz="fizbuzz">grandchild content</grandchild>' +
               '</child>' +
               '<sibling>with content!</sibling>' +
           '</root>';

var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
...
```

#### <a name="apidoc.element.libxmljs.parseXmlString"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>parseXmlString (string, options)](#apidoc.element.libxmljs.parseXmlString)
- description and source-code
```javascript
parseXmlString = function (string, options) {
    return bindings.fromXml(string, options || {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.libxmljs.Comment"></a>[module libxmljs.Comment](#apidoc.module.libxmljs.Comment)

#### <a name="apidoc.element.libxmljs.Comment.Comment"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>Comment (doc, content)](#apidoc.element.libxmljs.Comment.Comment)
- description and source-code
```javascript
Comment = function (doc, content) {
    if (!doc) {
        throw new Error('document argument required');
    } else if (! (doc instanceof bindings.Document)) {
        throw new Error('document argument must be an ' +
                        'instance of Document');
    }

    return new bindings.Comment(doc, content);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.libxmljs.Comment.prototype"></a>[module libxmljs.Comment.prototype](#apidoc.module.libxmljs.Comment.prototype)

#### <a name="apidoc.element.libxmljs.Comment.prototype.text"></a>[function <span class="apidocSignatureSpan">libxmljs.Comment.prototype.</span>text ()](#apidoc.element.libxmljs.Comment.prototype.text)
- description and source-code
```javascript
function text() { [native code] }
```
- example usage
```shell
...
           '</root>';

var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
'''
...
```



# <a name="apidoc.module.libxmljs.Document"></a>[module libxmljs.Document](#apidoc.module.libxmljs.Document)

#### <a name="apidoc.element.libxmljs.Document.Document"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>Document (version, encoding)](#apidoc.element.libxmljs.Document.Document)
- description and source-code
```javascript
function Document(version, encoding) {
    version = version || '1.0';
    var doc = new bindings.Document(version);
    doc.encoding(encoding || 'utf8');
    return doc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.fromHtml"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromHtml (string, opts)](#apidoc.element.libxmljs.Document.fromHtml)
- description and source-code
```javascript
fromHtml = function (string, opts) {
    opts = opts || {};

    // if for some reason user did not specify an object for the options
    if (typeof(opts) !== 'object') {
        throw new Error('fromHtml options must be an object');
    }

    return bindings.fromHtml(string, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.fromHtmlFragment"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromHtmlFragment (string, opts)](#apidoc.element.libxmljs.Document.fromHtmlFragment)
- description and source-code
```javascript
fromHtmlFragment = function (string, opts) {
    opts = opts || {};

    // if for some reason user did not specify an object for the options
    if (typeof(opts) !== 'object') {
        throw new Error('fromHtmlFragment options must be an object');
    }

    opts.doctype = false;
    opts.implied = false;

    return bindings.fromHtml(string, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.fromHtmlString"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromHtmlString (string, opts)](#apidoc.element.libxmljs.Document.fromHtmlString)
- description and source-code
```javascript
fromHtmlString = function (string, opts) {
    opts = opts || {};

    // if for some reason user did not specify an object for the options
    if (typeof(opts) !== 'object') {
        throw new Error('fromHtml options must be an object');
    }

    return bindings.fromHtml(string, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.fromXml"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromXml (string, options)](#apidoc.element.libxmljs.Document.fromXml)
- description and source-code
```javascript
fromXml = function (string, options) {
    return bindings.fromXml(string, options || {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.fromXmlString"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.</span>fromXmlString (string, options)](#apidoc.element.libxmljs.Document.fromXmlString)
- description and source-code
```javascript
fromXmlString = function (string, options) {
    return bindings.fromXml(string, options || {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.libxmljs.Document.prototype"></a>[module libxmljs.Document.prototype](#apidoc.module.libxmljs.Document.prototype)

#### <a name="apidoc.element.libxmljs.Document.prototype._encoding"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_encoding ()](#apidoc.element.libxmljs.Document.prototype._encoding)
- description and source-code
```javascript
function _encoding() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype._getDtd"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_getDtd ()](#apidoc.element.libxmljs.Document.prototype._getDtd)
- description and source-code
```javascript
function _getDtd() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype._rngValidate"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_rngValidate ()](#apidoc.element.libxmljs.Document.prototype._rngValidate)
- description and source-code
```javascript
function _rngValidate() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype._root"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_root ()](#apidoc.element.libxmljs.Document.prototype._root)
- description and source-code
```javascript
function _root() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype._setDtd"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_setDtd ()](#apidoc.element.libxmljs.Document.prototype._setDtd)
- description and source-code
```javascript
function _setDtd() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype._toString"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_toString ()](#apidoc.element.libxmljs.Document.prototype._toString)
- description and source-code
```javascript
function _toString() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype._validate"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_validate ()](#apidoc.element.libxmljs.Document.prototype._validate)
- description and source-code
```javascript
function _validate() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype._version"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>_version ()](#apidoc.element.libxmljs.Document.prototype._version)
- description and source-code
```javascript
function _version() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.child"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>child (id)](#apidoc.element.libxmljs.Document.prototype.child)
- description and source-code
```javascript
child = function (id) {
    if (id === undefined || typeof id !== 'number') {
        throw new Error('id argument required for #child');
    }

    assertRoot(this);

    return this.root().child(id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.childNodes"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>childNodes ()](#apidoc.element.libxmljs.Document.prototype.childNodes)
- description and source-code
```javascript
childNodes = function () {
    assertRoot(this);

    return this.root().childNodes();
}
```
- example usage
```shell
...
var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
'''

## Support
...
```

#### <a name="apidoc.element.libxmljs.Document.prototype.encoding"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>encoding (encoding)](#apidoc.element.libxmljs.Document.prototype.encoding)
- description and source-code
```javascript
encoding = function (encoding) {
    return this._encoding(encoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.find"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>find (xpath, ns_uri)](#apidoc.element.libxmljs.Document.prototype.find)
- description and source-code
```javascript
find = function (xpath, ns_uri) {
    assertRoot(this);

    return this.root().find(xpath, ns_uri);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.get"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>get (xpath, ns_uri)](#apidoc.element.libxmljs.Document.prototype.get)
- description and source-code
```javascript
get = function (xpath, ns_uri) {
    assertRoot(this);

    return this.root().get(xpath, ns_uri);
}
```
- example usage
```shell
...
               '</child>' +
               '<sibling>with content!</sibling>' +
           '</root>';

var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
...
```

#### <a name="apidoc.element.libxmljs.Document.prototype.getDtd"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>getDtd ()](#apidoc.element.libxmljs.Document.prototype.getDtd)
- description and source-code
```javascript
getDtd = function () {
    return this._getDtd();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.namespaces"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>namespaces ()](#apidoc.element.libxmljs.Document.prototype.namespaces)
- description and source-code
```javascript
namespaces = function () {
    assertRoot(this);

    return this.root().namespaces();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.node"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>node (name, content)](#apidoc.element.libxmljs.Document.prototype.node)
- description and source-code
```javascript
node = function (name, content) {
    return this.root(Element(this, name, content));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.rngValidate"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>rngValidate (rng)](#apidoc.element.libxmljs.Document.prototype.rngValidate)
- description and source-code
```javascript
rngValidate = function (rng) {
    return this._rngValidate(rng);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.root"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>root (elem)](#apidoc.element.libxmljs.Document.prototype.root)
- description and source-code
```javascript
root = function (elem) {
    return this._root(elem);
}
```
- example usage
```shell
...
var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
'''

## Support
...
```

#### <a name="apidoc.element.libxmljs.Document.prototype.setDtd"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>setDtd (name, ext, sys)](#apidoc.element.libxmljs.Document.prototype.setDtd)
- description and source-code
```javascript
setDtd = function (name, ext, sys) {
    if (!name) {
        throw new Error('Must pass in a DTD name');
    } else if (typeof name !== 'string') {
        throw new Error('Must pass in a valid DTD name');
    }

    var params = [name];
    if (typeof ext !== 'undefined') {
        params.push(ext);
    }
    if (ext && typeof sys !== 'undefined') {
        params.push(sys);
    }

    return this._setDtd.apply(this, params);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.toString"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>toString (formatted)](#apidoc.element.libxmljs.Document.prototype.toString)
- description and source-code
```javascript
toString = function (formatted) {
    return this._toString(formatted !== undefined ? formatted : true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.type"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>type ()](#apidoc.element.libxmljs.Document.prototype.type)
- description and source-code
```javascript
type = function () {
    return 'document';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.validate"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>validate (xsd)](#apidoc.element.libxmljs.Document.prototype.validate)
- description and source-code
```javascript
validate = function (xsd) {
    return this._validate(xsd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Document.prototype.version"></a>[function <span class="apidocSignatureSpan">libxmljs.Document.prototype.</span>version ()](#apidoc.element.libxmljs.Document.prototype.version)
- description and source-code
```javascript
version = function () {
    return this._version();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.libxmljs.Element"></a>[module libxmljs.Element](#apidoc.module.libxmljs.Element)

#### <a name="apidoc.element.libxmljs.Element.Element"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>Element (doc, name, content)](#apidoc.element.libxmljs.Element.Element)
- description and source-code
```javascript
function Element(doc, name, content) {
    if (!doc) {
        throw new Error('document argument required');
    } else if (! (doc instanceof bindings.Document)) {
        throw new Error('document argument must be an ' +
                        'instance of Document');
    } else if (!name) {
        throw new Error('name argument required');
    }

    return new bindings.Element(doc, name, content);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.libxmljs.Element.prototype"></a>[module libxmljs.Element.prototype](#apidoc.module.libxmljs.Element.prototype)

#### <a name="apidoc.element.libxmljs.Element.prototype._attr"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>_attr ()](#apidoc.element.libxmljs.Element.prototype._attr)
- description and source-code
```javascript
function _attr() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.addCData"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>addCData ()](#apidoc.element.libxmljs.Element.prototype.addCData)
- description and source-code
```javascript
function addCData() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.addChild"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>addChild ()](#apidoc.element.libxmljs.Element.prototype.addChild)
- description and source-code
```javascript
function addChild() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.addNextSibling"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>addNextSibling ()](#apidoc.element.libxmljs.Element.prototype.addNextSibling)
- description and source-code
```javascript
function addNextSibling() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.addPrevSibling"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>addPrevSibling ()](#apidoc.element.libxmljs.Element.prototype.addPrevSibling)
- description and source-code
```javascript
function addPrevSibling() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.attr"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>attr ()](#apidoc.element.libxmljs.Element.prototype.attr)
- description and source-code
```javascript
attr = function () {
    if (arguments.length === 1) {
        var arg = arguments[0];
        if (typeof arg === 'object') {
            // object setter
            // iterate keys/value to set attributes
            for (var k in arg) {
                this._attr(k, arg[k]);
            };
            return this;
        } else if (typeof arg === 'string') {
            // getter
            return this._attr(arg);
        }
    } else if (arguments.length === 2) {
        // 2 arg setter
        var name = arguments[0];
        var value = arguments[1];
        this._attr(name, value);
        return this;
    }
}
```
- example usage
```shell
...
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
'''

## Support

* Docs - [http://github.com/libxmljs/libxmljs/wiki](http://github.com/libxmljs/libxmljs/wiki)
* Mailing list - [http://groups.google.com/group/libxmljs](http://groups.google.com/group/libxmljs)
...
```

#### <a name="apidoc.element.libxmljs.Element.prototype.attrs"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>attrs ()](#apidoc.element.libxmljs.Element.prototype.attrs)
- description and source-code
```javascript
function attrs() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.cdata"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>cdata (content)](#apidoc.element.libxmljs.Element.prototype.cdata)
- description and source-code
```javascript
cdata = function (content) {
  this.addCData(content);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.child"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>child ()](#apidoc.element.libxmljs.Element.prototype.child)
- description and source-code
```javascript
function child() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.childNodes"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>childNodes ()](#apidoc.element.libxmljs.Element.prototype.childNodes)
- description and source-code
```javascript
function childNodes() { [native code] }
```
- example usage
```shell
...
var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
'''

## Support
...
```

#### <a name="apidoc.element.libxmljs.Element.prototype.defineNamespace"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>defineNamespace (prefix, href)](#apidoc.element.libxmljs.Element.prototype.defineNamespace)
- description and source-code
```javascript
defineNamespace = function (prefix, href) {
    // if no prefix specified
    if (!href) {
        href = prefix;
        prefix = null;
    }
    return new bindings.Namespace(this, prefix, href);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.find"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>find ()](#apidoc.element.libxmljs.Element.prototype.find)
- description and source-code
```javascript
function find() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.get"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>get ()](#apidoc.element.libxmljs.Element.prototype.get)
- description and source-code
```javascript
get = function () {
    var res = this.find.apply(this, arguments);
    if (res instanceof Array) {
        return res[0];
    } else {
        return res;
    }
}
```
- example usage
```shell
...
               '</child>' +
               '<sibling>with content!</sibling>' +
           '</root>';

var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
...
```

#### <a name="apidoc.element.libxmljs.Element.prototype.name"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>name ()](#apidoc.element.libxmljs.Element.prototype.name)
- description and source-code
```javascript
function name() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.nextElement"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>nextElement ()](#apidoc.element.libxmljs.Element.prototype.nextElement)
- description and source-code
```javascript
function nextElement() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.node"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>node (name, content)](#apidoc.element.libxmljs.Element.prototype.node)
- description and source-code
```javascript
node = function (name, content) {
    var elem = Element(this.doc(), name, content);
    this.addChild(elem);
    return elem;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.path"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>path ()](#apidoc.element.libxmljs.Element.prototype.path)
- description and source-code
```javascript
function path() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.prevElement"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>prevElement ()](#apidoc.element.libxmljs.Element.prototype.prevElement)
- description and source-code
```javascript
function prevElement() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.replace"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>replace ()](#apidoc.element.libxmljs.Element.prototype.replace)
- description and source-code
```javascript
function replace() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Element.prototype.text"></a>[function <span class="apidocSignatureSpan">libxmljs.Element.prototype.</span>text ()](#apidoc.element.libxmljs.Element.prototype.text)
- description and source-code
```javascript
function text() { [native code] }
```
- example usage
```shell
...
           '</root>';

var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
'''
...
```



# <a name="apidoc.module.libxmljs.Text"></a>[module libxmljs.Text](#apidoc.module.libxmljs.Text)

#### <a name="apidoc.element.libxmljs.Text.Text"></a>[function <span class="apidocSignatureSpan">libxmljs.</span>Text (doc, content)](#apidoc.element.libxmljs.Text.Text)
- description and source-code
```javascript
function Text(doc, content) {
    if (!doc) {
        throw new Error('document argument required');
    }

    if (!(doc instanceof bindings.Document)) {
        throw new Error('document argument must be an instance of Document');
    }

    if (!content) {
        throw new Error('content argument required');
    }

    return new bindings.Text(doc, content);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.libxmljs.Text.prototype"></a>[module libxmljs.Text.prototype](#apidoc.module.libxmljs.Text.prototype)

#### <a name="apidoc.element.libxmljs.Text.prototype.nextElement"></a>[function <span class="apidocSignatureSpan">libxmljs.Text.prototype.</span>nextElement ()](#apidoc.element.libxmljs.Text.prototype.nextElement)
- description and source-code
```javascript
function nextElement() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Text.prototype.prevElement"></a>[function <span class="apidocSignatureSpan">libxmljs.Text.prototype.</span>prevElement ()](#apidoc.element.libxmljs.Text.prototype.prevElement)
- description and source-code
```javascript
function prevElement() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Text.prototype.replace"></a>[function <span class="apidocSignatureSpan">libxmljs.Text.prototype.</span>replace ()](#apidoc.element.libxmljs.Text.prototype.replace)
- description and source-code
```javascript
function replace() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.Text.prototype.text"></a>[function <span class="apidocSignatureSpan">libxmljs.Text.prototype.</span>text ()](#apidoc.element.libxmljs.Text.prototype.text)
- description and source-code
```javascript
function text() { [native code] }
```
- example usage
```shell
...
           '</root>';

var xmlDoc = libxmljs.parseXml(xml);

// xpath queries
var gchild = xmlDoc.get('//grandchild');

console.log(gchild.text());  // prints "grandchild content"

var children = xmlDoc.root().childNodes();
var child = children[0];

console.log(child.attr('foo').value()); // prints "bar"
'''
...
```



# <a name="apidoc.module.libxmljs.bindings"></a>[module libxmljs.bindings](#apidoc.module.libxmljs.bindings)

#### <a name="apidoc.element.libxmljs.bindings.Attribute"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Attribute ()](#apidoc.element.libxmljs.bindings.Attribute)
- description and source-code
```javascript
Attribute = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.Comment"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Comment ()](#apidoc.element.libxmljs.bindings.Comment)
- description and source-code
```javascript
Comment = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.Document"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Document ()](#apidoc.element.libxmljs.bindings.Document)
- description and source-code
```javascript
function Document() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.Element"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Element ()](#apidoc.element.libxmljs.bindings.Element)
- description and source-code
```javascript
Element = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.Namespace"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Namespace ()](#apidoc.element.libxmljs.bindings.Namespace)
- description and source-code
```javascript
Namespace = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.SaxParser"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>SaxParser ()](#apidoc.element.libxmljs.bindings.SaxParser)
- description and source-code
```javascript
SaxParser = function () { [native code] }
```
- example usage
```shell
...


var events = require('events');

var bindings = require('./bindings');

var SaxParser = function(callbacks) {
var parser = new bindings.SaxParser();

// attach callbacks
for (var callback in callbacks) {
    parser.on(callback, callbacks[callback]);
}

return parser;
...
```

#### <a name="apidoc.element.libxmljs.bindings.SaxPushParser"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>SaxPushParser ()](#apidoc.element.libxmljs.bindings.SaxPushParser)
- description and source-code
```javascript
SaxPushParser = function () { [native code] }
```
- example usage
```shell
...

// Overriding the prototype, like util.inherit, wipes out the native binding.
// Copy over the methods instead.
for (var k in events.EventEmitter.prototype)
bindings.SaxParser.prototype[k] = events.EventEmitter.prototype[k];

var SaxPushParser = function(callbacks) {
var parser = new bindings.SaxPushParser();

// attach callbacks
for (var callback in callbacks) {
    parser.on(callback, callbacks[callback]);
}

return parser;
...
```

#### <a name="apidoc.element.libxmljs.bindings.Text"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>Text ()](#apidoc.element.libxmljs.bindings.Text)
- description and source-code
```javascript
Text = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.fromHtml"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>fromHtml ()](#apidoc.element.libxmljs.bindings.fromHtml)
- description and source-code
```javascript
function fromHtml() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.fromXml"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>fromXml ()](#apidoc.element.libxmljs.bindings.fromXml)
- description and source-code
```javascript
function fromXml() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.xmlMemUsed"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>xmlMemUsed ()](#apidoc.element.libxmljs.bindings.xmlMemUsed)
- description and source-code
```javascript
function xmlMemUsed() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.libxmljs.bindings.xmlNodeCount"></a>[function <span class="apidocSignatureSpan">libxmljs.bindings.</span>xmlNodeCount ()](#apidoc.element.libxmljs.bindings.xmlNodeCount)
- description and source-code
```javascript
function xmlNodeCount() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.libxmljs.sax_parser"></a>[module libxmljs.sax_parser](#apidoc.module.libxmljs.sax_parser)

#### <a name="apidoc.element.libxmljs.sax_parser.SaxParser"></a>[function <span class="apidocSignatureSpan">libxmljs.sax_parser.</span>SaxParser (callbacks)](#apidoc.element.libxmljs.sax_parser.SaxParser)
- description and source-code
```javascript
SaxParser = function (callbacks) {
    var parser = new bindings.SaxParser();

    // attach callbacks
    for (var callback in callbacks) {
        parser.on(callback, callbacks[callback]);
    }

    return parser;
}
```
- example usage
```shell
...


var events = require('events');

var bindings = require('./bindings');

var SaxParser = function(callbacks) {
var parser = new bindings.SaxParser();

// attach callbacks
for (var callback in callbacks) {
    parser.on(callback, callbacks[callback]);
}

return parser;
...
```

#### <a name="apidoc.element.libxmljs.sax_parser.SaxPushParser"></a>[function <span class="apidocSignatureSpan">libxmljs.sax_parser.</span>SaxPushParser (callbacks)](#apidoc.element.libxmljs.sax_parser.SaxPushParser)
- description and source-code
```javascript
SaxPushParser = function (callbacks) {
    var parser = new bindings.SaxPushParser();

    // attach callbacks
    for (var callback in callbacks) {
        parser.on(callback, callbacks[callback]);
    }

    return parser;
}
```
- example usage
```shell
...

// Overriding the prototype, like util.inherit, wipes out the native binding.
// Copy over the methods instead.
for (var k in events.EventEmitter.prototype)
bindings.SaxParser.prototype[k] = events.EventEmitter.prototype[k];

var SaxPushParser = function(callbacks) {
var parser = new bindings.SaxPushParser();

// attach callbacks
for (var callback in callbacks) {
    parser.on(callback, callbacks[callback]);
}

return parser;
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
