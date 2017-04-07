# api documentation for  [tar-stream (v1.5.2)](https://github.com/mafintosh/tar-stream)  [![npm package](https://img.shields.io/npm/v/npmdoc-tar-stream.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tar-stream) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tar-stream.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tar-stream)
#### tar-stream is a streaming tar parser and generator and nothing else. It is streams2 and operates purely using streams which means you can easily extract/parse tarballs without ever hitting the file system.

[![NPM](https://nodei.co/npm/tar-stream.png?downloads=true)](https://www.npmjs.com/package/tar-stream)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tar-stream/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-tar-stream_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tar-stream/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tar-stream/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tar-stream/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mathias Buus",
        "email": "mathiasbuus@gmail.com"
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
            "name": "mafintosh",
            "email": "mathiasbuus@gmail.com"
        },
        {
            "name": "maxogden",
            "email": "max@maxogden.com"
        }
    ],
    "name": "tar-stream",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module tar-stream](#apidoc.module.tar-stream)
1.  [function <span class="apidocSignatureSpan">tar-stream.</span>extract (opts)](#apidoc.element.tar-stream.extract)
1.  [function <span class="apidocSignatureSpan">tar-stream.</span>extract.super_ (options)](#apidoc.element.tar-stream.extract.super_)
1.  [function <span class="apidocSignatureSpan">tar-stream.</span>pack (opts)](#apidoc.element.tar-stream.pack)
1.  [function <span class="apidocSignatureSpan">tar-stream.</span>pack.super_ (options)](#apidoc.element.tar-stream.pack.super_)
1.  object <span class="apidocSignatureSpan">tar-stream.</span>extract.prototype
1.  object <span class="apidocSignatureSpan">tar-stream.</span>extract.super_.WritableState.prototype
1.  object <span class="apidocSignatureSpan">tar-stream.</span>extract.super_.prototype
1.  object <span class="apidocSignatureSpan">tar-stream.</span>headers
1.  object <span class="apidocSignatureSpan">tar-stream.</span>pack.prototype
1.  object <span class="apidocSignatureSpan">tar-stream.</span>pack.super_.Duplex.prototype
1.  object <span class="apidocSignatureSpan">tar-stream.</span>pack.super_.PassThrough.prototype
1.  object <span class="apidocSignatureSpan">tar-stream.</span>pack.super_.Transform.prototype
1.  object <span class="apidocSignatureSpan">tar-stream.</span>pack.super_.prototype

#### [module tar-stream.extract](#apidoc.module.tar-stream.extract)
1.  [function <span class="apidocSignatureSpan">tar-stream.</span>extract (opts)](#apidoc.element.tar-stream.extract.extract)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.</span>super_ (options)](#apidoc.element.tar-stream.extract.super_)

#### [module tar-stream.extract.prototype](#apidoc.module.tar-stream.extract.prototype)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.prototype.</span>_continue ()](#apidoc.element.tar-stream.extract.prototype._continue)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.prototype.</span>_parse (size, onparse)](#apidoc.element.tar-stream.extract.prototype._parse)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.prototype.</span>_write (data, enc, cb)](#apidoc.element.tar-stream.extract.prototype._write)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.prototype.</span>destroy (err)](#apidoc.element.tar-stream.extract.prototype.destroy)

#### [module tar-stream.extract.super_](#apidoc.module.tar-stream.extract.super_)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.</span>super_ ()](#apidoc.element.tar-stream.extract.super_.super_)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.</span>WritableState (options, stream)](#apidoc.element.tar-stream.extract.super_.WritableState)

#### [module tar-stream.extract.super_.WritableState.prototype](#apidoc.module.tar-stream.extract.super_.WritableState.prototype)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.WritableState.prototype.</span>getBuffer ()](#apidoc.element.tar-stream.extract.super_.WritableState.prototype.getBuffer)

#### [module tar-stream.extract.super_.prototype](#apidoc.module.tar-stream.extract.super_.prototype)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.tar-stream.extract.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>cork ()](#apidoc.element.tar-stream.extract.super_.prototype.cork)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.tar-stream.extract.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>pipe ()](#apidoc.element.tar-stream.extract.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.tar-stream.extract.super_.prototype.setDefaultEncoding)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>uncork ()](#apidoc.element.tar-stream.extract.super_.prototype.uncork)
1.  [function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.tar-stream.extract.super_.prototype.write)
1.  object <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>_writev

#### [module tar-stream.headers](#apidoc.module.tar-stream.headers)
1.  [function <span class="apidocSignatureSpan">tar-stream.headers.</span>decode (buf)](#apidoc.element.tar-stream.headers.decode)
1.  [function <span class="apidocSignatureSpan">tar-stream.headers.</span>decodeLongPath (buf)](#apidoc.element.tar-stream.headers.decodeLongPath)
1.  [function <span class="apidocSignatureSpan">tar-stream.headers.</span>decodePax (buf)](#apidoc.element.tar-stream.headers.decodePax)
1.  [function <span class="apidocSignatureSpan">tar-stream.headers.</span>encode (opts)](#apidoc.element.tar-stream.headers.encode)
1.  [function <span class="apidocSignatureSpan">tar-stream.headers.</span>encodePax (opts)](#apidoc.element.tar-stream.headers.encodePax)

#### [module tar-stream.pack](#apidoc.module.tar-stream.pack)
1.  [function <span class="apidocSignatureSpan">tar-stream.</span>pack (opts)](#apidoc.element.tar-stream.pack.pack)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.</span>super_ (options)](#apidoc.element.tar-stream.pack.super_)

#### [module tar-stream.pack.prototype](#apidoc.module.tar-stream.pack.prototype)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>_encode (header)](#apidoc.element.tar-stream.pack.prototype._encode)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>_encodePax (header)](#apidoc.element.tar-stream.pack.prototype._encodePax)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>_read (n)](#apidoc.element.tar-stream.pack.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>destroy (err)](#apidoc.element.tar-stream.pack.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>entry (header, buffer, callback)](#apidoc.element.tar-stream.pack.prototype.entry)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>finalize ()](#apidoc.element.tar-stream.pack.prototype.finalize)

#### [module tar-stream.pack.super_](#apidoc.module.tar-stream.pack.super_)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.</span>super_ ()](#apidoc.element.tar-stream.pack.super_.super_)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Duplex (options)](#apidoc.element.tar-stream.pack.super_.Duplex)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>PassThrough (options)](#apidoc.element.tar-stream.pack.super_.PassThrough)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Readable (options)](#apidoc.element.tar-stream.pack.super_.Readable)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>ReadableState (options, stream)](#apidoc.element.tar-stream.pack.super_.ReadableState)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Stream ()](#apidoc.element.tar-stream.pack.super_.Stream)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Transform (options)](#apidoc.element.tar-stream.pack.super_.Transform)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Writable (options)](#apidoc.element.tar-stream.pack.super_.Writable)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>_fromList (n, state)](#apidoc.element.tar-stream.pack.super_._fromList)

#### [module tar-stream.pack.super_.Duplex.prototype](#apidoc.module.tar-stream.pack.super_.Duplex.prototype)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Duplex.prototype._write)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>cork ()](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.cork)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.end)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.setDefaultEncoding)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>uncork ()](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.uncork)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.write)
1.  object <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>_writev

#### [module tar-stream.pack.super_.PassThrough.prototype](#apidoc.module.tar-stream.pack.super_.PassThrough.prototype)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.PassThrough.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.PassThrough.prototype._transform)

#### [module tar-stream.pack.super_.Transform.prototype](#apidoc.module.tar-stream.pack.super_.Transform.prototype)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Transform.prototype.</span>_read (n)](#apidoc.element.tar-stream.pack.super_.Transform.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Transform.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Transform.prototype._transform)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Transform.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Transform.prototype._write)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.Transform.prototype.</span>push (chunk, encoding)](#apidoc.element.tar-stream.pack.super_.Transform.prototype.push)

#### [module tar-stream.pack.super_.prototype](#apidoc.module.tar-stream.pack.super_.prototype)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>_read (n)](#apidoc.element.tar-stream.pack.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>addListener (ev, fn)](#apidoc.element.tar-stream.pack.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>isPaused ()](#apidoc.element.tar-stream.pack.super_.prototype.isPaused)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>on (ev, fn)](#apidoc.element.tar-stream.pack.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>pause ()](#apidoc.element.tar-stream.pack.super_.prototype.pause)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.tar-stream.pack.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.tar-stream.pack.super_.prototype.push)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>read (n)](#apidoc.element.tar-stream.pack.super_.prototype.read)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>resume ()](#apidoc.element.tar-stream.pack.super_.prototype.resume)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>setEncoding (enc)](#apidoc.element.tar-stream.pack.super_.prototype.setEncoding)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>unpipe (dest)](#apidoc.element.tar-stream.pack.super_.prototype.unpipe)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>unshift (chunk)](#apidoc.element.tar-stream.pack.super_.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>wrap (stream)](#apidoc.element.tar-stream.pack.super_.prototype.wrap)



# <a name="apidoc.module.tar-stream"></a>[module tar-stream](#apidoc.module.tar-stream)

#### <a name="apidoc.element.tar-stream.extract"></a>[function <span class="apidocSignatureSpan">tar-stream.</span>extract (opts)](#apidoc.element.tar-stream.extract)
- description and source-code
```javascript
extract = function (opts) {
  if (!(this instanceof Extract)) return new Extract(opts)
  Writable.call(this, opts)

  this._offset = 0
  this._buffer = bl()
  this._missing = 0
  this._onparse = noop
  this._header = null
  this._stream = null
  this._overflow = null
  this._cb = null
  this._locked = false
  this._destroyed = false
  this._pax = null
  this._paxGlobal = null
  this._gnuLongPath = null
  this._gnuLongLinkPath = null

  var self = this
  var b = self._buffer

  var oncontinue = function () {
    self._continue()
  }

  var onunlock = function (err) {
    self._locked = false
    if (err) return self.destroy(err)
    if (!self._stream) oncontinue()
  }

  var onstreamend = function () {
    self._stream = null
    var drain = overflow(self._header.size)
    if (drain) self._parse(drain, ondrain)
    else self._parse(512, onheader)
    if (!self._locked) oncontinue()
  }

  var ondrain = function () {
    self._buffer.consume(overflow(self._header.size))
    self._parse(512, onheader)
    oncontinue()
  }

  var onpaxglobalheader = function () {
    var size = self._header.size
    self._paxGlobal = headers.decodePax(b.slice(0, size))
    b.consume(size)
    onstreamend()
  }

  var onpaxheader = function () {
    var size = self._header.size
    self._pax = headers.decodePax(b.slice(0, size))
    if (self._paxGlobal) self._pax = xtend(self._paxGlobal, self._pax)
    b.consume(size)
    onstreamend()
  }

  var ongnulongpath = function () {
    var size = self._header.size
    this._gnuLongPath = headers.decodeLongPath(b.slice(0, size))
    b.consume(size)
    onstreamend()
  }

  var ongnulonglinkpath = function () {
    var size = self._header.size
    this._gnuLongLinkPath = headers.decodeLongPath(b.slice(0, size))
    b.consume(size)
    onstreamend()
  }

  var onheader = function () {
    var offset = self._offset
    var header
    try {
      header = self._header = headers.decode(b.slice(0, 512))
    } catch (err) {
      self.emit('error', err)
    }
    b.consume(512)

    if (!header) {
      self._parse(512, onheader)
      oncontinue()
      return
    }
    if (header.type === 'gnu-long-path') {
      self._parse(header.size, ongnulongpath)
      oncontinue()
      return
    }
    if (header.type === 'gnu-long-link-path') {
      self._parse(header.size, ongnulonglinkpath)
      oncontinue()
      return
    }
    if (header.type === 'pax-global-header') {
      self._parse(header.size, onpaxglobalheader)
      oncontinue()
      return
    }
    if (header.type === 'pax-header') {
      self._parse(header.size, onpaxheader)
      oncontinue()
      return
    }

    if (self._gnuLongPath) {
      header.name = self._gnuLongPath
      self._gnuLongPath = null
    }

    if (self._gnuLongLinkPath) {
      header.linkname = self._gnuLongLinkPath
      self._gnuLongLinkPath = null
    }

    if (self._pax) {
      self._header = header = mixinPax(header, self._pax)
      self._pax = null
    }

    self._locked = true

    if (!header.size) {
      self._parse(512, onheader)
      self.emit('entry', header, emptyStream(self, offset), onunlock)
      return
    }

    self._stream = new Source(self, offset)

    self.emit('entry', header, self._stream, onunlock)
    self._parse(header.size, onstreamend)
    oncontinue()
  }

  this._parse(512, onheader)
}
```
- example usage
```shell
...

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''

## Extracting

To extract a stream use 'tar.extract()' and listen for 'extract.on('entry', header, stream, callback)'

''' js
var extract = tar.extract()

extract.on('entry', function(header, stream, callback) {
// header is the tar header
// stream is the content body (might be an empty stream)
...
```

#### <a name="apidoc.element.tar-stream.extract.super_"></a>[function <span class="apidocSignatureSpan">tar-stream.</span>extract.super_ (options)](#apidoc.element.tar-stream.extract.super_)
- description and source-code
```javascript
function Writable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!realHasInstance.call(Writable, this) && !(this instanceof Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function') this._write = options.write;

    if (typeof options.writev === 'function') this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack"></a>[function <span class="apidocSignatureSpan">tar-stream.</span>pack (opts)](#apidoc.element.tar-stream.pack)
- description and source-code
```javascript
pack = function (opts) {
  if (!(this instanceof Pack)) return new Pack(opts)
  Readable.call(this, opts)

  this._drain = noop
  this._finalized = false
  this._finalizing = false
  this._destroyed = false
  this._stream = null
}
```
- example usage
```shell
...

## Related

If you want to pack/unpack directories on the file system check out [tar-fs](https://github.com/mafintosh/tar-fs) which provides
 file system bindings to this module.

## Packing

To create a pack stream use 'tar.pack()' and call 'pack.entry(header, [callback])' to add tar entries.

''' js
var tar = require('tar-stream')
var pack = tar.pack() // pack is a streams2 stream

// add a file called my-test.txt with the content "Hello World!"
pack.entry({ name: 'my-test.txt' }, 'Hello World!')
...
```

#### <a name="apidoc.element.tar-stream.pack.super_"></a>[function <span class="apidocSignatureSpan">tar-stream.</span>pack.super_ (options)](#apidoc.element.tar-stream.pack.super_)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.extract"></a>[module tar-stream.extract](#apidoc.module.tar-stream.extract)

#### <a name="apidoc.element.tar-stream.extract.extract"></a>[function <span class="apidocSignatureSpan">tar-stream.</span>extract (opts)](#apidoc.element.tar-stream.extract.extract)
- description and source-code
```javascript
extract = function (opts) {
  if (!(this instanceof Extract)) return new Extract(opts)
  Writable.call(this, opts)

  this._offset = 0
  this._buffer = bl()
  this._missing = 0
  this._onparse = noop
  this._header = null
  this._stream = null
  this._overflow = null
  this._cb = null
  this._locked = false
  this._destroyed = false
  this._pax = null
  this._paxGlobal = null
  this._gnuLongPath = null
  this._gnuLongLinkPath = null

  var self = this
  var b = self._buffer

  var oncontinue = function () {
    self._continue()
  }

  var onunlock = function (err) {
    self._locked = false
    if (err) return self.destroy(err)
    if (!self._stream) oncontinue()
  }

  var onstreamend = function () {
    self._stream = null
    var drain = overflow(self._header.size)
    if (drain) self._parse(drain, ondrain)
    else self._parse(512, onheader)
    if (!self._locked) oncontinue()
  }

  var ondrain = function () {
    self._buffer.consume(overflow(self._header.size))
    self._parse(512, onheader)
    oncontinue()
  }

  var onpaxglobalheader = function () {
    var size = self._header.size
    self._paxGlobal = headers.decodePax(b.slice(0, size))
    b.consume(size)
    onstreamend()
  }

  var onpaxheader = function () {
    var size = self._header.size
    self._pax = headers.decodePax(b.slice(0, size))
    if (self._paxGlobal) self._pax = xtend(self._paxGlobal, self._pax)
    b.consume(size)
    onstreamend()
  }

  var ongnulongpath = function () {
    var size = self._header.size
    this._gnuLongPath = headers.decodeLongPath(b.slice(0, size))
    b.consume(size)
    onstreamend()
  }

  var ongnulonglinkpath = function () {
    var size = self._header.size
    this._gnuLongLinkPath = headers.decodeLongPath(b.slice(0, size))
    b.consume(size)
    onstreamend()
  }

  var onheader = function () {
    var offset = self._offset
    var header
    try {
      header = self._header = headers.decode(b.slice(0, 512))
    } catch (err) {
      self.emit('error', err)
    }
    b.consume(512)

    if (!header) {
      self._parse(512, onheader)
      oncontinue()
      return
    }
    if (header.type === 'gnu-long-path') {
      self._parse(header.size, ongnulongpath)
      oncontinue()
      return
    }
    if (header.type === 'gnu-long-link-path') {
      self._parse(header.size, ongnulonglinkpath)
      oncontinue()
      return
    }
    if (header.type === 'pax-global-header') {
      self._parse(header.size, onpaxglobalheader)
      oncontinue()
      return
    }
    if (header.type === 'pax-header') {
      self._parse(header.size, onpaxheader)
      oncontinue()
      return
    }

    if (self._gnuLongPath) {
      header.name = self._gnuLongPath
      self._gnuLongPath = null
    }

    if (self._gnuLongLinkPath) {
      header.linkname = self._gnuLongLinkPath
      self._gnuLongLinkPath = null
    }

    if (self._pax) {
      self._header = header = mixinPax(header, self._pax)
      self._pax = null
    }

    self._locked = true

    if (!header.size) {
      self._parse(512, onheader)
      self.emit('entry', header, emptyStream(self, offset), onunlock)
      return
    }

    self._stream = new Source(self, offset)

    self.emit('entry', header, self._stream, onunlock)
    self._parse(header.size, onstreamend)
    oncontinue()
  }

  this._parse(512, onheader)
}
```
- example usage
```shell
...

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''

## Extracting

To extract a stream use 'tar.extract()' and listen for 'extract.on('entry', header, stream, callback)'

''' js
var extract = tar.extract()

extract.on('entry', function(header, stream, callback) {
// header is the tar header
// stream is the content body (might be an empty stream)
...
```

#### <a name="apidoc.element.tar-stream.extract.super_"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.</span>super_ (options)](#apidoc.element.tar-stream.extract.super_)
- description and source-code
```javascript
function Writable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!realHasInstance.call(Writable, this) && !(this instanceof Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function') this._write = options.write;

    if (typeof options.writev === 'function') this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.extract.prototype"></a>[module tar-stream.extract.prototype](#apidoc.module.tar-stream.extract.prototype)

#### <a name="apidoc.element.tar-stream.extract.prototype._continue"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.prototype.</span>_continue ()](#apidoc.element.tar-stream.extract.prototype._continue)
- description and source-code
```javascript
_continue = function () {
  if (this._destroyed) return
  var cb = this._cb
  this._cb = noop
  if (this._overflow) this._write(this._overflow, undefined, cb)
  else cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.extract.prototype._parse"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.prototype.</span>_parse (size, onparse)](#apidoc.element.tar-stream.extract.prototype._parse)
- description and source-code
```javascript
_parse = function (size, onparse) {
  if (this._destroyed) return
  this._offset += size
  this._missing = size
  this._onparse = onparse
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.extract.prototype._write"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.prototype.</span>_write (data, enc, cb)](#apidoc.element.tar-stream.extract.prototype._write)
- description and source-code
```javascript
_write = function (data, enc, cb) {
  if (this._destroyed) return

  var s = this._stream
  var b = this._buffer
  var missing = this._missing

  // we do not reach end-of-chunk now. just forward it

  if (data.length < missing) {
    this._missing -= data.length
    this._overflow = null
    if (s) return s.write(data, cb)
    b.append(data)
    return cb()
  }

  // end-of-chunk. the parser should call cb.

  this._cb = cb
  this._missing = 0

  var overflow = null
  if (data.length > missing) {
    overflow = data.slice(missing)
    data = data.slice(0, missing)
  }

  if (s) s.end(data)
  else b.append(data)

  this._overflow = overflow
  this._onparse()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.extract.prototype.destroy"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.prototype.</span>destroy (err)](#apidoc.element.tar-stream.extract.prototype.destroy)
- description and source-code
```javascript
destroy = function (err) {
  if (this._destroyed) return
  this._destroyed = true

  if (err) this.emit('error', err)
  this.emit('close')
  if (this._stream) this._stream.emit('close')
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.extract.super_"></a>[module tar-stream.extract.super_](#apidoc.module.tar-stream.extract.super_)

#### <a name="apidoc.element.tar-stream.extract.super_.super_"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.</span>super_ ()](#apidoc.element.tar-stream.extract.super_.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.extract.super_.WritableState"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.</span>WritableState (options, stream)](#apidoc.element.tar-stream.extract.super_.WritableState)
- description and source-code
```javascript
function WritableState(options, stream) {
  Duplex = Duplex || require('./_stream_duplex');

  options = options || {};

  // object stream flag to indicate whether or not this stream
  // contains buffers or objects.
  this.objectMode = !!options.objectMode;

  if (stream instanceof Duplex) this.objectMode = this.objectMode || !!options.writableObjectMode;

  // the point at which write() starts returning false
  // Note: 0 is a valid value, means that we always return false if
  // the entire buffer is not flushed immediately on write()
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = hwm || hwm === 0 ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  // drain event flag.
  this.needDrain = false;
  // at the start of calling end()
  this.ending = false;
  // when end() has been called, and returned
  this.ended = false;
  // when 'finish' is emitted
  this.finished = false;

  // should we decode strings into buffers before passing to _write?
  // this is here so that some node-core streams can optimize string
  // handling at a lower level.
  var noDecode = options.decodeStrings === false;
  this.decodeStrings = !noDecode;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // not an actual buffer we keep track of, but a measurement
  // of how much we're waiting to get pushed to some underlying
  // socket or file.
  this.length = 0;

  // a flag to see when we're in the middle of a write.
  this.writing = false;

  // when true all writes will be buffered until .uncork() call
  this.corked = 0;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // a flag to know if we're processing previously buffered items, which
  // may call the _write() callback in the same tick, so that we don't
  // end up in an overlapped onwrite situation.
  this.bufferProcessing = false;

  // the callback that's passed to _write(chunk,cb)
  this.onwrite = function (er) {
    onwrite(stream, er);
  };

  // the callback that the user supplies to write(chunk,encoding,cb)
  this.writecb = null;

  // the amount that is being written when _write is called.
  this.writelen = 0;

  this.bufferedRequest = null;
  this.lastBufferedRequest = null;

  // number of pending user-supplied write callbacks
  // this must be 0 before 'finish' can be emitted
  this.pendingcb = 0;

  // emit prefinish if the only thing we're waiting for is _write cbs
  // This is relevant for synchronous Transform streams
  this.prefinished = false;

  // True if the error was already emitted and should not be thrown again
  this.errorEmitted = false;

  // count buffered requests
  this.bufferedRequestCount = 0;

  // allocate the first CorkedRequest, there is always
  // one allocated and free to use, and we maintain at most two
  this.corkedRequestsFree = new CorkedRequest(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.extract.super_.WritableState.prototype"></a>[module tar-stream.extract.super_.WritableState.prototype](#apidoc.module.tar-stream.extract.super_.WritableState.prototype)

#### <a name="apidoc.element.tar-stream.extract.super_.WritableState.prototype.getBuffer"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.WritableState.prototype.</span>getBuffer ()](#apidoc.element.tar-stream.extract.super_.WritableState.prototype.getBuffer)
- description and source-code
```javascript
function getBuffer() {
  var current = this.bufferedRequest;
  var out = [];
  while (current) {
    out.push(current);
    current = current.next;
  }
  return out;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.extract.super_.prototype"></a>[module tar-stream.extract.super_.prototype](#apidoc.module.tar-stream.extract.super_.prototype)

#### <a name="apidoc.element.tar-stream.extract.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.tar-stream.extract.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('_write() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.extract.super_.prototype.cork"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>cork ()](#apidoc.element.tar-stream.extract.super_.prototype.cork)
- description and source-code
```javascript
cork = function () {
  var state = this._writableState;

  state.corked++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.extract.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.tar-stream.extract.super_.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (chunk !== null && chunk !== undefined) this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished) endWritable(this, state, cb);
}
```
- example usage
```shell
...
  // no more entries
  pack.finalize()
})

entry.write('hello')
entry.write(' ')
entry.write('world')
entry.end()

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''

## Extracting
...
```

#### <a name="apidoc.element.tar-stream.extract.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>pipe ()](#apidoc.element.tar-stream.extract.super_.prototype.pipe)
- description and source-code
```javascript
pipe = function () {
  this.emit('error', new Error('Cannot pipe, not readable'));
}
```
- example usage
```shell
...

entry.write('hello')
entry.write(' ')
entry.write('world')
entry.end()

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''

## Extracting

To extract a stream use 'tar.extract()' and listen for 'extract.on('entry', header, stream, callback)'

''' js
...
```

#### <a name="apidoc.element.tar-stream.extract.super_.prototype.setDefaultEncoding"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.tar-stream.extract.super_.prototype.setDefaultEncoding)
- description and source-code
```javascript
function setDefaultEncoding(encoding) {
  // node::ParseEncoding() requires lower case.
  if (typeof encoding === 'string') encoding = encoding.toLowerCase();
  if (!(['hex', 'utf8', 'utf-8', 'ascii', 'binary', 'base64', 'ucs2', 'ucs-2', 'utf16le', 'utf-16le', 'raw'].indexOf((encoding + '').
toLowerCase()) > -1)) throw new TypeError('Unknown encoding: ' + encoding);
  this._writableState.defaultEncoding = encoding;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.extract.super_.prototype.uncork"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>uncork ()](#apidoc.element.tar-stream.extract.super_.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  var state = this._writableState;

  if (state.corked) {
    state.corked--;

    if (!state.writing && !state.corked && !state.finished && !state.bufferProcessing && state.bufferedRequest) clearBuffer(this
, state);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.extract.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">tar-stream.extract.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.tar-stream.extract.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;
  var isBuf = Buffer.isBuffer(chunk);

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (isBuf) encoding = 'buffer';else if (!encoding) encoding = state.defaultEncoding;

  if (typeof cb !== 'function') cb = nop;

  if (state.ended) writeAfterEnd(this, cb);else if (isBuf || validChunk(this, state, chunk, cb)) {
    state.pendingcb++;
    ret = writeOrBuffer(this, state, isBuf, chunk, encoding, cb);
  }

  return ret;
}
```
- example usage
```shell
...
// add a file called my-stream-test.txt from a stream
var entry = pack.entry({ name: 'my-stream-test.txt', size: 11 }, function(err) {
  // the stream was added
  // no more entries
  pack.finalize()
})

entry.write('hello')
entry.write(' ')
entry.write('world')
entry.end()

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''
...
```



# <a name="apidoc.module.tar-stream.headers"></a>[module tar-stream.headers](#apidoc.module.tar-stream.headers)

#### <a name="apidoc.element.tar-stream.headers.decode"></a>[function <span class="apidocSignatureSpan">tar-stream.headers.</span>decode (buf)](#apidoc.element.tar-stream.headers.decode)
- description and source-code
```javascript
decode = function (buf) {
  var typeflag = buf[156] === 0 ? 0 : buf[156] - ZERO_OFFSET

  var name = decodeStr(buf, 0, 100)
  var mode = decodeOct(buf, 100)
  var uid = decodeOct(buf, 108)
  var gid = decodeOct(buf, 116)
  var size = decodeOct(buf, 124)
  var mtime = decodeOct(buf, 136)
  var type = toType(typeflag)
  var linkname = buf[157] === 0 ? null : decodeStr(buf, 157, 100)
  var uname = decodeStr(buf, 265, 32)
  var gname = decodeStr(buf, 297, 32)
  var devmajor = decodeOct(buf, 329)
  var devminor = decodeOct(buf, 337)

  if (buf[345]) name = decodeStr(buf, 345, 155) + '/' + name

  // to support old tar versions that use trailing / to indicate dirs
  if (typeflag === 0 && name && name[name.length - 1] === '/') typeflag = 5

  var c = cksum(buf)

  // checksum is still initial value if header was null.
  if (c === 8 * 32) return null

  // valid checksum
  if (c !== decodeOct(buf, 148)) throw new Error('Invalid tar header. Maybe the tar is corrupted or it needs to be gunzipped?')

  return {
    name: name,
    mode: mode,
    uid: uid,
    gid: gid,
    size: size,
    mtime: new Date(1000 * mtime),
    type: type,
    linkname: linkname,
    uname: uname,
    gname: gname,
    devmajor: devmajor,
    devminor: devminor
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.headers.decodeLongPath"></a>[function <span class="apidocSignatureSpan">tar-stream.headers.</span>decodeLongPath (buf)](#apidoc.element.tar-stream.headers.decodeLongPath)
- description and source-code
```javascript
decodeLongPath = function (buf) {
  return decodeStr(buf, 0, buf.length)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.headers.decodePax"></a>[function <span class="apidocSignatureSpan">tar-stream.headers.</span>decodePax (buf)](#apidoc.element.tar-stream.headers.decodePax)
- description and source-code
```javascript
decodePax = function (buf) {
  var result = {}

  while (buf.length) {
    var i = 0
    while (i < buf.length && buf[i] !== 32) i++
    var len = parseInt(buf.slice(0, i).toString(), 10)
    if (!len) return result

    var b = buf.slice(i + 1, len - 1).toString()
    var keyIndex = b.indexOf('=')
    if (keyIndex === -1) return result
    result[b.slice(0, keyIndex)] = b.slice(keyIndex + 1)

    buf = buf.slice(len)
  }

  return result
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.headers.encode"></a>[function <span class="apidocSignatureSpan">tar-stream.headers.</span>encode (opts)](#apidoc.element.tar-stream.headers.encode)
- description and source-code
```javascript
encode = function (opts) {
  var buf = alloc(512)
  var name = opts.name
  var prefix = ''

  if (opts.typeflag === 5 && name[name.length - 1] !== '/') name += '/'
  if (Buffer.byteLength(name) !== name.length) return null // utf-8

  while (Buffer.byteLength(name) > 100) {
    var i = name.indexOf('/')
    if (i === -1) return null
    prefix += prefix ? '/' + name.slice(0, i) : name.slice(0, i)
    name = name.slice(i + 1)
  }

  if (Buffer.byteLength(name) > 100 || Buffer.byteLength(prefix) > 155) return null
  if (opts.linkname && Buffer.byteLength(opts.linkname) > 100) return null

  buf.write(name)
  buf.write(encodeOct(opts.mode & MASK, 6), 100)
  buf.write(encodeOct(opts.uid, 6), 108)
  buf.write(encodeOct(opts.gid, 6), 116)
  buf.write(encodeOct(opts.size, 11), 124)
  buf.write(encodeOct((opts.mtime.getTime() / 1000) | 0, 11), 136)

  buf[156] = ZERO_OFFSET + toTypeflag(opts.type)

  if (opts.linkname) buf.write(opts.linkname, 157)

  buf.write(USTAR, 257)
  if (opts.uname) buf.write(opts.uname, 265)
  if (opts.gname) buf.write(opts.gname, 297)
  buf.write(encodeOct(opts.devmajor || 0, 6), 329)
  buf.write(encodeOct(opts.devminor || 0, 6), 337)

  if (prefix) buf.write(prefix, 345)

  buf.write(encodeOct(cksum(buf), 6), 148)

  return buf
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.headers.encodePax"></a>[function <span class="apidocSignatureSpan">tar-stream.headers.</span>encodePax (opts)](#apidoc.element.tar-stream.headers.encodePax)
- description and source-code
```javascript
encodePax = function (opts) { // TODO: encode more stuff in pax
  var result = ''
  if (opts.name) result += addLength(' path=' + opts.name + '\n')
  if (opts.linkname) result += addLength(' linkpath=' + opts.linkname + '\n')
  var pax = opts.pax
  if (pax) {
    for (var key in pax) {
      result += addLength(' ' + key + '=' + pax[key] + '\n')
    }
  }
  return new Buffer(result)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.pack"></a>[module tar-stream.pack](#apidoc.module.tar-stream.pack)

#### <a name="apidoc.element.tar-stream.pack.pack"></a>[function <span class="apidocSignatureSpan">tar-stream.</span>pack (opts)](#apidoc.element.tar-stream.pack.pack)
- description and source-code
```javascript
pack = function (opts) {
  if (!(this instanceof Pack)) return new Pack(opts)
  Readable.call(this, opts)

  this._drain = noop
  this._finalized = false
  this._finalizing = false
  this._destroyed = false
  this._stream = null
}
```
- example usage
```shell
...

## Related

If you want to pack/unpack directories on the file system check out [tar-fs](https://github.com/mafintosh/tar-fs) which provides
 file system bindings to this module.

## Packing

To create a pack stream use 'tar.pack()' and call 'pack.entry(header, [callback])' to add tar entries.

''' js
var tar = require('tar-stream')
var pack = tar.pack() // pack is a streams2 stream

// add a file called my-test.txt with the content "Hello World!"
pack.entry({ name: 'my-test.txt' }, 'Hello World!')
...
```

#### <a name="apidoc.element.tar-stream.pack.super_"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.</span>super_ (options)](#apidoc.element.tar-stream.pack.super_)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.pack.prototype"></a>[module tar-stream.pack.prototype](#apidoc.module.tar-stream.pack.prototype)

#### <a name="apidoc.element.tar-stream.pack.prototype._encode"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>_encode (header)](#apidoc.element.tar-stream.pack.prototype._encode)
- description and source-code
```javascript
_encode = function (header) {
  if (!header.pax) {
    var buf = headers.encode(header)
    if (buf) {
      this.push(buf)
      return
    }
  }
  this._encodePax(header)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.prototype._encodePax"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>_encodePax (header)](#apidoc.element.tar-stream.pack.prototype._encodePax)
- description and source-code
```javascript
_encodePax = function (header) {
  var paxHeader = headers.encodePax({
    name: header.name,
    linkname: header.linkname,
    pax: header.pax
  })

  var newHeader = {
    name: 'PaxHeader',
    mode: header.mode,
    uid: header.uid,
    gid: header.gid,
    size: paxHeader.length,
    mtime: header.mtime,
    type: 'pax-header',
    linkname: header.linkname && 'PaxHeader',
    uname: header.uname,
    gname: header.gname,
    devmajor: header.devmajor,
    devminor: header.devminor
  }

  this.push(headers.encode(newHeader))
  this.push(paxHeader)
  overflow(this, paxHeader.length)

  newHeader.size = header.size
  newHeader.type = header.type
  this.push(headers.encode(newHeader))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.prototype._read"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>_read (n)](#apidoc.element.tar-stream.pack.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  var drain = this._drain
  this._drain = noop
  drain()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.prototype.destroy"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>destroy (err)](#apidoc.element.tar-stream.pack.prototype.destroy)
- description and source-code
```javascript
destroy = function (err) {
  if (this._destroyed) return
  this._destroyed = true

  if (err) this.emit('error', err)
  this.emit('close')
  if (this._stream && this._stream.destroy) this._stream.destroy()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.prototype.entry"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>entry (header, buffer, callback)](#apidoc.element.tar-stream.pack.prototype.entry)
- description and source-code
```javascript
entry = function (header, buffer, callback) {
  if (this._stream) throw new Error('already piping an entry')
  if (this._finalized || this._destroyed) return

  if (typeof buffer === 'function') {
    callback = buffer
    buffer = null
  }

  if (!callback) callback = noop

  var self = this

  if (!header.size || header.type === 'symlink') header.size = 0
  if (!header.type) header.type = modeToType(header.mode)
  if (!header.mode) header.mode = header.type === 'directory' ? DMODE : FMODE
  if (!header.uid) header.uid = 0
  if (!header.gid) header.gid = 0
  if (!header.mtime) header.mtime = new Date()

  if (typeof buffer === 'string') buffer = new Buffer(buffer)
  if (Buffer.isBuffer(buffer)) {
    header.size = buffer.length
    this._encode(header)
    this.push(buffer)
    overflow(self, header.size)
    process.nextTick(callback)
    return new Void()
  }

  if (header.type === 'symlink' && !header.linkname) {
    var linkSink = new LinkSink()
    eos(linkSink, function (err) {
      if (err) { // stream was closed
        self.destroy()
        return callback(err)
      }

      header.linkname = linkSink.linkname
      self._encode(header)
      callback()
    })

    return linkSink
  }

  this._encode(header)

  if (header.type !== 'file' && header.type !== 'contiguous-file') {
    process.nextTick(callback)
    return new Void()
  }

  var sink = new Sink(this)

  this._stream = sink

  eos(sink, function (err) {
    self._stream = null

    if (err) { // stream was closed
      self.destroy()
      return callback(err)
    }

    if (sink.written !== header.size) { // corrupting tar
      self.destroy()
      return callback(new Error('size mismatch'))
    }

    overflow(self, header.size)
    if (self._finalizing) self.finalize()
    callback()
  })

  return sink
}
```
- example usage
```shell
...

## Related

If you want to pack/unpack directories on the file system check out [tar-fs](https://github.com/mafintosh/tar-fs) which provides
 file system bindings to this module.

## Packing

To create a pack stream use 'tar.pack()' and call 'pack.entry(header, [callback])' to add tar entries.

''' js
var tar = require('tar-stream')
var pack = tar.pack() // pack is a streams2 stream

// add a file called my-test.txt with the content "Hello World!"
pack.entry({ name: 'my-test.txt' }, 'Hello World!')
...
```

#### <a name="apidoc.element.tar-stream.pack.prototype.finalize"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.prototype.</span>finalize ()](#apidoc.element.tar-stream.pack.prototype.finalize)
- description and source-code
```javascript
finalize = function () {
  if (this._stream) {
    this._finalizing = true
    return
  }

  if (this._finalized) return
  this._finalized = true
  this.push(END_OF_TAR)
  this.push(null)
}
```
- example usage
```shell
...
// add a file called my-test.txt with the content "Hello World!"
pack.entry({ name: 'my-test.txt' }, 'Hello World!')

// add a file called my-stream-test.txt from a stream
var entry = pack.entry({ name: 'my-stream-test.txt', size: 11 }, function(err) {
  // the stream was added
  // no more entries
  pack.finalize()
})

entry.write('hello')
entry.write(' ')
entry.write('world')
entry.end()
...
```



# <a name="apidoc.module.tar-stream.pack.super_"></a>[module tar-stream.pack.super_](#apidoc.module.tar-stream.pack.super_)

#### <a name="apidoc.element.tar-stream.pack.super_.super_"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.</span>super_ ()](#apidoc.element.tar-stream.pack.super_.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Duplex"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Duplex (options)](#apidoc.element.tar-stream.pack.super_.Duplex)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex)) return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false) this.readable = false;

  if (options && options.writable === false) this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false) this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.PassThrough"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>PassThrough (options)](#apidoc.element.tar-stream.pack.super_.PassThrough)
- description and source-code
```javascript
function PassThrough(options) {
  if (!(this instanceof PassThrough)) return new PassThrough(options);

  Transform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Readable"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Readable (options)](#apidoc.element.tar-stream.pack.super_.Readable)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.ReadableState"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>ReadableState (options, stream)](#apidoc.element.tar-stream.pack.super_.ReadableState)
- description and source-code
```javascript
function ReadableState(options, stream) {
  Duplex = Duplex || require('./_stream_duplex');

  options = options || {};

  // object stream flag. Used to make read(n) ignore n and to
  // make all the buffer merging and length checks go away
  this.objectMode = !!options.objectMode;

  if (stream instanceof Duplex) this.objectMode = this.objectMode || !!options.readableObjectMode;

  // the point at which it stops calling _read() to fill the buffer
  // Note: 0 is a valid value, means "don't call _read preemptively ever"
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = hwm || hwm === 0 ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  // A linked list is used to store data chunks instead of an array because the
  // linked list can remove elements from the beginning faster than
  // array.shift()
  this.buffer = new BufferList();
  this.length = 0;
  this.pipes = null;
  this.pipesCount = 0;
  this.flowing = null;
  this.ended = false;
  this.endEmitted = false;
  this.reading = false;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // whenever we return null, then we set a flag to say
  // that we're awaiting a 'readable' event emission.
  this.needReadable = false;
  this.emittedReadable = false;
  this.readableListening = false;
  this.resumeScheduled = false;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // when piping, we only care about 'readable' events that happen
  // after read()ing all the bytes and not getting any pushback.
  this.ranOut = false;

  // the number of writers that are awaiting a drain event in .pipe()s
  this.awaitDrain = 0;

  // if true, a maybeReadMore has been scheduled
  this.readingMore = false;

  this.decoder = null;
  this.encoding = null;
  if (options.encoding) {
    if (!StringDecoder) StringDecoder = require('string_decoder/').StringDecoder;
    this.decoder = new StringDecoder(options.encoding);
    this.encoding = options.encoding;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Stream"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Stream ()](#apidoc.element.tar-stream.pack.super_.Stream)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Transform"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Transform (options)](#apidoc.element.tar-stream.pack.super_.Transform)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  // When the writable side finishes, then flush out anything remaining.
  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er, data) {
      done(stream, er, data);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Writable"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>Writable (options)](#apidoc.element.tar-stream.pack.super_.Writable)
- description and source-code
```javascript
function Writable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!realHasInstance.call(Writable, this) && !(this instanceof Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function') this._write = options.write;

    if (typeof options.writev === 'function') this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_._fromList"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.</span>_fromList (n, state)](#apidoc.element.tar-stream.pack.super_._fromList)
- description and source-code
```javascript
function fromList(n, state) {
  // nothing buffered
  if (state.length === 0) return null;

  var ret;
  if (state.objectMode) ret = state.buffer.shift();else if (!n || n >= state.length) {
    // read it all, truncate the list
    if (state.decoder) ret = state.buffer.join('');else if (state.buffer.length === 1) ret = state.buffer.head.data;else ret = state
.buffer.concat(state.length);
    state.buffer.clear();
  } else {
    // read part of list
    ret = fromListPartial(n, state.buffer, state.decoder);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.pack.super_.Duplex.prototype"></a>[module tar-stream.pack.super_.Duplex.prototype](#apidoc.module.tar-stream.pack.super_.Duplex.prototype)

#### <a name="apidoc.element.tar-stream.pack.super_.Duplex.prototype._write"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Duplex.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('_write() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Duplex.prototype.cork"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>cork ()](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.cork)
- description and source-code
```javascript
cork = function () {
  var state = this._writableState;

  state.corked++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Duplex.prototype.end"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (chunk !== null && chunk !== undefined) this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished) endWritable(this, state, cb);
}
```
- example usage
```shell
...
  // no more entries
  pack.finalize()
})

entry.write('hello')
entry.write(' ')
entry.write('world')
entry.end()

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''

## Extracting
...
```

#### <a name="apidoc.element.tar-stream.pack.super_.Duplex.prototype.setDefaultEncoding"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.setDefaultEncoding)
- description and source-code
```javascript
function setDefaultEncoding(encoding) {
  // node::ParseEncoding() requires lower case.
  if (typeof encoding === 'string') encoding = encoding.toLowerCase();
  if (!(['hex', 'utf8', 'utf-8', 'ascii', 'binary', 'base64', 'ucs2', 'ucs-2', 'utf16le', 'utf-16le', 'raw'].indexOf((encoding + '').
toLowerCase()) > -1)) throw new TypeError('Unknown encoding: ' + encoding);
  this._writableState.defaultEncoding = encoding;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Duplex.prototype.uncork"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>uncork ()](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  var state = this._writableState;

  if (state.corked) {
    state.corked--;

    if (!state.writing && !state.corked && !state.finished && !state.bufferProcessing && state.bufferedRequest) clearBuffer(this
, state);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Duplex.prototype.write"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Duplex.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Duplex.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;
  var isBuf = Buffer.isBuffer(chunk);

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (isBuf) encoding = 'buffer';else if (!encoding) encoding = state.defaultEncoding;

  if (typeof cb !== 'function') cb = nop;

  if (state.ended) writeAfterEnd(this, cb);else if (isBuf || validChunk(this, state, chunk, cb)) {
    state.pendingcb++;
    ret = writeOrBuffer(this, state, isBuf, chunk, encoding, cb);
  }

  return ret;
}
```
- example usage
```shell
...
// add a file called my-stream-test.txt from a stream
var entry = pack.entry({ name: 'my-stream-test.txt', size: 11 }, function(err) {
  // the stream was added
  // no more entries
  pack.finalize()
})

entry.write('hello')
entry.write(' ')
entry.write('world')
entry.end()

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''
...
```



# <a name="apidoc.module.tar-stream.pack.super_.PassThrough.prototype"></a>[module tar-stream.pack.super_.PassThrough.prototype](#apidoc.module.tar-stream.pack.super_.PassThrough.prototype)

#### <a name="apidoc.element.tar-stream.pack.super_.PassThrough.prototype._transform"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.PassThrough.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.PassThrough.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, cb) {
  cb(null, chunk);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tar-stream.pack.super_.Transform.prototype"></a>[module tar-stream.pack.super_.Transform.prototype](#apidoc.module.tar-stream.pack.super_.Transform.prototype)

#### <a name="apidoc.element.tar-stream.pack.super_.Transform.prototype._read"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Transform.prototype.</span>_read (n)](#apidoc.element.tar-stream.pack.super_.Transform.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  var ts = this._transformState;

  if (ts.writechunk !== null && ts.writecb && !ts.transforming) {
    ts.transforming = true;
    this._transform(ts.writechunk, ts.writeencoding, ts.afterTransform);
  } else {
    // mark that we need a transform, so that any data that comes in
    // will get processed, now that we've asked for it.
    ts.needTransform = true;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Transform.prototype._transform"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Transform.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Transform.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, cb) {
  throw new Error('_transform() is not implemented');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Transform.prototype._write"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Transform.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.tar-stream.pack.super_.Transform.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  var ts = this._transformState;
  ts.writecb = cb;
  ts.writechunk = chunk;
  ts.writeencoding = encoding;
  if (!ts.transforming) {
    var rs = this._readableState;
    if (ts.needTransform || rs.needReadable || rs.length < rs.highWaterMark) this._read(rs.highWaterMark);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.Transform.prototype.push"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.Transform.prototype.</span>push (chunk, encoding)](#apidoc.element.tar-stream.pack.super_.Transform.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  this._transformState.needTransform = false;
  return Duplex.prototype.push.call(this, chunk, encoding);
}
```
- example usage
```shell
...
else return null

// build up a base-256 tuple from the least sig to the highest
var zero = false
var tuple = []
for (var i = buf.length - 1; i > 0; i--) {
  var byte = buf[i]
  if (positive) tuple.push(byte)
  else if (zero && byte === 0) tuple.push(0)
  else if (zero) {
    zero = false
    tuple.push(0x100 - byte)
  } else tuple.push(0xFF - byte)
}
...
```



# <a name="apidoc.module.tar-stream.pack.super_.prototype"></a>[module tar-stream.pack.super_.prototype](#apidoc.module.tar-stream.pack.super_.prototype)

#### <a name="apidoc.element.tar-stream.pack.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>_read (n)](#apidoc.element.tar-stream.pack.super_.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  this.emit('error', new Error('_read() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>addListener (ev, fn)](#apidoc.element.tar-stream.pack.super_.prototype.addListener)
- description and source-code
```javascript
addListener = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data') {
    // Start flowing on next tick if stream isn't explicitly paused
    if (this._readableState.flowing !== false) this.resume();
  } else if (ev === 'readable') {
    var state = this._readableState;
    if (!state.endEmitted && !state.readableListening) {
      state.readableListening = state.needReadable = true;
      state.emittedReadable = false;
      if (!state.reading) {
        processNextTick(nReadingNextTick, this);
      } else if (state.length) {
        emitReadable(this, state);
      }
    }
  }

  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.isPaused"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>isPaused ()](#apidoc.element.tar-stream.pack.super_.prototype.isPaused)
- description and source-code
```javascript
isPaused = function () {
  return this._readableState.flowing === false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>on (ev, fn)](#apidoc.element.tar-stream.pack.super_.prototype.on)
- description and source-code
```javascript
on = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data') {
    // Start flowing on next tick if stream isn't explicitly paused
    if (this._readableState.flowing !== false) this.resume();
  } else if (ev === 'readable') {
    var state = this._readableState;
    if (!state.endEmitted && !state.readableListening) {
      state.readableListening = state.needReadable = true;
      state.emittedReadable = false;
      if (!state.reading) {
        processNextTick(nReadingNextTick, this);
      } else if (state.length) {
        emitReadable(this, state);
      }
    }
  }

  return res;
}
```
- example usage
```shell
...

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''

## Extracting

To extract a stream use 'tar.extract()' and listen for 'extract.on('entry', header, stream, callback)'

''' js
var extract = tar.extract()

extract.on('entry', function(header, stream, callback) {
// header is the tar header
// stream is the content body (might be an empty stream)
...
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.pause"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>pause ()](#apidoc.element.tar-stream.pack.super_.prototype.pause)
- description and source-code
```javascript
pause = function () {
  debug('call pause flowing=%j', this._readableState.flowing);
  if (false !== this._readableState.flowing) {
    debug('pause');
    this._readableState.flowing = false;
    this.emit('pause');
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.tar-stream.pack.super_.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest, pipeOpts) {
  var src = this;
  var state = this._readableState;

  switch (state.pipesCount) {
    case 0:
      state.pipes = dest;
      break;
    case 1:
      state.pipes = [state.pipes, dest];
      break;
    default:
      state.pipes.push(dest);
      break;
  }
  state.pipesCount += 1;
  debug('pipe count=%d opts=%j', state.pipesCount, pipeOpts);

  var doEnd = (!pipeOpts || pipeOpts.end !== false) && dest !== process.stdout && dest !== process.stderr;

  var endFn = doEnd ? onend : cleanup;
  if (state.endEmitted) processNextTick(endFn);else src.once('end', endFn);

  dest.on('unpipe', onunpipe);
  function onunpipe(readable) {
    debug('onunpipe');
    if (readable === src) {
      cleanup();
    }
  }

  function onend() {
    debug('onend');
    dest.end();
  }

  // when the dest drains, it reduces the awaitDrain counter
  // on the source.  This would be more elegant with a .once()
  // handler in flow(), but adding and removing repeatedly is
  // too slow.
  var ondrain = pipeOnDrain(src);
  dest.on('drain', ondrain);

  var cleanedUp = false;
  function cleanup() {
    debug('cleanup');
    // cleanup event handlers once the pipe is broken
    dest.removeListener('close', onclose);
    dest.removeListener('finish', onfinish);
    dest.removeListener('drain', ondrain);
    dest.removeListener('error', onerror);
    dest.removeListener('unpipe', onunpipe);
    src.removeListener('end', onend);
    src.removeListener('end', cleanup);
    src.removeListener('data', ondata);

    cleanedUp = true;

    // if the reader is waiting for a drain event from this
    // specific writer, then it would cause it to never start
    // flowing again.
    // So, if this is awaiting a drain, then we just call it now.
    // If we don't know, then assume that we are waiting for one.
    if (state.awaitDrain && (!dest._writableState || dest._writableState.needDrain)) ondrain();
  }

  // If the user pushes more data while we're writing to dest then we'll end up
  // in ondata again. However, we only want to increase awaitDrain once because
  // dest will only emit one 'drain' event for the multiple writes.
  // => Introduce a guard on increasing awaitDrain.
  var increasedAwaitDrain = false;
  src.on('data', ondata);
  function ondata(chunk) {
    debug('ondata');
    increasedAwaitDrain = false;
    var ret = dest.write(chunk);
    if (false === ret && !increasedAwaitDrain) {
      // If the user unpiped during 'dest.write()', it is possible
      // to get stuck in a permanently paused state if that write
      // also returned false.
      // => Check whether 'dest' is still a piping destination.
      if ((state.pipesCount === 1 && state.pipes === dest || state.pipesCount > 1 && indexOf(state.pipes, dest) !== -1) && !cleanedUp
) {
        debug('false write response, pause', src._readableState.awaitDrain);
        src._readableState.awaitDrain++;
        increasedAwaitDrain = true;
      }
      src.pause();
    }
  }

  // if the dest has an error, then stop piping into it.
  // however, don't suppress the throwing behavior for this.
  function onerror(er) {
    debug('onerror', er);
    unpipe();
    dest.removeListener('error', onerror);
    if (EElistenerCount(dest, 'error') === 0) dest.emit('error', er);
  }

  // Make sure our error handler is attached before userland ones.
  prependListener(dest, 'error', onerror);

  // Both close and finish should trigger unpipe, but only once.
  function onclose() {
    dest.removeListener('finish', onfinish);
    unpipe();
  }
  dest.once('close', onclose);
  function onfinish() {
    debug('onfinish');
    dest.removeListener('close', onclose);
    unpipe();
  }
  dest.once('finish', onfinish);

  function unpipe() {
    debug('unpipe');
    src.unpipe(dest);
  }

  // tell the dest that it's being piped to
  dest.emit('pipe', src);

  // start the flow if it hasn't been started already.
  if (!state.flowing) {
    debug('pipe resume');
    src.resume();
  }

  return dest;
}
```
- example usage
```shell
...

entry.write('hello')
entry.write(' ')
entry.write('world')
entry.end()

// pipe the pack stream somewhere
pack.pipe(process.stdout)
'''

## Extracting

To extract a stream use 'tar.extract()' and listen for 'extract.on('entry', header, stream, callback)'

''' js
...
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.push"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.tar-stream.pack.super_.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  var state = this._readableState;

  if (!state.objectMode && typeof chunk === 'string') {
    encoding = encoding || state.defaultEncoding;
    if (encoding !== state.encoding) {
      chunk = bufferShim.from(chunk, encoding);
      encoding = '';
    }
  }

  return readableAddChunk(this, state, chunk, encoding, false);
}
```
- example usage
```shell
...
else return null

// build up a base-256 tuple from the least sig to the highest
var zero = false
var tuple = []
for (var i = buf.length - 1; i > 0; i--) {
  var byte = buf[i]
  if (positive) tuple.push(byte)
  else if (zero && byte === 0) tuple.push(0)
  else if (zero) {
    zero = false
    tuple.push(0x100 - byte)
  } else tuple.push(0xFF - byte)
}
...
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.read"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>read (n)](#apidoc.element.tar-stream.pack.super_.prototype.read)
- description and source-code
```javascript
read = function (n) {
  debug('read', n);
  n = parseInt(n, 10);
  var state = this._readableState;
  var nOrig = n;

  if (n !== 0) state.emittedReadable = false;

  // if we're doing read(0) to trigger a readable event, but we
  // already have a bunch of data in the buffer, then just trigger
  // the 'readable' event and move on.
  if (n === 0 && state.needReadable && (state.length >= state.highWaterMark || state.ended)) {
    debug('read: emitReadable', state.length, state.ended);
    if (state.length === 0 && state.ended) endReadable(this);else emitReadable(this);
    return null;
  }

  n = howMuchToRead(n, state);

  // if we've ended, and we're now clear, then finish it up.
  if (n === 0 && state.ended) {
    if (state.length === 0) endReadable(this);
    return null;
  }

  // All the actual chunk generation logic needs to be
  // *below* the call to _read.  The reason is that in certain
  // synthetic stream cases, such as passthrough streams, _read
  // may be a completely synchronous operation which may change
  // the state of the read buffer, providing enough data when
  // before there was *not* enough.
  //
  // So, the steps are:
  // 1. Figure out what the state of things will be after we do
  // a read from the buffer.
  //
  // 2. If that resulting state will trigger a _read, then call _read.
  // Note that this may be asynchronous, or synchronous.  Yes, it is
  // deeply ugly to write APIs this way, but that still doesn't mean
  // that the Readable class should behave improperly, as streams are
  // designed to be sync/async agnostic.
  // Take note if the _read call is sync or async (ie, if the read call
  // has returned yet), so that we know whether or not it's safe to emit
  // 'readable' etc.
  //
  // 3. Actually pull the requested chunks out of the buffer and return.

  // if we need a readable event, then we need to do some reading.
  var doRead = state.needReadable;
  debug('need readable', doRead);

  // if we currently have less than the highWaterMark, then also read some
  if (state.length === 0 || state.length - n < state.highWaterMark) {
    doRead = true;
    debug('length less than watermark', doRead);
  }

  // however, if we've ended, then there's no point, and if we're already
  // reading, then it's unnecessary.
  if (state.ended || state.reading) {
    doRead = false;
    debug('reading or ended', doRead);
  } else if (doRead) {
    debug('do read');
    state.reading = true;
    state.sync = true;
    // if the length is currently zero, then we *need* a readable event.
    if (state.length === 0) state.needReadable = true;
    // call internal read method
    this._read(state.highWaterMark);
    state.sync = false;
    // If _read pushed data synchronously, then 'reading' will be false,
    // and we need to re-evaluate how much data we can return to the user.
    if (!state.reading) n = howMuchToRead(nOrig, state);
  }

  var ret;
  if (n > 0) ret = fromList(n, state);else ret = null;

  if (ret === null) {
    state.needReadable = true;
    n = 0;
  } else {
    state.length -= n;
  }

  if (state.length === 0) {
    // If we have nothing in the buffer, then we want to know
    // as soon as we *do* get something into the buffer.
    if (!state.ended) state.needReadable = true;

    // If we tried to read() past the EOF, then emit end on the next tick.
    if (nOrig !== n && state.ended) endReadable(this);
  }

  if (ret !== null) this.emit('data', ret);

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.resume"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>resume ()](#apidoc.element.tar-stream.pack.super_.prototype.resume)
- description and source-code
```javascript
resume = function () {
  var state = this._readableState;
  if (!state.flowing) {
    debug('resume');
    state.flowing = true;
    resume(this, state);
  }
  return this;
}
```
- example usage
```shell
...
  // stream is the content body (might be an empty stream)
  // call next when you are done with this entry

  stream.on('end', function() {
    callback() // ready for next entry
  })

  stream.resume() // just auto drain the stream
})

extract.on('finish', function() {
  // all entries read
})

pack.pipe(extract)
...
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.setEncoding"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>setEncoding (enc)](#apidoc.element.tar-stream.pack.super_.prototype.setEncoding)
- description and source-code
```javascript
setEncoding = function (enc) {
  if (!StringDecoder) StringDecoder = require('string_decoder/').StringDecoder;
  this._readableState.decoder = new StringDecoder(enc);
  this._readableState.encoding = enc;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.unpipe"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>unpipe (dest)](#apidoc.element.tar-stream.pack.super_.prototype.unpipe)
- description and source-code
```javascript
unpipe = function (dest) {
  var state = this._readableState;

  // if we're not piping anywhere, then do nothing.
  if (state.pipesCount === 0) return this;

  // just one destination.  most common case.
  if (state.pipesCount === 1) {
    // passed in one, but it's not the right one.
    if (dest && dest !== state.pipes) return this;

    if (!dest) dest = state.pipes;

    // got a match.
    state.pipes = null;
    state.pipesCount = 0;
    state.flowing = false;
    if (dest) dest.emit('unpipe', this);
    return this;
  }

  // slow case. multiple pipe destinations.

  if (!dest) {
    // remove all.
    var dests = state.pipes;
    var len = state.pipesCount;
    state.pipes = null;
    state.pipesCount = 0;
    state.flowing = false;

    for (var i = 0; i < len; i++) {
      dests[i].emit('unpipe', this);
    }return this;
  }

  // try to find the right one.
  var index = indexOf(state.pipes, dest);
  if (index === -1) return this;

  state.pipes.splice(index, 1);
  state.pipesCount -= 1;
  if (state.pipesCount === 1) state.pipes = state.pipes[0];

  dest.emit('unpipe', this);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.unshift"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>unshift (chunk)](#apidoc.element.tar-stream.pack.super_.prototype.unshift)
- description and source-code
```javascript
unshift = function (chunk) {
  var state = this._readableState;
  return readableAddChunk(this, state, chunk, '', true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tar-stream.pack.super_.prototype.wrap"></a>[function <span class="apidocSignatureSpan">tar-stream.pack.super_.prototype.</span>wrap (stream)](#apidoc.element.tar-stream.pack.super_.prototype.wrap)
- description and source-code
```javascript
wrap = function (stream) {
  var state = this._readableState;
  var paused = false;

  var self = this;
  stream.on('end', function () {
    debug('wrapped end');
    if (state.decoder && !state.ended) {
      var chunk = state.decoder.end();
      if (chunk && chunk.length) self.push(chunk);
    }

    self.push(null);
  });

  stream.on('data', function (chunk) {
    debug('wrapped data');
    if (state.decoder) chunk = state.decoder.write(chunk);

    // don't skip over falsy values in objectMode
    if (state.objectMode && (chunk === null || chunk === undefined)) return;else if (!state.objectMode && (!chunk || !chunk.length
)) return;

    var ret = self.push(chunk);
    if (!ret) {
      paused = true;
      stream.pause();
    }
  });

  // proxy all the other methods.
  // important when wrapping filters and duplexes.
  for (var i in stream) {
    if (this[i] === undefined && typeof stream[i] === 'function') {
      this[i] = function (method) {
        return function () {
          return stream[method].apply(stream, arguments);
        };
      }(i);
    }
  }

  // proxy certain important events.
  var events = ['error', 'close', 'destroy', 'pause', 'resume'];
  forEach(events, function (ev) {
    stream.on(ev, self.emit.bind(self, ev));
  });

  // when we try to consume some more bytes, simply unpause the
  // underlying stream.
  self._read = function (n) {
    debug('wrapped _read', n);
    if (paused) {
      paused = false;
      stream.resume();
    }
  };

  return self;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
