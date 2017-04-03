# api documentation for  [fetch (v1.1.0)](http://github.com/andris9/fetch)  [![npm package](https://img.shields.io/npm/v/npmdoc-fetch.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fetch) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fetch.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fetch)
#### Fetch URL contents

[![NPM](https://nodei.co/npm/fetch.png?downloads=true)](https://www.npmjs.com/package/fetch)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fetch/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fetch_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fetch/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fetch/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fetch/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andris Reinman"
    },
    "bugs": {
        "url": "https://github.com/andris9/fetch/issues"
    },
    "dependencies": {
        "biskviit": "1.0.1",
        "encoding": "0.1.12"
    },
    "description": "Fetch URL contents",
    "devDependencies": {
        "chai": "^3.5.0",
        "grunt": "^1.0.1",
        "grunt-eslint": "^18.1.0",
        "grunt-mocha-test": "^0.12.7",
        "mocha": "^2.5.3"
    },
    "directories": {},
    "dist": {
        "shasum": "0a8279f06be37f9f0ebb567560a30a480da59a2e",
        "tarball": "https://registry.npmjs.org/fetch/-/fetch-1.1.0.tgz"
    },
    "gitHead": "c9872c7c7e507c2bc499e4526e0c79dcfa5f7fb2",
    "homepage": "http://github.com/andris9/fetch",
    "keywords": [
        "url"
    ],
    "license": "MIT",
    "main": "./lib/fetch",
    "maintainers": [
        {
            "name": "andris",
            "email": "andris@node.ee"
        }
    ],
    "name": "fetch",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/andris9/fetch.git"
    },
    "scripts": {
        "test": "grunt"
    },
    "version": "1.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fetch](#apidoc.module.fetch)
1.  [function <span class="apidocSignatureSpan">fetch.</span>CookieJar (options)](#apidoc.element.fetch.CookieJar)
1.  [function <span class="apidocSignatureSpan">fetch.</span>FetchStream (url, options)](#apidoc.element.fetch.FetchStream)
1.  [function <span class="apidocSignatureSpan">fetch.</span>fetchUrl (url, options, callback)](#apidoc.element.fetch.fetchUrl)
1.  object <span class="apidocSignatureSpan">fetch.</span>CookieJar.prototype
1.  object <span class="apidocSignatureSpan">fetch.</span>FetchStream.prototype
1.  object <span class="apidocSignatureSpan">fetch.</span>cookiejar

#### [module fetch.CookieJar](#apidoc.module.fetch.CookieJar)
1.  [function <span class="apidocSignatureSpan">fetch.</span>CookieJar (options)](#apidoc.element.fetch.CookieJar.CookieJar)

#### [module fetch.CookieJar.prototype](#apidoc.module.fetch.CookieJar.prototype)
1.  [function <span class="apidocSignatureSpan">fetch.CookieJar.prototype.</span>addCookie (cookie)](#apidoc.element.fetch.CookieJar.prototype.addCookie)
1.  [function <span class="apidocSignatureSpan">fetch.CookieJar.prototype.</span>getCookies (url)](#apidoc.element.fetch.CookieJar.prototype.getCookies)
1.  [function <span class="apidocSignatureSpan">fetch.CookieJar.prototype.</span>matchCookie (cookie, url)](#apidoc.element.fetch.CookieJar.prototype.matchCookie)
1.  [function <span class="apidocSignatureSpan">fetch.CookieJar.prototype.</span>setCookie (cookie_str, url)](#apidoc.element.fetch.CookieJar.prototype.setCookie)

#### [module fetch.FetchStream](#apidoc.module.fetch.FetchStream)
1.  [function <span class="apidocSignatureSpan">fetch.</span>FetchStream (url, options)](#apidoc.element.fetch.FetchStream.FetchStream)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.</span>super_ (options)](#apidoc.element.fetch.FetchStream.super_)

#### [module fetch.FetchStream.prototype](#apidoc.module.fetch.FetchStream.prototype)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>_read (size)](#apidoc.element.fetch.FetchStream.prototype._read)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>_runStream (url_data, url)](#apidoc.element.fetch.FetchStream.prototype._runStream)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>destroy (ex)](#apidoc.element.fetch.FetchStream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>drainBuffer ()](#apidoc.element.fetch.FetchStream.prototype.drainBuffer)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>normalizeOptions ()](#apidoc.element.fetch.FetchStream.prototype.normalizeOptions)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>parseUrl (url)](#apidoc.element.fetch.FetchStream.prototype.parseUrl)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>runStream (url)](#apidoc.element.fetch.FetchStream.prototype.runStream)
1.  [function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>setEncoding (encoding)](#apidoc.element.fetch.FetchStream.prototype.setEncoding)

#### [module fetch.cookiejar](#apidoc.module.fetch.cookiejar)
1.  [function <span class="apidocSignatureSpan">fetch.cookiejar.</span>CookieJar (options)](#apidoc.element.fetch.cookiejar.CookieJar)



# <a name="apidoc.module.fetch"></a>[module fetch](#apidoc.module.fetch)

#### <a name="apidoc.element.fetch.CookieJar"></a>[function <span class="apidocSignatureSpan">fetch.</span>CookieJar (options)](#apidoc.element.fetch.CookieJar)
- description and source-code
```javascript
function CookieJar(options) {
    this.options = options || {};
    this.options.sessionTimeout = this.options.sessionTimeout || 1800; // 30min

    this.cookies = {};
}
```
- example usage
```shell
...

## Cookie sharing

Cookies can be shared between different requests, this can be achieved with 'CookieJar'

var fetch = require("fetch");

var cookies = new fetch.CookieJar();

// add one cookie for testing
cookies.setCookie('alfa=beta; path=/;');

// create a FetchStream with custom CookieJar
var f = fetch.FetchStream("http://www.example.com/page1",{cookieJar: cookies});
...
```

#### <a name="apidoc.element.fetch.FetchStream"></a>[function <span class="apidocSignatureSpan">fetch.</span>FetchStream (url, options)](#apidoc.element.fetch.FetchStream)
- description and source-code
```javascript
function FetchStream(url, options) {
    Stream.call(this);

    options = options || {};

    this.url = url;
    if (!this.url) {
        return this.emit('error', new Error('url not defined'));
    }

    this.userAgent = options.userAgent || 'FetchStream';

    this._redirect_count = 0;

    this.options = options || {};
    this.normalizeOptions();

    // prevent errors before 'error' handler is set by defferring actions
    if (typeof setImmediate !== 'undefined') {
        setImmediate(this.runStream.bind(this, url));
    } else {
        process.nextTick(this.runStream.bind(this, url));
    }
    this.responseBuffer = USE_ALLOC ? Buffer.alloc(0, '', 'binary') : new Buffer(0, 'binary');
    this.ended = false;
    this.readyToRead = 0;
}
```
- example usage
```shell
...
**NB** If the file has been marked with charset other than utf-8, it is converted automatically.

By default 'iconv-lite' is used for charset conversion. If you want to use 'node-iconv' module instead,
add '"iconv": "*"' to your package.json file, it will be picked up by 'fetch' automatically.

## Streaming

'fetch.FetchStream(url [, options]) -> Stream'

Where

  * **url** is the url to fetch
  * **options** is an optional options object

With events:
...
```

#### <a name="apidoc.element.fetch.fetchUrl"></a>[function <span class="apidocSignatureSpan">fetch.</span>fetchUrl (url, options, callback)](#apidoc.element.fetch.fetchUrl)
- description and source-code
```javascript
function fetchUrl(url, options, callback) {
    if (!callback && typeof options === 'function') {
        callback = options;
        options = undefined;
    }
    options = options || {};

    var fetchstream = new FetchStream(url, options),
        response_data, chunks = [],
        length = 0,
        curpos = 0,
        buffer,
        content_type,
        callbackFired = false;

    fetchstream.on('meta', function (meta) {
        response_data = meta;
        content_type = _parseContentType(meta.responseHeaders['content-type']);
    });

    fetchstream.on('data', function (chunk) {
        if (chunk) {
            chunks.push(chunk);
            length += chunk.length;
        }
    });

    fetchstream.on('error', function (error) {
        if (error && error.code === 'HPE_INVALID_CONSTANT') {
            // skip invalid formatting errors
            return;
        }
        if (callbackFired) {
            return;
        }
        callbackFired = true;
        callback(error);
    });

    fetchstream.on('end', function () {
        if (callbackFired) {
            return;
        }
        callbackFired = true;

        buffer = USE_ALLOC ? Buffer.alloc(length) : new Buffer(length);
        for (var i = 0, len = chunks.length; i < len; i++) {
            chunks[i].copy(buffer, curpos);
            curpos += chunks[i].length;
        }

        if (content_type.mimeType === 'text/html') {
            content_type.charset = _findHTMLCharset(buffer) || content_type.charset;
        }

        content_type.charset = (options.overrideCharset || content_type.charset || 'utf-8').trim().toLowerCase();


        if (!options.disableDecoding && !content_type.charset.match(/^utf-?8$/i)) {
            buffer = encodinglib.convert(buffer, 'UTF-8', content_type.charset);
        }

        if (options.outputEncoding) {
            return callback(null, response_data, buffer.toString(options.outputEncoding));
        } else {
            return callback(null, response_data, buffer);
        }

    });
}
```
- example usage
```shell
...

## Usage

See examples folder for a complete example

## Fetch from URL

'fetch.fetchUrl(url [, options], callback)'

Where

* **url** is the url to fetch
* **options** is an optional options object
* **callback** is the callback to run - 'callback(error, meta, body)'
...
```



# <a name="apidoc.module.fetch.CookieJar"></a>[module fetch.CookieJar](#apidoc.module.fetch.CookieJar)

#### <a name="apidoc.element.fetch.CookieJar.CookieJar"></a>[function <span class="apidocSignatureSpan">fetch.</span>CookieJar (options)](#apidoc.element.fetch.CookieJar.CookieJar)
- description and source-code
```javascript
function CookieJar(options) {
    this.options = options || {};
    this.options.sessionTimeout = this.options.sessionTimeout || 1800; // 30min

    this.cookies = {};
}
```
- example usage
```shell
...

## Cookie sharing

Cookies can be shared between different requests, this can be achieved with 'CookieJar'

var fetch = require("fetch");

var cookies = new fetch.CookieJar();

// add one cookie for testing
cookies.setCookie('alfa=beta; path=/;');

// create a FetchStream with custom CookieJar
var f = fetch.FetchStream("http://www.example.com/page1",{cookieJar: cookies});
...
```



# <a name="apidoc.module.fetch.CookieJar.prototype"></a>[module fetch.CookieJar.prototype](#apidoc.module.fetch.CookieJar.prototype)

#### <a name="apidoc.element.fetch.CookieJar.prototype.addCookie"></a>[function <span class="apidocSignatureSpan">fetch.CookieJar.prototype.</span>addCookie (cookie)](#apidoc.element.fetch.CookieJar.prototype.addCookie)
- description and source-code
```javascript
addCookie = function (cookie) {

    if (!cookie || !cookie.name) {
        return;
    }

    var lcookie;

    if (!this.cookies[cookie.name]) {
        this.cookies[cookie.name] = [];
    }

    // overwrite if has same params
    for (var i = 0, len = this.cookies[cookie.name].length; i < len; i++) {
        lcookie = this.cookies[cookie.name][i];
        if (
            lcookie.path === cookie.path &&
            lcookie.domain === cookie.domain &&
            lcookie.secure === cookie.secure &&
            lcookie.httponly === cookie.httponly
        ) {
            this.cookies[cookie.name][i] = cookie;
            return;
        }
    }

    this.cookies[cookie.name].push(cookie);
}
```
- example usage
```shell
...
        if (urlparts.hostname) {
            cookie._domain = urlparts.hostname;
        }
    } else {
        cookie._domain = cookie.domain;
    }

    this.addCookie(cookie);
};
...
```

#### <a name="apidoc.element.fetch.CookieJar.prototype.getCookies"></a>[function <span class="apidocSignatureSpan">fetch.CookieJar.prototype.</span>getCookies (url)](#apidoc.element.fetch.CookieJar.prototype.getCookies)
- description and source-code
```javascript
getCookies = function (url) {
    var keys = Object.keys(this.cookies),
        cookie, cookies = [];

    for (var i = 0, len = keys.length; i < len; i++) {
        if (Array.isArray(this.cookies[keys[i]])) {
            for (var j = 0, lenj = this.cookies[keys[i]].length; j < lenj; j++) {
                cookie = this.cookies[keys[i]][j];
                if (this.matchCookie(cookie, url)) {
                    cookies.push(cookie.name + '=' + cookie.value);
                }
            }
        }
    }
    return cookies.join('; ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fetch.CookieJar.prototype.matchCookie"></a>[function <span class="apidocSignatureSpan">fetch.CookieJar.prototype.</span>matchCookie (cookie, url)](#apidoc.element.fetch.CookieJar.prototype.matchCookie)
- description and source-code
```javascript
matchCookie = function (cookie, url) {
    var urlparts = urllib.parse(url || '', false, true),
        path;

    // check expire
    if (cookie.expire) {
        if (cookie.expire.getTime() < Date.now()) {
            return;
        }
    }

    // check if hostname matches
    if (urlparts.hostname && cookie._domain) {
        if (!(urlparts.hostname === cookie._domain || urlparts.hostname.substr(-(cookie._domain.length + 1)) === '.' + cookie._domain
)) {
            return false;
        }
    }

    // check if path matches
    if (cookie.path && urlparts.pathname) {

        path = (urlparts.pathname || '/').split('/');
        path.pop();
        path = path.join('/').trim();
        if (path.substr(0, 1) !== '/') {
            path = '/' + path;
        }
        if (path.substr(-1) !== '/') {
            path += '/';
        }

        if (path.substr(0, cookie.path.length) !== cookie.path) {
            return false;
        }
    }

    // check secure
    if (cookie.secure && urlparts.protocol) {
        if (urlparts.protocol !== 'https:') {
            return false;
        }
    }

    // check httponly
    if (cookie.httponly && urlparts.protocol) {
        if (urlparts.protocol !== 'http:') {
            return false;
        }
    }

    return true;
}
```
- example usage
```shell
...
    var keys = Object.keys(this.cookies),
        cookie, cookies = [];

    for (var i = 0, len = keys.length; i < len; i++) {
        if (Array.isArray(this.cookies[keys[i]])) {
            for (var j = 0, lenj = this.cookies[keys[i]].length; j < lenj; j++) {
                cookie = this.cookies[keys[i]][j];
                if (this.matchCookie(cookie, url)) {
                    cookies.push(cookie.name + '=' + cookie.value);
                }
            }
        }
    }
    return cookies.join('; ');
};
...
```

#### <a name="apidoc.element.fetch.CookieJar.prototype.setCookie"></a>[function <span class="apidocSignatureSpan">fetch.CookieJar.prototype.</span>setCookie (cookie_str, url)](#apidoc.element.fetch.CookieJar.prototype.setCookie)
- description and source-code
```javascript
setCookie = function (cookie_str, url) {
    var parts = (cookie_str || '').split(';'),
        cookie = {},
        urlparts = urllib.parse(url || '', false, true),
        path;

    parts.forEach((function (part) {
        var key, val;
        part = part.split('=');
        key = part.shift().trim();
        val = part.join('=').trim();

        if (!key) {
            return;
        }

        switch (key.toLowerCase()) {

            case 'expires':

                cookie.expires = new Date(val);
                break;

            case 'path':
                cookie.path = val.trim();
                break;

            case 'domain':
                cookie.domain = val.toLowerCase();
                break;

            case 'max-age':
                cookie.expires = new Date(Date.now() + (Number(val) || 0) * 1000);
                break;

            case 'secure':
                cookie.secure = true;
                break;

            case 'httponly':
                cookie.httponly = true;
                break;

            default:
                if (!cookie.name) {
                    cookie.name = key;
                    cookie.value = val;
                }
        }
    }).bind(this));

    // use current path when path is not specified
    if (!cookie.path) {
        path = (urlparts.pathname || '/').split('/');
        path.pop();
        cookie.path = path.join('/').trim();
        if (cookie.path.substr(0, 1) !== '/') {
            cookie.path = '/' + cookie.path;
        }
        if (cookie.path.substr(-1) !== '/') {
            cookie.path += '/';
        }
    }

    // if no expire date, then use sessionTimeout value
    if (!cookie.expires) {
        cookie._expires = new Date(Date.now() + (Number(this.options.sessionTimeout) || 0) * 1000);
    } else {
        cookie._expires = cookie.expires;
    }

    if (!cookie.domain) {
        if (urlparts.hostname) {
            cookie._domain = urlparts.hostname;
        }
    } else {
        cookie._domain = cookie.domain;
    }

    this.addCookie(cookie);
}
```
- example usage
```shell
...
Cookies can be shared between different requests, this can be achieved with 'CookieJar'

var fetch = require("fetch");

var cookies = new fetch.CookieJar();

// add one cookie for testing
cookies.setCookie('alfa=beta; path=/;');

// create a FetchStream with custom CookieJar
var f = fetch.FetchStream("http://www.example.com/page1",{cookieJar: cookies});

f.on("end", function(){
    // if cookies were set with the previos request, the data is
    // saved in 'cookieJar' and passed to the next request
...
```



# <a name="apidoc.module.fetch.FetchStream"></a>[module fetch.FetchStream](#apidoc.module.fetch.FetchStream)

#### <a name="apidoc.element.fetch.FetchStream.FetchStream"></a>[function <span class="apidocSignatureSpan">fetch.</span>FetchStream (url, options)](#apidoc.element.fetch.FetchStream.FetchStream)
- description and source-code
```javascript
function FetchStream(url, options) {
    Stream.call(this);

    options = options || {};

    this.url = url;
    if (!this.url) {
        return this.emit('error', new Error('url not defined'));
    }

    this.userAgent = options.userAgent || 'FetchStream';

    this._redirect_count = 0;

    this.options = options || {};
    this.normalizeOptions();

    // prevent errors before 'error' handler is set by defferring actions
    if (typeof setImmediate !== 'undefined') {
        setImmediate(this.runStream.bind(this, url));
    } else {
        process.nextTick(this.runStream.bind(this, url));
    }
    this.responseBuffer = USE_ALLOC ? Buffer.alloc(0, '', 'binary') : new Buffer(0, 'binary');
    this.ended = false;
    this.readyToRead = 0;
}
```
- example usage
```shell
...
**NB** If the file has been marked with charset other than utf-8, it is converted automatically.

By default 'iconv-lite' is used for charset conversion. If you want to use 'node-iconv' module instead,
add '"iconv": "*"' to your package.json file, it will be picked up by 'fetch' automatically.

## Streaming

'fetch.FetchStream(url [, options]) -> Stream'

Where

  * **url** is the url to fetch
  * **options** is an optional options object

With events:
...
```

#### <a name="apidoc.element.fetch.FetchStream.super_"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.</span>super_ (options)](#apidoc.element.fetch.FetchStream.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function')
    this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fetch.FetchStream.prototype"></a>[module fetch.FetchStream.prototype](#apidoc.module.fetch.FetchStream.prototype)

#### <a name="apidoc.element.fetch.FetchStream.prototype._read"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>_read (size)](#apidoc.element.fetch.FetchStream.prototype._read)
- description and source-code
```javascript
_read = function (size) {
    if (this.ended && this.responseBuffer.length === 0) {
        this.push(null);
        return;
    }
    this.readyToRead += size;
    this.drainBuffer();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fetch.FetchStream.prototype._runStream"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>_runStream (url_data, url)](#apidoc.element.fetch.FetchStream.prototype._runStream)
- description and source-code
```javascript
_runStream = function (url_data, url) {

    var req = url_data.transport.request(url_data.urloptions, (function (res) {

        // catch new cookies before potential redirect
        if (Array.isArray(res.headers['set-cookie'])) {
            for (var i = 0; i < res.headers['set-cookie'].length; i++) {
                this.cookieJar.setCookie(res.headers['set-cookie'][i], url);
            }
        }

        if ([301, 302, 303, 307, 308].indexOf(res.statusCode) >= 0) {
            if (!this.options.disableRedirects && this.options.maxRedirects > this._redirect_count && res.headers.location) {
                this._redirect_count++;
                req.destroy();
                this.runStream(urllib.resolve(url, res.headers.location));
                return;
            }
        }

        this.meta = {
            status: res.statusCode,
            responseHeaders: res.headers,
            finalUrl: url,
            redirectCount: this._redirect_count,
            cookieJar: this.cookieJar
        };

        var curlen = 0,
            maxlen,

            receive = (function (chunk) {
                if (curlen + chunk.length > this.options.maxResponseLength) {
                    maxlen = this.options.maxResponseLength - curlen;
                } else {
                    maxlen = chunk.length;
                }

                if (maxlen <= 0) {
                    return;
                }

                curlen += Math.min(maxlen, chunk.length);
                if (maxlen >= chunk.length) {
                    if (this.responseBuffer.length === 0) {
                        this.responseBuffer = chunk;
                    } else {
                        this.responseBuffer = Buffer.concat([this.responseBuffer, chunk]);
                    }
                } else {
                    this.responseBuffer = Buffer.concat([this.responseBuffer, chunk], this.responseBuffer.length + maxlen);
                }
                this.drainBuffer();
            }).bind(this),

            error = (function (e) {
                this.ended = true;
                this.emit('error', e);
                this.drainBuffer();
            }).bind(this),

            end = (function () {
                this.ended = true;
                if (this.responseBuffer.length === 0) {
                    this.push(null);
                }
            }).bind(this),

            unpack = (function (type, res) {
                var z = zlib['create' + type]();
                z.on('data', receive);
                z.on('error', error);
                z.on('end', end);
                res.pipe(z);
            }).bind(this);

        this.emit('meta', this.meta);

        if (res.headers['content-encoding']) {
            switch (res.headers['content-encoding'].toLowerCase().trim()) {
                case 'gzip':
                    return unpack('Gunzip', res);
                case 'deflate':
                    return unpack('InflateRaw', res);
            }
        }

        res.on('data', receive);
        res.on('end', end);

    }).bind(this));

    req.on('error', (function (e) {
        this.emit('error', e);
    }).bind(this));

    if (this.options.timeout) {
        req.setTimeout(this.options.timeout, req.abort.bind(req));
    }
    this.on('destroy', req.abort.bind(req));

    if (this.options.payload) {
        req.end(this.options.payload);
    } else if (this.options.payloadStream) {
        this.options.payloadStream.pipe(req);
        this.options.payloadStream.resume();
    } else {
        req.end();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fetch.FetchStream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>destroy (ex)](#apidoc.element.fetch.FetchStream.prototype.destroy)
- description and source-code
```javascript
destroy = function (ex) {
    this.emit('destroy', ex);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fetch.FetchStream.prototype.drainBuffer"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>drainBuffer ()](#apidoc.element.fetch.FetchStream.prototype.drainBuffer)
- description and source-code
```javascript
drainBuffer = function () {
    if (this.readyToRead === 0) {
        return;
    }
    if (this.responseBuffer.length === 0) {
        return;
    }
    var push;
    var rest;
    var restSize;

    if (this.responseBuffer.length > this.readyToRead) {
        push = USE_ALLOC ? Buffer.alloc(this.readyToRead, '', 'binary') : new Buffer(this.readyToRead, 'binary');
        this.responseBuffer.copy(push, 0, 0, this.readyToRead);
        restSize = this.responseBuffer.length - this.readyToRead;
        rest = USE_ALLOC ? Buffer.alloc(restSize, '', 'binary') : new Buffer(restSize, 'binary');
        this.responseBuffer.copy(rest, 0, this.readyToRead);
    } else {
        push = this.responseBuffer;
        rest = USE_ALLOC ? Buffer.alloc(0, '', 'binary') : new Buffer(0, 'binary');
    }
    this.responseBuffer = rest;
    this.readyToRead = 0;
    if (this.options.encoding) {
        this.push(push, this.options.encoding);
    } else {
        this.push(push);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fetch.FetchStream.prototype.normalizeOptions"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>normalizeOptions ()](#apidoc.element.fetch.FetchStream.prototype.normalizeOptions)
- description and source-code
```javascript
normalizeOptions = function () {

    // cookiejar
    this.cookieJar = this.options.cookieJar || new CookieJar();

    // default redirects - 10
    // if disableRedirect is set, then 0
    if (!this.options.disableRedirect && typeof this.options.maxRedirects !== 'number' &&
        !(this.options.maxRedirects instanceof Number)) {
        this.options.maxRedirects = 10;
    } else if (this.options.disableRedirects) {
        this.options.maxRedirects = 0;
    }

    // normalize header keys
    // HTTP and HTTPS takes in key names in case insensitive but to find
    // an exact value from an object key name needs to be case sensitive
    // so we're just lowercasing all input keys
    this.options.headers = this.options.headers || {};

    var keys = Object.keys(this.options.headers);
    var newheaders = {};
    var i;

    for (i = keys.length - 1; i >= 0; i--) {
        newheaders[keys[i].toLowerCase().trim()] = this.options.headers[keys[i]];
    }

    this.options.headers = newheaders;

    if (!this.options.headers['user-agent']) {
        this.options.headers['user-agent'] = this.userAgent;
    }

    if (!this.options.headers.pragma) {
        this.options.headers.pragma = 'no-cache';
    }

    if (!this.options.headers['cache-control']) {
        this.options.headers['cache-control'] = 'no-cache';
    }

    if (!this.options.disableGzip) {
        this.options.headers['accept-encoding'] = 'gzip, deflate';
    } else {
        delete this.options.headers['accept-encoding'];
    }

    // max length for the response,
    // if not set, default is Infinity
    if (!this.options.maxResponseLength) {
        this.options.maxResponseLength = Infinity;
    }

    // method:
    // defaults to GET, or when payload present to POST
    if (!this.options.method) {
        this.options.method = this.options.payload || this.options.payloadSize ? 'POST' : 'GET';
    }

    // set cookies
    // takes full cookie definition strings as params
    if (this.options.cookies) {
        for (i = 0; i < this.options.cookies.length; i++) {
            this.cookieJar.setCookie(this.options.cookies[i], this.url);
        }
    }

    // rejectUnauthorized
    if (typeof this.options.rejectUnauthorized === 'undefined') {
        this.options.rejectUnauthorized = true;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fetch.FetchStream.prototype.parseUrl"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>parseUrl (url)](#apidoc.element.fetch.FetchStream.prototype.parseUrl)
- description and source-code
```javascript
parseUrl = function (url) {
    var urlparts = urllib.parse(url, false, true),
        transport,
        urloptions = {
            host: urlparts.hostname || urlparts.host,
            port: urlparts.port,
            path: urlparts.pathname + (urlparts.search || '') || '/',
            method: this.options.method,
            rejectUnauthorized: this.options.rejectUnauthorized
        };

    switch (urlparts.protocol) {
        case 'https:':
            transport = https;
            break;
        case 'http:':
        default:
            transport = http;
            break;
    }

    if (transport === https) {
        if('agentHttps' in this.options){
            urloptions.agent = this.options.agentHttps;
        }
        if('agent' in this.options){
            urloptions.agent = this.options.agent;
        }
    } else {
        if('agentHttp' in this.options){
            urloptions.agent = this.options.agentHttp;
        }
        if('agent' in this.options){
            urloptions.agent = this.options.agent;
        }
    }

    if (!urloptions.port) {
        switch (urlparts.protocol) {
            case 'https:':
                urloptions.port = 443;
                break;
            case 'http:':
            default:
                urloptions.port = 80;
                break;
        }
    }

    urloptions.headers = this.options.headers || {};

    if (urlparts.auth) {
        var buf = USE_ALLOC ? Buffer.alloc(Buffer.byteLength(urlparts.auth), urlparts.auth) : new Buffer(urlparts.auth);
        urloptions.headers.Authorization = 'Basic ' + buf.toString('base64');
    }

    return {
        urloptions: urloptions,
        transport: transport
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fetch.FetchStream.prototype.runStream"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>runStream (url)](#apidoc.element.fetch.FetchStream.prototype.runStream)
- description and source-code
```javascript
runStream = function (url) {
    var url_data = this.parseUrl(url),
        cookies = this.cookieJar.getCookies(url);

    if (cookies) {
        url_data.urloptions.headers.cookie = cookies;
    } else {
        delete url_data.urloptions.headers.cookie;
    }

    if (this.options.payload) {
        url_data.urloptions.headers['content-length'] = Buffer.byteLength(this.options.payload || '', 'utf-8');
    }

    if (this.options.payloadSize) {
        url_data.urloptions.headers['content-length'] = this.options.payloadSize;
    }

    if (this.options.asyncDnsLoookup) {
        var dnsCallback = (function (err, addresses) {
            if (err) {
                this.emit('error', err);
                return;
            }

            url_data.urloptions.headers.host = url_data.urloptions.hostname || url_data.urloptions.host;
            url_data.urloptions.hostname = addresses[0];
            url_data.urloptions.host = url_data.urloptions.headers.host + (url_data.urloptions.port ? ':' + url_data.urloptions.
port : '');

            this._runStream(url_data, url);
        }).bind(this);

        if (net.isIP(url_data.urloptions.host)) {
            dnsCallback(null, [url_data.urloptions.host]);
        } else {
            dns.resolve4(url_data.urloptions.host, dnsCallback);
        }
    } else {
        this._runStream(url_data, url);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fetch.FetchStream.prototype.setEncoding"></a>[function <span class="apidocSignatureSpan">fetch.FetchStream.prototype.</span>setEncoding (encoding)](#apidoc.element.fetch.FetchStream.prototype.setEncoding)
- description and source-code
```javascript
setEncoding = function (encoding) {
    this.options.encoding = encoding;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fetch.cookiejar"></a>[module fetch.cookiejar](#apidoc.module.fetch.cookiejar)

#### <a name="apidoc.element.fetch.cookiejar.CookieJar"></a>[function <span class="apidocSignatureSpan">fetch.cookiejar.</span>CookieJar (options)](#apidoc.element.fetch.cookiejar.CookieJar)
- description and source-code
```javascript
function CookieJar(options) {
    this.options = options || {};
    this.options.sessionTimeout = this.options.sessionTimeout || 1800; // 30min

    this.cookies = {};
}
```
- example usage
```shell
...

## Cookie sharing

Cookies can be shared between different requests, this can be achieved with 'CookieJar'

var fetch = require("fetch");

var cookies = new fetch.CookieJar();

// add one cookie for testing
cookies.setCookie('alfa=beta; path=/;');

// create a FetchStream with custom CookieJar
var f = fetch.FetchStream("http://www.example.com/page1",{cookieJar: cookies});
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
