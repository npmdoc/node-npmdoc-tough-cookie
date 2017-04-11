# api documentation for  [tough-cookie (v2.3.2)](https://github.com/salesforce/tough-cookie)  [![npm package](https://img.shields.io/npm/v/npmdoc-tough-cookie.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tough-cookie) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tough-cookie.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tough-cookie)
#### RFC6265 Cookies and Cookie Jar for node.js

[![NPM](https://nodei.co/npm/tough-cookie.png?downloads=true)](https://www.npmjs.com/package/tough-cookie)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tough-cookie/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-tough-cookie%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tough-cookie/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tough-cookie/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tough-cookie/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jeremy Stashewsky",
        "email": "jstashewsky@salesforce.com"
    },
    "bugs": {
        "url": "https://github.com/salesforce/tough-cookie/issues"
    },
    "contributors": [
        {
            "name": "Alexander Savin"
        },
        {
            "name": "Ian Livingstone"
        },
        {
            "name": "Ivan Nikulin"
        },
        {
            "name": "Lalit Kapoor"
        },
        {
            "name": "Sam Thompson"
        },
        {
            "name": "Sebastian Mayr"
        }
    ],
    "dependencies": {
        "punycode": "^1.4.1"
    },
    "description": "RFC6265 Cookies and Cookie Jar for node.js",
    "devDependencies": {
        "async": "^1.4.2",
        "string.prototype.repeat": "^0.2.0",
        "vows": "^0.8.1"
    },
    "directories": {},
    "dist": {
        "shasum": "f081f76e4c85720e6c37a5faced737150d84072a",
        "tarball": "https://registry.npmjs.org/tough-cookie/-/tough-cookie-2.3.2.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "files": [
        "lib"
    ],
    "gitHead": "2610df5dc8ef7373a483d509006e5887572a4076",
    "homepage": "https://github.com/salesforce/tough-cookie",
    "keywords": [
        "HTTP",
        "cookie",
        "cookies",
        "set-cookie",
        "cookiejar",
        "jar",
        "RFC6265",
        "RFC2965"
    ],
    "license": "BSD-3-Clause",
    "main": "./lib/cookie",
    "maintainers": [
        {
            "name": "awaterma",
            "email": "awaterma@awaterma.net"
        },
        {
            "name": "jstash",
            "email": "jstash@gmail.com"
        },
        {
            "name": "nexxy",
            "email": "emily@contactvibe.com"
        }
    ],
    "name": "tough-cookie",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/salesforce/tough-cookie.git"
    },
    "scripts": {
        "suffixup": "curl -o public_suffix_list.dat https://publicsuffix.org/list/public_suffix_list.dat && ./generate-pubsuffix.js",
        "test": "vows test/*_test.js"
    },
    "version": "2.3.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module tough-cookie](#apidoc.module.tough-cookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>Cookie (options)](#apidoc.element.tough-cookie.Cookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>CookieJar (store, options)](#apidoc.element.tough-cookie.CookieJar)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>MemoryCookieStore ()](#apidoc.element.tough-cookie.MemoryCookieStore)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>Store ()](#apidoc.element.tough-cookie.Store)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>canonicalDomain (str)](#apidoc.element.tough-cookie.canonicalDomain)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>cookieCompare (a, b)](#apidoc.element.tough-cookie.cookieCompare)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>defaultPath (path)](#apidoc.element.tough-cookie.defaultPath)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>domainMatch (str, domStr, canonicalize)](#apidoc.element.tough-cookie.domainMatch)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>formatDate (date)](#apidoc.element.tough-cookie.formatDate)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>fromJSON (str)](#apidoc.element.tough-cookie.fromJSON)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>getPublicSuffix (domain)](#apidoc.element.tough-cookie.getPublicSuffix)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>parse (str, options)](#apidoc.element.tough-cookie.parse)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>parseDate (str)](#apidoc.element.tough-cookie.parseDate)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>pathMatch (reqPath, cookiePath)](#apidoc.element.tough-cookie.pathMatch)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>permuteDomain (domain)](#apidoc.element.tough-cookie.permuteDomain)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>permutePath (path)](#apidoc.element.tough-cookie.permutePath)
1.  object <span class="apidocSignatureSpan">tough-cookie.</span>Cookie.prototype
1.  object <span class="apidocSignatureSpan">tough-cookie.</span>CookieJar.prototype
1.  object <span class="apidocSignatureSpan">tough-cookie.</span>MemoryCookieStore.prototype
1.  object <span class="apidocSignatureSpan">tough-cookie.</span>Store.prototype
1.  object <span class="apidocSignatureSpan">tough-cookie.</span>memstore

#### [module tough-cookie.Cookie](#apidoc.module.tough-cookie.Cookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>Cookie (options)](#apidoc.element.tough-cookie.Cookie.Cookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.</span>fromJSON (str)](#apidoc.element.tough-cookie.Cookie.fromJSON)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.</span>parse (str, options)](#apidoc.element.tough-cookie.Cookie.parse)
1.  number <span class="apidocSignatureSpan">tough-cookie.Cookie.</span>cookiesCreated
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.</span>serializableProperties

#### [module tough-cookie.Cookie.prototype](#apidoc.module.tough-cookie.Cookie.prototype)
1.  boolean <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>httpOnly
1.  boolean <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>secure
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>TTL (now)](#apidoc.element.tough-cookie.Cookie.prototype.TTL)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>canonicalizedDomain ()](#apidoc.element.tough-cookie.Cookie.prototype.canonicalizedDomain)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>cdomain ()](#apidoc.element.tough-cookie.Cookie.prototype.cdomain)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>clone ()](#apidoc.element.tough-cookie.Cookie.prototype.clone)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>cookieString ()](#apidoc.element.tough-cookie.Cookie.prototype.cookieString)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>expiryDate (now)](#apidoc.element.tough-cookie.Cookie.prototype.expiryDate)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>expiryTime (now)](#apidoc.element.tough-cookie.Cookie.prototype.expiryTime)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>inspect ()](#apidoc.element.tough-cookie.Cookie.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>isPersistent ()](#apidoc.element.tough-cookie.Cookie.prototype.isPersistent)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>setExpires (exp)](#apidoc.element.tough-cookie.Cookie.prototype.setExpires)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>setMaxAge (age)](#apidoc.element.tough-cookie.Cookie.prototype.setMaxAge)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>toJSON ()](#apidoc.element.tough-cookie.Cookie.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>toString ()](#apidoc.element.tough-cookie.Cookie.prototype.toString)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>validate ()](#apidoc.element.tough-cookie.Cookie.prototype.validate)
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>creation
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>domain
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>extensions
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>hostOnly
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>lastAccessed
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>maxAge
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>path
1.  object <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>pathIsDefault
1.  string <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>expires
1.  string <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>key
1.  string <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>value

#### [module tough-cookie.CookieJar](#apidoc.module.tough-cookie.CookieJar)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>CookieJar (store, options)](#apidoc.element.tough-cookie.CookieJar.CookieJar)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.</span>deserialize (strOrObj, store, cb)](#apidoc.element.tough-cookie.CookieJar.deserialize)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.</span>deserializeSync (strOrObj, store)](#apidoc.element.tough-cookie.CookieJar.deserializeSync)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.</span>fromJSON (strOrObj, store)](#apidoc.element.tough-cookie.CookieJar.fromJSON)

#### [module tough-cookie.CookieJar.prototype](#apidoc.module.tough-cookie.CookieJar.prototype)
1.  boolean <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>enableLooseMode
1.  boolean <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>rejectPublicSuffixes
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>_importCookies (serialized, cb)](#apidoc.element.tough-cookie.CookieJar.prototype._importCookies)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>_importCookiesSync ()](#apidoc.element.tough-cookie.CookieJar.prototype._importCookiesSync)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>clone (newStore, cb)](#apidoc.element.tough-cookie.CookieJar.prototype.clone)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>cloneSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.cloneSync)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getCookieString ()](#apidoc.element.tough-cookie.CookieJar.prototype.getCookieString)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getCookieStringSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.getCookieStringSync)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getCookies (url, options, cb)](#apidoc.element.tough-cookie.CookieJar.prototype.getCookies)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getCookiesSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.getCookiesSync)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getSetCookieStrings ()](#apidoc.element.tough-cookie.CookieJar.prototype.getSetCookieStrings)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getSetCookieStringsSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.getSetCookieStringsSync)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>serialize (cb)](#apidoc.element.tough-cookie.CookieJar.prototype.serialize)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>serializeSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.serializeSync)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>setCookie (cookie, url, options, cb)](#apidoc.element.tough-cookie.CookieJar.prototype.setCookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>setCookieSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.setCookieSync)
1.  [function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>toJSON ()](#apidoc.element.tough-cookie.CookieJar.prototype.toJSON)
1.  object <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>store

#### [module tough-cookie.MemoryCookieStore](#apidoc.module.tough-cookie.MemoryCookieStore)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>MemoryCookieStore ()](#apidoc.element.tough-cookie.MemoryCookieStore.MemoryCookieStore)
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.</span>super_ ()](#apidoc.element.tough-cookie.MemoryCookieStore.super_)

#### [module tough-cookie.MemoryCookieStore.prototype](#apidoc.module.tough-cookie.MemoryCookieStore.prototype)
1.  boolean <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>synchronous
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>findCookie (domain, path, key, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.findCookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>findCookies (domain, path, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.findCookies)
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>getAllCookies (cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.getAllCookies)
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>inspect ()](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>putCookie (cookie, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.putCookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>removeCookie (domain, path, key, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.removeCookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>removeCookies (domain, path, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.removeCookies)
1.  [function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>updateCookie (oldCookie, newCookie, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.updateCookie)
1.  object <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>idx

#### [module tough-cookie.Store](#apidoc.module.tough-cookie.Store)
1.  [function <span class="apidocSignatureSpan">tough-cookie.</span>Store ()](#apidoc.element.tough-cookie.Store.Store)

#### [module tough-cookie.Store.prototype](#apidoc.module.tough-cookie.Store.prototype)
1.  boolean <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>synchronous
1.  [function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>findCookie (domain, path, key, cb)](#apidoc.element.tough-cookie.Store.prototype.findCookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>findCookies (domain, path, cb)](#apidoc.element.tough-cookie.Store.prototype.findCookies)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>getAllCookies (cb)](#apidoc.element.tough-cookie.Store.prototype.getAllCookies)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>putCookie (cookie, cb)](#apidoc.element.tough-cookie.Store.prototype.putCookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>removeCookie (domain, path, key, cb)](#apidoc.element.tough-cookie.Store.prototype.removeCookie)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>removeCookies (domain, path, cb)](#apidoc.element.tough-cookie.Store.prototype.removeCookies)
1.  [function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>updateCookie (oldCookie, newCookie, cb)](#apidoc.element.tough-cookie.Store.prototype.updateCookie)

#### [module tough-cookie.memstore](#apidoc.module.tough-cookie.memstore)
1.  [function <span class="apidocSignatureSpan">tough-cookie.memstore.</span>MemoryCookieStore ()](#apidoc.element.tough-cookie.memstore.MemoryCookieStore)



# <a name="apidoc.module.tough-cookie"></a>[module tough-cookie](#apidoc.module.tough-cookie)

#### <a name="apidoc.element.tough-cookie.Cookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>Cookie (options)](#apidoc.element.tough-cookie.Cookie)
- description and source-code
```javascript
function Cookie(options) {
  options = options || {};

  Object.keys(options).forEach(function(prop) {
    if (Cookie.prototype.hasOwnProperty(prop) &&
        Cookie.prototype[prop] !== options[prop] &&
        prop.substr(0,1) !== '_')
    {
      this[prop] = options[prop];
    }
  }, this);

  this.creation = this.creation || new Date();

  // used to break creation ties in cookieCompare():
  Object.defineProperty(this, 'creationIndex', {
    configurable: false,
    enumerable: false, // important for assert.deepEqual checks
    writable: true,
    value: ++Cookie.cookiesCreated
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.CookieJar"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>CookieJar (store, options)](#apidoc.element.tough-cookie.CookieJar)
- description and source-code
```javascript
function CookieJar(store, options) {
  if (typeof options === "boolean") {
    options = {rejectPublicSuffixes: options};
  } else if (options == null) {
    options = {};
  }
  if (options.rejectPublicSuffixes != null) {
    this.rejectPublicSuffixes = options.rejectPublicSuffixes;
  }
  if (options.looseMode != null) {
    this.enableLooseMode = options.looseMode;
  }

  if (!store) {
    store = new MemoryCookieStore();
  }
  this.store = store;
}
```
- example usage
```shell
...
''' javascript
var tough = require('tough-cookie');
var Cookie = tough.Cookie;
var cookie = Cookie.parse(header);
cookie.value = 'somethingdifferent';
header = cookie.toString();

var cookiejar = new tough.CookieJar();
cookiejar.setCookie(cookie, 'http://currentdomain.example.com/path', cb);
// ...
cookiejar.getCookies('http://example.com/otherpath',function(err,cookies) {
  res.headers['cookie'] = cookies.join('; ');
});
'''
...
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>MemoryCookieStore ()](#apidoc.element.tough-cookie.MemoryCookieStore)
- description and source-code
```javascript
function MemoryCookieStore() {
  Store.call(this);
  this.idx = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.Store"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>Store ()](#apidoc.element.tough-cookie.Store)
- description and source-code
```javascript
function Store() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.canonicalDomain"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>canonicalDomain (str)](#apidoc.element.tough-cookie.canonicalDomain)
- description and source-code
```javascript
function canonicalDomain(str) {
  if (str == null) {
    return null;
  }
  str = str.trim().replace(/^\./,''); // S4.1.2.3 & S5.2.3: ignore leading .

  // convert to IDN if any non-ASCII characters
  if (punycode && /[^\u0001-\u007f]/.test(str)) {
    str = punycode.toASCII(str);
  }

  return str.toLowerCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.cookieCompare"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>cookieCompare (a, b)](#apidoc.element.tough-cookie.cookieCompare)
- description and source-code
```javascript
function cookieCompare(a, b) {
  var cmp = 0;

  // descending for length: b CMP a
  var aPathLen = a.path ? a.path.length : 0;
  var bPathLen = b.path ? b.path.length : 0;
  cmp = bPathLen - aPathLen;
  if (cmp !== 0) {
    return cmp;
  }

  // ascending for time: a CMP b
  var aTime = a.creation ? a.creation.getTime() : MAX_TIME;
  var bTime = b.creation ? b.creation.getTime() : MAX_TIME;
  cmp = aTime - bTime;
  if (cmp !== 0) {
    return cmp;
  }

  // break ties for the same millisecond (precision of JavaScript's clock)
  cmp = a.creationIndex - b.creationIndex;

  return cmp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.defaultPath"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>defaultPath (path)](#apidoc.element.tough-cookie.defaultPath)
- description and source-code
```javascript
function defaultPath(path) {
  // "2. If the uri-path is empty or if the first character of the uri-path is not
  // a %x2F ("/") character, output %x2F ("/") and skip the remaining steps.
  if (!path || path.substr(0,1) !== "/") {
    return "/";
  }

  // "3. If the uri-path contains no more than one %x2F ("/") character, output
  // %x2F ("/") and skip the remaining step."
  if (path === "/") {
    return path;
  }

  var rightSlash = path.lastIndexOf("/");
  if (rightSlash === 0) {
    return "/";
  }

  // "4. Output the characters of the uri-path from the first character up to,
  // but not including, the right-most %x2F ("/")."
  return path.slice(0, rightSlash);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.domainMatch"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>domainMatch (str, domStr, canonicalize)](#apidoc.element.tough-cookie.domainMatch)
- description and source-code
```javascript
function domainMatch(str, domStr, canonicalize) {
  if (str == null || domStr == null) {
    return null;
  }
  if (canonicalize !== false) {
    str = canonicalDomain(str);
    domStr = canonicalDomain(domStr);
  }

<span class="apidocCodeCommentSpan">  /*
   * "The domain string and the string are identical. (Note that both the
   * domain string and the string will have been canonicalized to lower case at
   * this point)"
   */
</span>  if (str == domStr) {
    return true;
  }

  /* "All of the following [three] conditions hold:" (order adjusted from the RFC) */

  /* "* The string is a host name (i.e., not an IP address)." */
  if (net.isIP(str)) {
    return false;
  }

  /* "* The domain string is a suffix of the string" */
  var idx = str.indexOf(domStr);
  if (idx <= 0) {
    return false; // it's a non-match (-1) or prefix (0)
  }

  // e.g "a.b.c".indexOf("b.c") === 2
  // 5 === 3+2
  if (str.length !== domStr.length + idx) { // it's not a suffix
    return false;
  }

  /* "* The last character of the string that is not included in the domain
  * string is a %x2E (".") character." */
  if (str.substr(idx-1,1) !== '.') {
    return false;
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.formatDate"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>formatDate (date)](#apidoc.element.tough-cookie.formatDate)
- description and source-code
```javascript
function formatDate(date) {
  var d = date.getUTCDate(); d = d >= 10 ? d : '0'+d;
  var h = date.getUTCHours(); h = h >= 10 ? h : '0'+h;
  var m = date.getUTCMinutes(); m = m >= 10 ? m : '0'+m;
  var s = date.getUTCSeconds(); s = s >= 10 ? s : '0'+s;
  return NUM_TO_DAY[date.getUTCDay()] + ', ' +
    d+' '+ NUM_TO_MONTH[date.getUTCMonth()] +' '+ date.getUTCFullYear() +' '+
    h+':'+m+':'+s+' GMT';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.fromJSON"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>fromJSON (str)](#apidoc.element.tough-cookie.fromJSON)
- description and source-code
```javascript
function fromJSON(str) {
  if (!str) {
    return null;
  }

  var obj;
  if (typeof str === 'string') {
    obj = jsonParse(str);
    if (obj instanceof Error) {
      return null;
    }
  } else {
    // assume it's an Object
    obj = str;
  }

  var c = new Cookie();
  for (var i=0; i<Cookie.serializableProperties.length; i++) {
    var prop = Cookie.serializableProperties[i];
    if (obj[prop] === undefined ||
        obj[prop] === Cookie.prototype[prop])
    {
      continue; // leave as prototype default
    }

    if (prop === 'expires' ||
        prop === 'creation' ||
        prop === 'lastAccessed')
    {
      if (obj[prop] === null) {
        c[prop] = null;
      } else {
        c[prop] = obj[prop] == "Infinity" ?
          "Infinity" : new Date(obj[prop]);
      }
    } else {
      c[prop] = obj[prop];
    }
  }

  return c;
}
```
- example usage
```shell
...

### 'parse(cookieString[, options])'

alias for 'Cookie.parse(cookieString[, options])'

### 'fromJSON(string)'

alias for 'Cookie.fromJSON(string)'

### 'getPublicSuffix(hostname)'

Returns the public suffix of this hostname.  The public suffix is the shortest domain-name upon which a cookie can be set.  Returns
 'null' if the hostname cannot have cookies set for it.

For example: 'www.example.com' and 'www.subdomain.example.com' both have public suffix 'example.com'.
...
```

#### <a name="apidoc.element.tough-cookie.getPublicSuffix"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>getPublicSuffix (domain)](#apidoc.element.tough-cookie.getPublicSuffix)
- description and source-code
```javascript
function getPublicSuffix(domain) {
<span class="apidocCodeCommentSpan">  /*!
   * Copyright (c) 2015, Salesforce.com, Inc.
   * All rights reserved.
   *
   * Redistribution and use in source and binary forms, with or without
   * modification, are permitted provided that the following conditions are met:
   *
   * 1. Redistributions of source code must retain the above copyright notice,
   * this list of conditions and the following disclaimer.
   *
   * 2. Redistributions in binary form must reproduce the above copyright notice,
   * this list of conditions and the following disclaimer in the documentation
   * and/or other materials provided with the distribution.
   *
   * 3. Neither the name of Salesforce.com nor the names of its contributors may
   * be used to endorse or promote products derived from this software without
   * specific prior written permission.
   *
   * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
   * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
   * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
   * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
   * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
   * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
   * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
   * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
   * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
   * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
   * POSSIBILITY OF SUCH DAMAGE.
   */
</span>  if (!domain) {
    return null;
  }
  if (domain.match(/^\./)) {
    return null;
  }
  var asciiDomain = punycode.toASCII(domain);
  var converted = false;
  if (asciiDomain !== domain) {
    domain = asciiDomain;
    converted = true;
  }
  if (index[domain]) {
    return null;
  }

  domain = domain.toLowerCase();
  var parts = domain.split('.').reverse();

  var suffix = '';
  var suffixLen = 0;
  for (var i=0; i<parts.length; i++) {
    var part = parts[i];
    var starstr = '*'+suffix;
    var partstr = part+suffix;

    if (index[starstr]) { // star rule matches
      suffixLen = i+1;
      if (index[partstr] === false) { // exception rule matches (NB: false, not undefined)
        suffixLen--;
      }
    } else if (index[partstr]) { // exact match, not exception
      suffixLen = i+1;
    }

    suffix = '.'+partstr;
  }

  if (index['*'+suffix]) { // *.domain exists (e.g. *.kyoto.jp for domain='kyoto.jp');
    return null;
  }

  suffixLen = suffixLen || 1;
  if (parts.length > suffixLen) {
    var publicSuffix = parts.slice(0,suffixLen+1).reverse().join('.');
    return converted ? punycode.toUnicode(publicSuffix) : publicSuffix;
  }

  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.parse"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>parse (str, options)](#apidoc.element.tough-cookie.parse)
- description and source-code
```javascript
function parse(str, options) {
  if (!options || typeof options !== 'object') {
    options = {};
  }
  str = str.trim();

  // We use a regex to parse the "name-value-pair" part of S5.2
  var firstSemi = str.indexOf(';'); // S5.2 step 1
  var pairRe = options.loose ? LOOSE_COOKIE_PAIR : COOKIE_PAIR;
  var result = pairRe.exec(firstSemi === -1 ? str : str.substr(0,firstSemi));

  // Rx satisfies the "the name string is empty" and "lacks a %x3D ("=")"
  // constraints as well as trimming any whitespace.
  if (!result) {
    return;
  }

  var c = new Cookie();
  if (result[1]) {
    c.key = result[2].trim();
  } else {
    c.key = '';
  }
  c.value = result[3].trim();
  if (CONTROL_CHARS.test(c.key) || CONTROL_CHARS.test(c.value)) {
    return;
  }

  if (firstSemi === -1) {
    return c;
  }

  // S5.2.3 "unparsed-attributes consist of the remainder of the set-cookie-string
  // (including the %x3B (";") in question)." plus later on in the same section
  // "discard the first ";" and trim".
  var unparsed = str.slice(firstSemi + 1).trim();

  // "If the unparsed-attributes string is empty, skip the rest of these
  // steps."
  if (unparsed.length === 0) {
    return c;
  }

<span class="apidocCodeCommentSpan">  /*
   * S5.2 says that when looping over the items "[p]rocess the attribute-name
   * and attribute-value according to the requirements in the following
   * subsections" for every item.  Plus, for many of the individual attributes
   * in S5.3 it says to use the "attribute-value of the last attribute in the
   * cookie-attribute-list".  Therefore, in this implementation, we overwrite
   * the previous value.
   */
</span>  var cookie_avs = unparsed.split(';');
  while (cookie_avs.length) {
    var av = cookie_avs.shift().trim();
    if (av.length === 0) { // happens if ";;" appears
      continue;
    }
    var av_sep = av.indexOf('=');
    var av_key, av_value;

    if (av_sep === -1) {
      av_key = av;
      av_value = null;
    } else {
      av_key = av.substr(0,av_sep);
      av_value = av.substr(av_sep+1);
    }

    av_key = av_key.trim().toLowerCase();

    if (av_value) {
      av_value = av_value.trim();
    }

    switch(av_key) {
    case 'expires': // S5.2.1
      if (av_value) {
        var exp = parseDate(av_value);
        // "If the attribute-value failed to parse as a cookie date, ignore the
        // cookie-av."
        if (exp) {
          // over and underflow not realistically a concern: V8's getTime() seems to
          // store something larger than a 32-bit time_t (even with 32-bit node)
          c.expires = exp;
        }
      }
      break;

    case 'max-age': // S5.2.2
      if (av_value) {
        // "If the first character of the attribute-value is not a DIGIT or a "-"
        // character ...[or]... If the remainder of attribute-value contains a
        // non-DIGIT character, ignore the cookie-av."
        if (/^-?[0-9]+$/.test(av_value)) {
          var delta = parseInt(av_value, 10);
          // "If delta-seconds is less than or equal to zero (0), let expiry-time
          // be the earliest representable date and time."
          c.setMaxAge(delta);
        }
      }
      break;

    case 'domain': // S5.2.3
      // "If the attribute-value is empty, the behavior is undefined.  However,
      // the user agent SHOULD ignore the cookie-av entirely."
      if (av_value) {
        // S5.2.3 "Let cookie-domain be the attribute-value without the leading %x2E
        // (".") character."
        var domain = av_value.trim().replace(/^\./, '');
        if (domain) {
          // "Convert the cookie-domain to lower case."
          c.domain = domain.toLowerCase();
        }
      }
      break;

    case 'path': // S5.2.4
      /*
       * "If the attribute-value is empty or if the first character of the
       * attribute-value is not %x2F ("/"):
       *   Let cookie-path be the default-path.
       * Otherwise:
       *   Let cookie-path be the attribute-value."
       *
       * We'll represent the default-path as null since it depends on the
       * context of the parsing.
       */
      c.path = av_value && av_va ...
```
- example usage
```shell
...
[![Build Status](https://travis-ci.org/salesforce/tough-cookie.png?branch=master)](https://travis-ci.org/salesforce/tough-cookie
)

# Synopsis

''' javascript
var tough = require('tough-cookie');
var Cookie = tough.Cookie;
var cookie = Cookie.parse(header);
cookie.value = 'somethingdifferent';
header = cookie.toString();

var cookiejar = new tough.CookieJar();
cookiejar.setCookie(cookie, 'http://currentdomain.example.com/path', cb);
// ...
cookiejar.getCookies('http://example.com/otherpath',function(err,cookies) {
...
```

#### <a name="apidoc.element.tough-cookie.parseDate"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>parseDate (str)](#apidoc.element.tough-cookie.parseDate)
- description and source-code
```javascript
function parseDate(str) {
  if (!str) {
    return;
  }

<span class="apidocCodeCommentSpan">  /* RFC6265 S5.1.1:
   * 2. Process each date-token sequentially in the order the date-tokens
   * appear in the cookie-date
   */
</span>  var tokens = str.split(DATE_DELIM);
  if (!tokens) {
    return;
  }

  var hour = null;
  var minutes = null;
  var seconds = null;
  var day = null;
  var month = null;
  var year = null;

  for (var i=0; i<tokens.length; i++) {
    var token = tokens[i].trim();
    if (!token.length) {
      continue;
    }

    var result;

    /* 2.1. If the found-time flag is not set and the token matches the time
     * production, set the found-time flag and set the hour- value,
     * minute-value, and second-value to the numbers denoted by the digits in
     * the date-token, respectively.  Skip the remaining sub-steps and continue
     * to the next date-token.
     */
    if (seconds === null) {
      result = TIME.exec(token);
      if (result) {
        hour = parseInt(result[1], 10);
        minutes = parseInt(result[2], 10);
        seconds = parseInt(result[3], 10);
        /* RFC6265 S5.1.1.5:
         * [fail if]
         * *  the hour-value is greater than 23,
         * *  the minute-value is greater than 59, or
         * *  the second-value is greater than 59.
         */
        if(hour > 23 || minutes > 59 || seconds > 59) {
          return;
        }

        continue;
      }
    }

    /* 2.2. If the found-day-of-month flag is not set and the date-token matches
     * the day-of-month production, set the found-day-of- month flag and set
     * the day-of-month-value to the number denoted by the date-token.  Skip
     * the remaining sub-steps and continue to the next date-token.
     */
    if (day === null) {
      result = DAY_OF_MONTH.exec(token);
      if (result) {
        day = parseInt(result, 10);
        /* RFC6265 S5.1.1.5:
         * [fail if] the day-of-month-value is less than 1 or greater than 31
         */
        if(day < 1 || day > 31) {
          return;
        }
        continue;
      }
    }

    /* 2.3. If the found-month flag is not set and the date-token matches the
     * month production, set the found-month flag and set the month-value to
     * the month denoted by the date-token.  Skip the remaining sub-steps and
     * continue to the next date-token.
     */
    if (month === null) {
      result = MONTH.exec(token);
      if (result) {
        month = MONTH_TO_NUM[result[1].toLowerCase()];
        continue;
      }
    }

    /* 2.4. If the found-year flag is not set and the date-token matches the year
     * production, set the found-year flag and set the year-value to the number
     * denoted by the date-token.  Skip the remaining sub-steps and continue to
     * the next date-token.
     */
    if (year === null) {
      result = YEAR.exec(token);
      if (result) {
        year = parseInt(result[0], 10);
        /* From S5.1.1:
         * 3.  If the year-value is greater than or equal to 70 and less
         * than or equal to 99, increment the year-value by 1900.
         * 4.  If the year-value is greater than or equal to 0 and less
         * than or equal to 69, increment the year-value by 2000.
         */
        if (70 <= year && year <= 99) {
          year += 1900;
        } else if (0 <= year && year <= 69) {
          year += 2000;
        }

        if (year < 1601) {
          return; // 5. ... the year-value is less than 1601
        }
      }
    }
  }

  if (seconds === null || day === null || month === null || year === null) {
    return; // 5. ... at least one of the found-day-of-month, found-month, found-
            // year, or found-time flags is not set,
  }

  return new Date(Date.UTC(year, month, day, hour, minutes, seconds));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.pathMatch"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>pathMatch (reqPath, cookiePath)](#apidoc.element.tough-cookie.pathMatch)
- description and source-code
```javascript
function pathMatch(reqPath, cookiePath) {
  // "o  The cookie-path and the request-path are identical."
  if (cookiePath === reqPath) {
    return true;
  }

  var idx = reqPath.indexOf(cookiePath);
  if (idx === 0) {
    // "o  The cookie-path is a prefix of the request-path, and the last
    // character of the cookie-path is %x2F ("/")."
    if (cookiePath.substr(-1) === "/") {
      return true;
    }

    // " o  The cookie-path is a prefix of the request-path, and the first
    // character of the request-path that is not included in the cookie- path
    // is a %x2F ("/") character."
    if (reqPath.substr(cookiePath.length, 1) === "/") {
      return true;
    }
  }

  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.permuteDomain"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>permuteDomain (domain)](#apidoc.element.tough-cookie.permuteDomain)
- description and source-code
```javascript
function permuteDomain(domain) {
  var pubSuf = pubsuffix.getPublicSuffix(domain);
  if (!pubSuf) {
    return null;
  }
  if (pubSuf == domain) {
    return [domain];
  }

  var prefix = domain.slice(0, -(pubSuf.length + 1)); // ".example.com"
  var parts = prefix.split('.').reverse();
  var cur = pubSuf;
  var permutations = [cur];
  while (parts.length) {
    cur = parts.shift() + '.' + cur;
    permutations.push(cur);
  }
  return permutations;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.permutePath"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>permutePath (path)](#apidoc.element.tough-cookie.permutePath)
- description and source-code
```javascript
function permutePath(path) {
  if (path === '/') {
    return ['/'];
  }
  if (path.lastIndexOf('/') === path.length-1) {
    path = path.substr(0,path.length-1);
  }
  var permutations = [path];
  while (path.length > 1) {
    var lindex = path.lastIndexOf('/');
    if (lindex === 0) {
      break;
    }
    path = path.substr(0,lindex);
    permutations.push(path);
  }
  permutations.push('/');
  return permutations;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tough-cookie.Cookie"></a>[module tough-cookie.Cookie](#apidoc.module.tough-cookie.Cookie)

#### <a name="apidoc.element.tough-cookie.Cookie.Cookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>Cookie (options)](#apidoc.element.tough-cookie.Cookie.Cookie)
- description and source-code
```javascript
function Cookie(options) {
  options = options || {};

  Object.keys(options).forEach(function(prop) {
    if (Cookie.prototype.hasOwnProperty(prop) &&
        Cookie.prototype[prop] !== options[prop] &&
        prop.substr(0,1) !== '_')
    {
      this[prop] = options[prop];
    }
  }, this);

  this.creation = this.creation || new Date();

  // used to break creation ties in cookieCompare():
  Object.defineProperty(this, 'creationIndex', {
    configurable: false,
    enumerable: false, // important for assert.deepEqual checks
    writable: true,
    value: ++Cookie.cookiesCreated
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.Cookie.fromJSON"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.</span>fromJSON (str)](#apidoc.element.tough-cookie.Cookie.fromJSON)
- description and source-code
```javascript
function fromJSON(str) {
  if (!str) {
    return null;
  }

  var obj;
  if (typeof str === 'string') {
    obj = jsonParse(str);
    if (obj instanceof Error) {
      return null;
    }
  } else {
    // assume it's an Object
    obj = str;
  }

  var c = new Cookie();
  for (var i=0; i<Cookie.serializableProperties.length; i++) {
    var prop = Cookie.serializableProperties[i];
    if (obj[prop] === undefined ||
        obj[prop] === Cookie.prototype[prop])
    {
      continue; // leave as prototype default
    }

    if (prop === 'expires' ||
        prop === 'creation' ||
        prop === 'lastAccessed')
    {
      if (obj[prop] === null) {
        c[prop] = null;
      } else {
        c[prop] = obj[prop] == "Infinity" ?
          "Infinity" : new Date(obj[prop]);
      }
    } else {
      c[prop] = obj[prop];
    }
  }

  return c;
}
```
- example usage
```shell
...

### 'parse(cookieString[, options])'

alias for 'Cookie.parse(cookieString[, options])'

### 'fromJSON(string)'

alias for 'Cookie.fromJSON(string)'

### 'getPublicSuffix(hostname)'

Returns the public suffix of this hostname.  The public suffix is the shortest domain-name upon which a cookie can be set.  Returns
 'null' if the hostname cannot have cookies set for it.

For example: 'www.example.com' and 'www.subdomain.example.com' both have public suffix 'example.com'.
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.parse"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.</span>parse (str, options)](#apidoc.element.tough-cookie.Cookie.parse)
- description and source-code
```javascript
function parse(str, options) {
  if (!options || typeof options !== 'object') {
    options = {};
  }
  str = str.trim();

  // We use a regex to parse the "name-value-pair" part of S5.2
  var firstSemi = str.indexOf(';'); // S5.2 step 1
  var pairRe = options.loose ? LOOSE_COOKIE_PAIR : COOKIE_PAIR;
  var result = pairRe.exec(firstSemi === -1 ? str : str.substr(0,firstSemi));

  // Rx satisfies the "the name string is empty" and "lacks a %x3D ("=")"
  // constraints as well as trimming any whitespace.
  if (!result) {
    return;
  }

  var c = new Cookie();
  if (result[1]) {
    c.key = result[2].trim();
  } else {
    c.key = '';
  }
  c.value = result[3].trim();
  if (CONTROL_CHARS.test(c.key) || CONTROL_CHARS.test(c.value)) {
    return;
  }

  if (firstSemi === -1) {
    return c;
  }

  // S5.2.3 "unparsed-attributes consist of the remainder of the set-cookie-string
  // (including the %x3B (";") in question)." plus later on in the same section
  // "discard the first ";" and trim".
  var unparsed = str.slice(firstSemi + 1).trim();

  // "If the unparsed-attributes string is empty, skip the rest of these
  // steps."
  if (unparsed.length === 0) {
    return c;
  }

<span class="apidocCodeCommentSpan">  /*
   * S5.2 says that when looping over the items "[p]rocess the attribute-name
   * and attribute-value according to the requirements in the following
   * subsections" for every item.  Plus, for many of the individual attributes
   * in S5.3 it says to use the "attribute-value of the last attribute in the
   * cookie-attribute-list".  Therefore, in this implementation, we overwrite
   * the previous value.
   */
</span>  var cookie_avs = unparsed.split(';');
  while (cookie_avs.length) {
    var av = cookie_avs.shift().trim();
    if (av.length === 0) { // happens if ";;" appears
      continue;
    }
    var av_sep = av.indexOf('=');
    var av_key, av_value;

    if (av_sep === -1) {
      av_key = av;
      av_value = null;
    } else {
      av_key = av.substr(0,av_sep);
      av_value = av.substr(av_sep+1);
    }

    av_key = av_key.trim().toLowerCase();

    if (av_value) {
      av_value = av_value.trim();
    }

    switch(av_key) {
    case 'expires': // S5.2.1
      if (av_value) {
        var exp = parseDate(av_value);
        // "If the attribute-value failed to parse as a cookie date, ignore the
        // cookie-av."
        if (exp) {
          // over and underflow not realistically a concern: V8's getTime() seems to
          // store something larger than a 32-bit time_t (even with 32-bit node)
          c.expires = exp;
        }
      }
      break;

    case 'max-age': // S5.2.2
      if (av_value) {
        // "If the first character of the attribute-value is not a DIGIT or a "-"
        // character ...[or]... If the remainder of attribute-value contains a
        // non-DIGIT character, ignore the cookie-av."
        if (/^-?[0-9]+$/.test(av_value)) {
          var delta = parseInt(av_value, 10);
          // "If delta-seconds is less than or equal to zero (0), let expiry-time
          // be the earliest representable date and time."
          c.setMaxAge(delta);
        }
      }
      break;

    case 'domain': // S5.2.3
      // "If the attribute-value is empty, the behavior is undefined.  However,
      // the user agent SHOULD ignore the cookie-av entirely."
      if (av_value) {
        // S5.2.3 "Let cookie-domain be the attribute-value without the leading %x2E
        // (".") character."
        var domain = av_value.trim().replace(/^\./, '');
        if (domain) {
          // "Convert the cookie-domain to lower case."
          c.domain = domain.toLowerCase();
        }
      }
      break;

    case 'path': // S5.2.4
      /*
       * "If the attribute-value is empty or if the first character of the
       * attribute-value is not %x2F ("/"):
       *   Let cookie-path be the default-path.
       * Otherwise:
       *   Let cookie-path be the attribute-value."
       *
       * We'll represent the default-path as null since it depends on the
       * context of the parsing.
       */
      c.path = av_value && av_va ...
```
- example usage
```shell
...
[![Build Status](https://travis-ci.org/salesforce/tough-cookie.png?branch=master)](https://travis-ci.org/salesforce/tough-cookie
)

# Synopsis

''' javascript
var tough = require('tough-cookie');
var Cookie = tough.Cookie;
var cookie = Cookie.parse(header);
cookie.value = 'somethingdifferent';
header = cookie.toString();

var cookiejar = new tough.CookieJar();
cookiejar.setCookie(cookie, 'http://currentdomain.example.com/path', cb);
// ...
cookiejar.getCookies('http://example.com/otherpath',function(err,cookies) {
...
```



# <a name="apidoc.module.tough-cookie.Cookie.prototype"></a>[module tough-cookie.Cookie.prototype](#apidoc.module.tough-cookie.Cookie.prototype)

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.TTL"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>TTL (now)](#apidoc.element.tough-cookie.Cookie.prototype.TTL)
- description and source-code
```javascript
function TTL(now) {
<span class="apidocCodeCommentSpan">  /* RFC6265 S4.1.2.2 If a cookie has both the Max-Age and the Expires
   * attribute, the Max-Age attribute has precedence and controls the
   * expiration date of the cookie.
   * (Concurs with S5.3 step 3)
   */
</span>  if (this.maxAge != null) {
    return this.maxAge<=0 ? 0 : this.maxAge*1000;
  }

  var expires = this.expires;
  if (expires != Infinity) {
    if (!(expires instanceof Date)) {
      expires = parseDate(expires) || Infinity;
    }

    if (expires == Infinity) {
      return Infinity;
    }

    return expires.getTime() - (now || Date.now());
  }

  return Infinity;
}
```
- example usage
```shell
...

Max-Age takes precedence over Expires (as per the RFC). The '.creation' attribute -- or, by default, the 'now' paramter -- is used
 to offset the '.maxAge' attribute.

If Expires ('.expires') is set, that's returned.

Otherwise, 'expiryTime()' returns 'Infinity' and 'expiryDate()' returns a 'Date' object for "Tue, 19 Jan 2038 03:14:07 GMT" (latest
 date that can be expressed by a 32-bit 'time_t'; the common limit for most user-agents).

### '.TTL([now=Date.now()])'

compute the TTL relative to 'now' (milliseconds).  The same precedence rules as for 'expiryTime'/'expiryDate' apply.

The "number" 'Infinity' is returned for cookies without an explicit expiry and '0' is returned if the cookie is expired.  Otherwise
 a time-to-live in milliseconds is returned.

### '.canonicalizedDoman()'
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.canonicalizedDomain"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>canonicalizedDomain ()](#apidoc.element.tough-cookie.Cookie.prototype.canonicalizedDomain)
- description and source-code
```javascript
function canonicalizedDomain() {
  if (this.domain == null) {
    return null;
  }
  return canonicalDomain(this.domain);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.cdomain"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>cdomain ()](#apidoc.element.tough-cookie.Cookie.prototype.cdomain)
- description and source-code
```javascript
function canonicalizedDomain() {
  if (this.domain == null) {
    return null;
  }
  return canonicalDomain(this.domain);
}
```
- example usage
```shell
...

compute the TTL relative to 'now' (milliseconds).  The same precedence rules as for 'expiryTime'/'expiryDate' apply.

The "number" 'Infinity' is returned for cookies without an explicit expiry and '0' is returned if the cookie is expired.  Otherwise
 a time-to-live in milliseconds is returned.

### '.canonicalizedDoman()'

### '.cdomain()'

return the canonicalized '.domain' field.  This is lower-cased and punycode (RFC3490) encoded if the domain has any non-ASCII characters
.

### '.toJSON()'

For convenience in using 'JSON.serialize(cookie)'. Returns a plain-old 'Object' that can be JSON-serialized.
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.clone"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>clone ()](#apidoc.element.tough-cookie.Cookie.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return fromJSON(this.toJSON());
}
```
- example usage
```shell
...

Does the reverse of 'cookie.toJSON()'. If passed a string, will 'JSON.parse()' that first.

Any 'Date' properties (i.e., '.expires', '.creation', and '.lastAccessed') are parsed via 'Date.parse()', not the tough-cookie '
parseDate', since it's JavaScript/JSON-y timestamps being handled at this layer.

Returns 'null' upon JSON parsing error.

### '.clone()'

Does a deep clone of this cookie, exactly implemented as 'Cookie.fromJSON(cookie.toJSON())'.

### '.validate()'

Status: *IN PROGRESS*. Works for a few things, but is by no means comprehensive.
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.cookieString"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>cookieString ()](#apidoc.element.tough-cookie.Cookie.prototype.cookieString)
- description and source-code
```javascript
function cookieString() {
  var val = this.value;
  if (val == null) {
    val = '';
  }
  if (this.key === '') {
    return val;
  }
  return this.key+'='+val;
}
```
- example usage
```shell
...

Receives an options object that can contain any of the above Cookie properties, uses the default for unspecified properties.

### '.toString()'

encode to a Set-Cookie header value.  The Expires cookie field is set using 'formatDate()', but is omitted entirely if '.expires
' is 'Infinity'.

### '.cookieString()'

encode to a Cookie header value (i.e. the '.key' and '.value' properties joined with '=').

### '.setExpires(String)'

sets the expiry based on a date-string passed through 'parseDate()'.  If parseDate returns 'null' (i.e. can't parse this date string
), '.expires' is set to '"Infinity"' (a string) is set.
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.expiryDate"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>expiryDate (now)](#apidoc.element.tough-cookie.Cookie.prototype.expiryDate)
- description and source-code
```javascript
function expiryDate(now) {
  var millisec = this.expiryTime(now);
  if (millisec == Infinity) {
    return new Date(MAX_TIME);
  } else if (millisec == -Infinity) {
    return new Date(MIN_TIME);
  } else {
    return new Date(millisec);
  }
}
```
- example usage
```shell
...

### '.setMaxAge(number)'

sets the maxAge in seconds.  Coerces '-Infinity' to '"-Infinity"' and 'Infinity' to '"Infinity"' so it JSON serializes correctly
.

### '.expiryTime([now=Date.now()])'

### '.expiryDate([now=Date.now()])'

expiryTime() Computes the absolute unix-epoch milliseconds that this cookie expires. expiryDate() works similarly, except it returns
 a 'Date' object.  Note that in both cases the 'now' parameter should be milliseconds.

Max-Age takes precedence over Expires (as per the RFC). The '.creation' attribute -- or, by default, the 'now' paramter -- is used
 to offset the '.maxAge' attribute.

If Expires ('.expires') is set, that's returned.
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.expiryTime"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>expiryTime (now)](#apidoc.element.tough-cookie.Cookie.prototype.expiryTime)
- description and source-code
```javascript
function expiryTime(now) {
  if (this.maxAge != null) {
    var relativeTo = now || this.creation || new Date();
    var age = (this.maxAge <= 0) ? -Infinity : this.maxAge*1000;
    return relativeTo.getTime() + age;
  }

  if (this.expires == Infinity) {
    return Infinity;
  }
  return this.expires.getTime();
}
```
- example usage
```shell
...

sets the expiry based on a date-string passed through 'parseDate()'.  If parseDate returns 'null' (i.e. can't parse this date string
), '.expires' is set to '"Infinity"' (a string) is set.

### '.setMaxAge(number)'

sets the maxAge in seconds.  Coerces '-Infinity' to '"-Infinity"' and 'Infinity' to '"Infinity"' so it JSON serializes correctly
.

### '.expiryTime([now=Date.now()])'

### '.expiryDate([now=Date.now()])'

expiryTime() Computes the absolute unix-epoch milliseconds that this cookie expires. expiryDate() works similarly, except it returns
 a 'Date' object.  Note that in both cases the 'now' parameter should be milliseconds.

Max-Age takes precedence over Expires (as per the RFC). The '.creation' attribute -- or, by default, the 'now' paramter -- is used
 to offset the '.maxAge' attribute.
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.inspect"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>inspect ()](#apidoc.element.tough-cookie.Cookie.prototype.inspect)
- description and source-code
```javascript
function inspect() {
  var now = Date.now();
  return 'Cookie="'+this.toString() +
    '; hostOnly='+(this.hostOnly != null ? this.hostOnly : '?') +
    '; aAge='+(this.lastAccessed ? (now-this.lastAccessed.getTime())+'ms' : '?') +
    '; cAge='+(this.creation ? (now-this.creation.getTime())+'ms' : '?') +
    '"';
}
```
- example usage
```shell
...
MemoryCookieStore.prototype.idx = null;

// Since it's just a struct in RAM, this Store is synchronous
MemoryCookieStore.prototype.synchronous = true;

// force a default depth:
MemoryCookieStore.prototype.inspect = function() {
return "{ idx: "+util.inspect(this.idx, false, 2)+' }';
};

MemoryCookieStore.prototype.findCookie = function(domain, path, key, cb) {
if (!this.idx[domain]) {
  return cb(null,undefined);
}
if (!this.idx[domain][path]) {
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.isPersistent"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>isPersistent ()](#apidoc.element.tough-cookie.Cookie.prototype.isPersistent)
- description and source-code
```javascript
function isPersistent() {
  return (this.maxAge != null || this.expires != Infinity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.setExpires"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>setExpires (exp)](#apidoc.element.tough-cookie.Cookie.prototype.setExpires)
- description and source-code
```javascript
function setExpires(exp) {
  if (exp instanceof Date) {
    this.expires = exp;
  } else {
    this.expires = parseDate(exp) || "Infinity";
  }
}
```
- example usage
```shell
...

encode to a Set-Cookie header value.  The Expires cookie field is set using 'formatDate()', but is omitted entirely if '.expires
' is 'Infinity'.

### '.cookieString()'

encode to a Cookie header value (i.e. the '.key' and '.value' properties joined with '=').

### '.setExpires(String)'

sets the expiry based on a date-string passed through 'parseDate()'.  If parseDate returns 'null' (i.e. can't parse this date string
), '.expires' is set to '"Infinity"' (a string) is set.

### '.setMaxAge(number)'

sets the maxAge in seconds.  Coerces '-Infinity' to '"-Infinity"' and 'Infinity' to '"Infinity"' so it JSON serializes correctly
.
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.setMaxAge"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>setMaxAge (age)](#apidoc.element.tough-cookie.Cookie.prototype.setMaxAge)
- description and source-code
```javascript
function setMaxAge(age) {
  if (age === Infinity || age === -Infinity) {
    this.maxAge = age.toString(); // so JSON.stringify() works
  } else {
    this.maxAge = age;
  }
}
```
- example usage
```shell
...

encode to a Cookie header value (i.e. the '.key' and '.value' properties joined with '=').

### '.setExpires(String)'

sets the expiry based on a date-string passed through 'parseDate()'.  If parseDate returns 'null' (i.e. can't parse this date string
), '.expires' is set to '"Infinity"' (a string) is set.

### '.setMaxAge(number)'

sets the maxAge in seconds.  Coerces '-Infinity' to '"-Infinity"' and 'Infinity' to '"Infinity"' so it JSON serializes correctly
.

### '.expiryTime([now=Date.now()])'

### '.expiryDate([now=Date.now()])'
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>toJSON ()](#apidoc.element.tough-cookie.Cookie.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  var obj = {};

  var props = Cookie.serializableProperties;
  for (var i=0; i<props.length; i++) {
    var prop = props[i];
    if (this[prop] === Cookie.prototype[prop]) {
      continue; // leave as prototype default
    }

    if (prop === 'expires' ||
        prop === 'creation' ||
        prop === 'lastAccessed')
    {
      if (this[prop] === null) {
        obj[prop] = null;
      } else {
        obj[prop] = this[prop] == "Infinity" ? // intentionally not ===
          "Infinity" : this[prop].toISOString();
      }
    } else if (prop === 'maxAge') {
      if (this[prop] !== null) {
        // again, intentionally not ===
        obj[prop] = (this[prop] == Infinity || this[prop] == -Infinity) ?
          this[prop].toString() : this[prop];
      }
    } else {
      if (this[prop] !== Cookie.prototype[prop]) {
        obj[prop] = this[prop];
      }
    }
  }

  return obj;
}
```
- example usage
```shell
...

### '.canonicalizedDoman()'

### '.cdomain()'

return the canonicalized '.domain' field.  This is lower-cased and punycode (RFC3490) encoded if the domain has any non-ASCII characters
.

### '.toJSON()'

For convenience in using 'JSON.serialize(cookie)'. Returns a plain-old 'Object' that can be JSON-serialized.

Any 'Date' properties (i.e., '.expires', '.creation', and '.lastAccessed') are exported in ISO format ('.toISOString()').

**NOTE**: Custom 'Cookie' properties will be discarded. In tough-cookie 1.x, since there was no '.toJSON' method explicitly defined
, all enumerable properties were captured. If you want a property to be serialized, add the property name to the 'Cookie.serializableProperties
' Array.
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.toString"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>toString ()](#apidoc.element.tough-cookie.Cookie.prototype.toString)
- description and source-code
```javascript
function toString() {
  var str = this.cookieString();

  if (this.expires != Infinity) {
    if (this.expires instanceof Date) {
      str += '; Expires='+formatDate(this.expires);
    } else {
      str += '; Expires='+this.expires;
    }
  }

  if (this.maxAge != null && this.maxAge != Infinity) {
    str += '; Max-Age='+this.maxAge;
  }

  if (this.domain && !this.hostOnly) {
    str += '; Domain='+this.domain;
  }
  if (this.path) {
    str += '; Path='+this.path;
  }

  if (this.secure) {
    str += '; Secure';
  }
  if (this.httpOnly) {
    str += '; HttpOnly';
  }
  if (this.extensions) {
    this.extensions.forEach(function(ext) {
      str += '; '+ext;
    });
  }

  return str;
}
```
- example usage
```shell
...
# Synopsis

''' javascript
var tough = require('tough-cookie');
var Cookie = tough.Cookie;
var cookie = Cookie.parse(header);
cookie.value = 'somethingdifferent';
header = cookie.toString();

var cookiejar = new tough.CookieJar();
cookiejar.setCookie(cookie, 'http://currentdomain.example.com/path', cb);
// ...
cookiejar.getCookies('http://example.com/otherpath',function(err,cookies) {
  res.headers['cookie'] = cookies.join('; ');
});
...
```

#### <a name="apidoc.element.tough-cookie.Cookie.prototype.validate"></a>[function <span class="apidocSignatureSpan">tough-cookie.Cookie.prototype.</span>validate ()](#apidoc.element.tough-cookie.Cookie.prototype.validate)
- description and source-code
```javascript
function validate() {
  if (!COOKIE_OCTETS.test(this.value)) {
    return false;
  }
  if (this.expires != Infinity && !(this.expires instanceof Date) && !parseDate(this.expires)) {
    return false;
  }
  if (this.maxAge != null && this.maxAge <= 0) {
    return false; // "Max-Age=" non-zero-digit *DIGIT
  }
  if (this.path != null && !PATH_VALUE.test(this.path)) {
    return false;
  }

  var cdomain = this.cdomain();
  if (cdomain) {
    if (cdomain.match(/\.$/)) {
      return false; // S4.1.2.3 suggests that this is bad. domainMatch() tests confirm this
    }
    var suffix = pubsuffix.getPublicSuffix(cdomain);
    if (suffix == null) { // it's a public suffix
      return false;
    }
  }
  return true;
}
```
- example usage
```shell
...

Returns 'null' upon JSON parsing error.

### '.clone()'

Does a deep clone of this cookie, exactly implemented as 'Cookie.fromJSON(cookie.toJSON())'.

### '.validate()'

Status: *IN PROGRESS*. Works for a few things, but is by no means comprehensive.

validates cookie attributes for semantic correctness.  Useful for "lint" checking any Set-Cookie headers you generate.  For now,
it returns a boolean, but eventually could return a reason string -- you can future-proof with this construct:

''' javascript
if (cookie.validate() === true) {
...
```



# <a name="apidoc.module.tough-cookie.CookieJar"></a>[module tough-cookie.CookieJar](#apidoc.module.tough-cookie.CookieJar)

#### <a name="apidoc.element.tough-cookie.CookieJar.CookieJar"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>CookieJar (store, options)](#apidoc.element.tough-cookie.CookieJar.CookieJar)
- description and source-code
```javascript
function CookieJar(store, options) {
  if (typeof options === "boolean") {
    options = {rejectPublicSuffixes: options};
  } else if (options == null) {
    options = {};
  }
  if (options.rejectPublicSuffixes != null) {
    this.rejectPublicSuffixes = options.rejectPublicSuffixes;
  }
  if (options.looseMode != null) {
    this.enableLooseMode = options.looseMode;
  }

  if (!store) {
    store = new MemoryCookieStore();
  }
  this.store = store;
}
```
- example usage
```shell
...
''' javascript
var tough = require('tough-cookie');
var Cookie = tough.Cookie;
var cookie = Cookie.parse(header);
cookie.value = 'somethingdifferent';
header = cookie.toString();

var cookiejar = new tough.CookieJar();
cookiejar.setCookie(cookie, 'http://currentdomain.example.com/path', cb);
// ...
cookiejar.getCookies('http://example.com/otherpath',function(err,cookies) {
  res.headers['cookie'] = cookies.join('; ');
});
'''
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.deserialize"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.</span>deserialize (strOrObj, store, cb)](#apidoc.element.tough-cookie.CookieJar.deserialize)
- description and source-code
```javascript
deserialize = function (strOrObj, store, cb) {
  if (arguments.length !== 3) {
    // store is optional
    cb = store;
    store = null;
  }

  var serialized;
  if (typeof strOrObj === 'string') {
    serialized = jsonParse(strOrObj);
    if (serialized instanceof Error) {
      return cb(serialized);
    }
  } else {
    serialized = strOrObj;
  }

  var jar = new CookieJar(store, serialized.rejectPublicSuffixes);
  jar._importCookies(serialized, function(err) {
    if (err) {
      return cb(err);
    }
    cb(null, jar);
  });
}
```
- example usage
```shell
...

Sync version of .serialize

### '.toJSON()'

Alias of .serializeSync() for the convenience of 'JSON.stringify(cookiejar)'.

### 'CookieJar.deserialize(serialized, [store], cb(err,object))'

A new Jar is created and the serialized Cookies are added to the underlying store. Each 'Cookie' is added via 'store.putCookie'
in the order in which they appear in the serialization.

The 'store' argument is optional, but should be an instance of 'Store'. By default, a new instance of 'MemoryCookieStore' is created
.

As a convenience, if 'serialized' is a string, it is passed through 'JSON.parse' first. If that throws an error, this is passed
to the callback.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.deserializeSync"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.</span>deserializeSync (strOrObj, store)](#apidoc.element.tough-cookie.CookieJar.deserializeSync)
- description and source-code
```javascript
deserializeSync = function (strOrObj, store) {
  var serialized = typeof strOrObj === 'string' ?
    JSON.parse(strOrObj) : strOrObj;
  var jar = new CookieJar(store, serialized.rejectPublicSuffixes);

  // catch this mistake early:
  if (!jar.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  jar._importCookiesSync(serialized);
  return jar;
}
```
- example usage
```shell
...

A new Jar is created and the serialized Cookies are added to the underlying store. Each 'Cookie' is added via 'store.putCookie'
in the order in which they appear in the serialization.

The 'store' argument is optional, but should be an instance of 'Store'. By default, a new instance of 'MemoryCookieStore' is created
.

As a convenience, if 'serialized' is a string, it is passed through 'JSON.parse' first. If that throws an error, this is passed
to the callback.

### 'CookieJar.deserializeSync(serialized, [store])'

Sync version of '.deserialize'.  _Note_ that the 'store' must be synchronous for this to work.

### 'CookieJar.fromJSON(string)'

Alias of '.deserializeSync' to provide consistency with 'Cookie.fromJSON()'.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.fromJSON"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.</span>fromJSON (strOrObj, store)](#apidoc.element.tough-cookie.CookieJar.fromJSON)
- description and source-code
```javascript
fromJSON = function (strOrObj, store) {
  var serialized = typeof strOrObj === 'string' ?
    JSON.parse(strOrObj) : strOrObj;
  var jar = new CookieJar(store, serialized.rejectPublicSuffixes);

  // catch this mistake early:
  if (!jar.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  jar._importCookiesSync(serialized);
  return jar;
}
```
- example usage
```shell
...

### 'parse(cookieString[, options])'

alias for 'Cookie.parse(cookieString[, options])'

### 'fromJSON(string)'

alias for 'Cookie.fromJSON(string)'

### 'getPublicSuffix(hostname)'

Returns the public suffix of this hostname.  The public suffix is the shortest domain-name upon which a cookie can be set.  Returns
 'null' if the hostname cannot have cookies set for it.

For example: 'www.example.com' and 'www.subdomain.example.com' both have public suffix 'example.com'.
...
```



# <a name="apidoc.module.tough-cookie.CookieJar.prototype"></a>[module tough-cookie.CookieJar.prototype](#apidoc.module.tough-cookie.CookieJar.prototype)

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype._importCookies"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>_importCookies (serialized, cb)](#apidoc.element.tough-cookie.CookieJar.prototype._importCookies)
- description and source-code
```javascript
_importCookies = function (serialized, cb) {
  var jar = this;
  var cookies = serialized.cookies;
  if (!cookies || !Array.isArray(cookies)) {
    return cb(new Error('serialized jar has no cookies array'));
  }

  function putNext(err) {
    if (err) {
      return cb(err);
    }

    if (!cookies.length) {
      return cb(err, jar);
    }

    var cookie;
    try {
      cookie = fromJSON(cookies.shift());
    } catch (e) {
      return cb(e);
    }

    if (cookie === null) {
      return putNext(null); // skip this cookie
    }

    jar.store.putCookie(cookie, putNext);
  }

  putNext();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype._importCookiesSync"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>_importCookiesSync ()](#apidoc.element.tough-cookie.CookieJar.prototype._importCookiesSync)
- description and source-code
```javascript
_importCookiesSync = function () {
  if (!this.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  var args = Array.prototype.slice.call(arguments);
  var syncErr, syncResult;
  args.push(function syncCb(err, result) {
    syncErr = err;
    syncResult = result;
  });
  this[method].apply(this, args);

  if (syncErr) {
    throw syncErr;
  }
  return syncResult;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.clone"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>clone (newStore, cb)](#apidoc.element.tough-cookie.CookieJar.prototype.clone)
- description and source-code
```javascript
clone = function (newStore, cb) {
  if (arguments.length === 1) {
    cb = newStore;
    newStore = null;
  }

  this.serialize(function(err,serialized) {
    if (err) {
      return cb(err);
    }
    CookieJar.deserialize(newStore, serialized, cb);
  });
}
```
- example usage
```shell
...

Does the reverse of 'cookie.toJSON()'. If passed a string, will 'JSON.parse()' that first.

Any 'Date' properties (i.e., '.expires', '.creation', and '.lastAccessed') are parsed via 'Date.parse()', not the tough-cookie '
parseDate', since it's JavaScript/JSON-y timestamps being handled at this layer.

Returns 'null' upon JSON parsing error.

### '.clone()'

Does a deep clone of this cookie, exactly implemented as 'Cookie.fromJSON(cookie.toJSON())'.

### '.validate()'

Status: *IN PROGRESS*. Works for a few things, but is by no means comprehensive.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.cloneSync"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>cloneSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.cloneSync)
- description and source-code
```javascript
cloneSync = function () {
  if (!this.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  var args = Array.prototype.slice.call(arguments);
  var syncErr, syncResult;
  args.push(function syncCb(err, result) {
    syncErr = err;
    syncResult = result;
  });
  this[method].apply(this, args);

  if (syncErr) {
    throw syncErr;
  }
  return syncResult;
}
```
- example usage
```shell
...

### '.clone([store,]cb(err,newJar))'

Produces a deep clone of this jar. Modifications to the original won't affect the clone, and vice versa.

The 'store' argument is optional, but should be an instance of 'Store'. By default, a new instance of 'MemoryCookieStore' is created
. Transferring between store types is supported so long as the source implements '.getAllCookies()' and the destination implements
 '.putCookie()'.

### '.cloneSync([store])'

Synchronous version of '.clone', returning a new 'CookieJar' instance.

The 'store' argument is optional, but must be a _synchronous_ 'Store' instance if specified. If not passed, a new instance of 'MemoryCookieStore
' is used.

The _source_ and _destination_ must both be synchronous 'Store's. If one or both stores are asynchronous, use '.clone' instead.
Recall that 'MemoryCookieStore' supports both synchronous and asynchronous API calls.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.getCookieString"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getCookieString ()](#apidoc.element.tough-cookie.CookieJar.prototype.getCookieString)
- description and source-code
```javascript
getCookieString = function () {
  var args = Array.prototype.slice.call(arguments,0);
  var cb = args.pop();
  var next = function(err,cookies) {
    if (err) {
      cb(err);
    } else {
      cb(null, cookies
        .sort(cookieCompare)
        .map(function(c){
          return c.cookieString();
        })
        .join('; '));
    }
  };
  args.push(next);
  this.getCookies.apply(this,args);
}
```
- example usage
```shell
...

The '.lastAccessed' property of the returned cookies will have been updated.

### '.getCookiesSync(currentUrl, [{options}])'

Synchronous version of 'getCookies'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').

### '.getCookieString(...)'

Accepts the same options as '.getCookies()' but passes a string suitable for a Cookie header rather than an array to the callback
.  Simply maps the 'Cookie' array via '.cookieString()'.

### '.getCookieStringSync(...)'

Synchronous version of 'getCookieString'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.getCookieStringSync"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getCookieStringSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.getCookieStringSync)
- description and source-code
```javascript
getCookieStringSync = function () {
  if (!this.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  var args = Array.prototype.slice.call(arguments);
  var syncErr, syncResult;
  args.push(function syncCb(err, result) {
    syncErr = err;
    syncResult = result;
  });
  this[method].apply(this, args);

  if (syncErr) {
    throw syncErr;
  }
  return syncResult;
}
```
- example usage
```shell
...

Synchronous version of 'getCookies'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').

### '.getCookieString(...)'

Accepts the same options as '.getCookies()' but passes a string suitable for a Cookie header rather than an array to the callback
.  Simply maps the 'Cookie' array via '.cookieString()'.

### '.getCookieStringSync(...)'

Synchronous version of 'getCookieString'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').

### '.getSetCookieStrings(...)'

Returns an array of strings suitable for **Set-Cookie** headers. Accepts the same options as '.getCookies()'.  Simply maps the cookie
 array via '.toString()'.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.getCookies"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getCookies (url, options, cb)](#apidoc.element.tough-cookie.CookieJar.prototype.getCookies)
- description and source-code
```javascript
getCookies = function (url, options, cb) {
  var context = getCookieContext(url);
  if (options instanceof Function) {
    cb = options;
    options = {};
  }

  var host = canonicalDomain(context.hostname);
  var path = context.pathname || '/';

  var secure = options.secure;
  if (secure == null && context.protocol &&
      (context.protocol == 'https:' || context.protocol == 'wss:'))
  {
    secure = true;
  }

  var http = options.http;
  if (http == null) {
    http = true;
  }

  var now = options.now || Date.now();
  var expireCheck = options.expire !== false;
  var allPaths = !!options.allPaths;
  var store = this.store;

  function matchingCookie(c) {
    // "Either:
    //   The cookie's host-only-flag is true and the canonicalized
    //   request-host is identical to the cookie's domain.
    // Or:
    //   The cookie's host-only-flag is false and the canonicalized
    //   request-host domain-matches the cookie's domain."
    if (c.hostOnly) {
      if (c.domain != host) {
        return false;
      }
    } else {
      if (!domainMatch(host, c.domain, false)) {
        return false;
      }
    }

    // "The request-uri's path path-matches the cookie's path."
    if (!allPaths && !pathMatch(path, c.path)) {
      return false;
    }

    // "If the cookie's secure-only-flag is true, then the request-uri's
    // scheme must denote a "secure" protocol"
    if (c.secure && !secure) {
      return false;
    }

    // "If the cookie's http-only-flag is true, then exclude the cookie if the
    // cookie-string is being generated for a "non-HTTP" API"
    if (c.httpOnly && !http) {
      return false;
    }

    // deferred from S5.3
    // non-RFC: allow retention of expired cookies by choice
    if (expireCheck && c.expiryTime() <= now) {
      store.removeCookie(c.domain, c.path, c.key, function(){}); // result ignored
      return false;
    }

    return true;
  }

  store.findCookies(host, allPaths ? null : path, function(err,cookies) {
    if (err) {
      return cb(err);
    }

    cookies = cookies.filter(matchingCookie);

    // sorting of S5.4 part 2
    if (options.sort !== false) {
      cookies = cookies.sort(cookieCompare);
    }

    // S5.4 part 3
    var now = new Date();
    cookies.forEach(function(c) {
      c.lastAccessed = now;
    });
    // TODO persist lastAccessed

    cb(null,cookies);
  });
}
```
- example usage
```shell
...
var cookie = Cookie.parse(header);
cookie.value = 'somethingdifferent';
header = cookie.toString();

var cookiejar = new tough.CookieJar();
cookiejar.setCookie(cookie, 'http://currentdomain.example.com/path', cb);
// ...
cookiejar.getCookies('http://example.com/otherpath',function(err,cookies) {
  res.headers['cookie'] = cookies.join('; ');
});
'''

# Installation

It's _so_ easy!
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.getCookiesSync"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getCookiesSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.getCookiesSync)
- description and source-code
```javascript
getCookiesSync = function () {
  if (!this.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  var args = Array.prototype.slice.call(arguments);
  var syncErr, syncResult;
  args.push(function syncCb(err, result) {
    syncErr = err;
    syncResult = result;
  });
  this[method].apply(this, args);

  if (syncErr) {
    throw syncErr;
  }
  return syncResult;
}
```
- example usage
```shell
...
  * _secure_ - boolean - autodetect from url - indicates if this is a "Secure" API.  If the currentUrl starts with 'https:' or '
wss:' then this is defaulted to 'true', otherwise 'false'.
  * _now_ - Date - default 'new Date()' - what to use for the creation/access time of cookies
  * _expire_ - boolean - default 'true' - perform expiry-time checking of cookies and asynchronously remove expired cookies from
 the store.  Using 'false' will return expired cookies and **not** remove them from the store (which is useful for replaying Set
-Cookie headers, potentially).
  * _allPaths_ - boolean - default 'false' - if 'true', do not scope cookies by path. The default uses RFC-compliant path scoping
. **Note**: may not be supported by the underlying store (the default 'MemoryCookieStore' supports it).

The '.lastAccessed' property of the returned cookies will have been updated.

### '.getCookiesSync(currentUrl, [{options}])'

Synchronous version of 'getCookies'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').

### '.getCookieString(...)'

Accepts the same options as '.getCookies()' but passes a string suitable for a Cookie header rather than an array to the callback
.  Simply maps the 'Cookie' array via '.cookieString()'.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.getSetCookieStrings"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getSetCookieStrings ()](#apidoc.element.tough-cookie.CookieJar.prototype.getSetCookieStrings)
- description and source-code
```javascript
getSetCookieStrings = function () {
  var args = Array.prototype.slice.call(arguments,0);
  var cb = args.pop();
  var next = function(err,cookies) {
    if (err) {
      cb(err);
    } else {
      cb(null, cookies.map(function(c){
        return c.toString();
      }));
    }
  };
  args.push(next);
  this.getCookies.apply(this,args);
}
```
- example usage
```shell
...

Accepts the same options as '.getCookies()' but passes a string suitable for a Cookie header rather than an array to the callback
.  Simply maps the 'Cookie' array via '.cookieString()'.

### '.getCookieStringSync(...)'

Synchronous version of 'getCookieString'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').

### '.getSetCookieStrings(...)'

Returns an array of strings suitable for **Set-Cookie** headers. Accepts the same options as '.getCookies()'.  Simply maps the cookie
 array via '.toString()'.

### '.getSetCookieStringsSync(...)'

Synchronous version of 'getSetCookieStrings'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.getSetCookieStringsSync"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>getSetCookieStringsSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.getSetCookieStringsSync)
- description and source-code
```javascript
getSetCookieStringsSync = function () {
  if (!this.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  var args = Array.prototype.slice.call(arguments);
  var syncErr, syncResult;
  args.push(function syncCb(err, result) {
    syncErr = err;
    syncResult = result;
  });
  this[method].apply(this, args);

  if (syncErr) {
    throw syncErr;
  }
  return syncResult;
}
```
- example usage
```shell
...

Synchronous version of 'getCookieString'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').

### '.getSetCookieStrings(...)'

Returns an array of strings suitable for **Set-Cookie** headers. Accepts the same options as '.getCookies()'.  Simply maps the cookie
 array via '.toString()'.

### '.getSetCookieStringsSync(...)'

Synchronous version of 'getSetCookieStrings'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').

### '.serialize(cb(err,serializedObject))'

Serialize the Jar if the underlying store supports '.getAllCookies'.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.serialize"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>serialize (cb)](#apidoc.element.tough-cookie.CookieJar.prototype.serialize)
- description and source-code
```javascript
serialize = function (cb) {
  var type = this.store.constructor.name;
  if (type === 'Object') {
    type = null;
  }

  // update README.md "Serialization Format" if you change this, please!
  var serialized = {
    // The version of tough-cookie that serialized this jar. Generally a good
    // practice since future versions can make data import decisions based on
    // known past behavior. When/if this matters, use 'semver'.
    version: 'tough-cookie@'+VERSION,

    // add the store type, to make humans happy:
    storeType: type,

    // CookieJar configuration:
    rejectPublicSuffixes: !!this.rejectPublicSuffixes,

    // this gets filled from getAllCookies:
    cookies: []
  };

  if (!(this.store.getAllCookies &&
        typeof this.store.getAllCookies === 'function'))
  {
    return cb(new Error('store does not support getAllCookies and cannot be serialized'));
  }

  this.store.getAllCookies(function(err,cookies) {
    if (err) {
      return cb(err);
    }

    serialized.cookies = cookies.map(function(cookie) {
      // convert to serialized 'raw' cookies
      cookie = (cookie instanceof Cookie) ? cookie.toJSON() : cookie;

      // Remove the index so new ones get assigned during deserialization
      delete cookie.creationIndex;

      return cookie;
    });

    return cb(null, serialized);
  });
}
```
- example usage
```shell
...

### '.cdomain()'

return the canonicalized '.domain' field.  This is lower-cased and punycode (RFC3490) encoded if the domain has any non-ASCII characters
.

### '.toJSON()'

For convenience in using 'JSON.serialize(cookie)'. Returns a plain-old 'Object' that can be JSON-serialized.

Any 'Date' properties (i.e., '.expires', '.creation', and '.lastAccessed') are exported in ISO format ('.toISOString()').

**NOTE**: Custom 'Cookie' properties will be discarded. In tough-cookie 1.x, since there was no '.toJSON' method explicitly defined
, all enumerable properties were captured. If you want a property to be serialized, add the property name to the 'Cookie.serializableProperties
' Array.

### 'Cookie.fromJSON(strOrObj)'
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.serializeSync"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>serializeSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.serializeSync)
- description and source-code
```javascript
serializeSync = function () {
  if (!this.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  var args = Array.prototype.slice.call(arguments);
  var syncErr, syncResult;
  args.push(function syncCb(err, result) {
    syncErr = err;
    syncResult = result;
  });
  this[method].apply(this, args);

  if (syncErr) {
    throw syncErr;
  }
  return syncResult;
}
```
- example usage
```shell
...

Serialize the Jar if the underlying store supports '.getAllCookies'.

**NOTE**: Custom 'Cookie' properties will be discarded. If you want a property to be serialized, add the property name to the 'Cookie
.serializableProperties' Array.

See [Serialization Format].

### '.serializeSync()'

Sync version of .serialize

### '.toJSON()'

Alias of .serializeSync() for the convenience of 'JSON.stringify(cookiejar)'.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.setCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>setCookie (cookie, url, options, cb)](#apidoc.element.tough-cookie.CookieJar.prototype.setCookie)
- description and source-code
```javascript
setCookie = function (cookie, url, options, cb) {
  var err;
  var context = getCookieContext(url);
  if (options instanceof Function) {
    cb = options;
    options = {};
  }

  var host = canonicalDomain(context.hostname);
  var loose = this.enableLooseMode;
  if (options.loose != null) {
    loose = options.loose;
  }

  // S5.3 step 1
  if (!(cookie instanceof Cookie)) {
    cookie = Cookie.parse(cookie, { loose: loose });
  }
  if (!cookie) {
    err = new Error("Cookie failed to parse");
    return cb(options.ignoreError ? null : err);
  }

  // S5.3 step 2
  var now = options.now || new Date(); // will assign later to save effort in the face of errors

  // S5.3 step 3: NOOP; persistent-flag and expiry-time is handled by getCookie()

  // S5.3 step 4: NOOP; domain is null by default

  // S5.3 step 5: public suffixes
  if (this.rejectPublicSuffixes && cookie.domain) {
    var suffix = pubsuffix.getPublicSuffix(cookie.cdomain());
    if (suffix == null) { // e.g. "com"
      err = new Error("Cookie has domain set to a public suffix");
      return cb(options.ignoreError ? null : err);
    }
  }

  // S5.3 step 6:
  if (cookie.domain) {
    if (!domainMatch(host, cookie.cdomain(), false)) {
      err = new Error("Cookie not in this host's domain. Cookie:"+cookie.cdomain()+" Request:"+host);
      return cb(options.ignoreError ? null : err);
    }

    if (cookie.hostOnly == null) { // don't reset if already set
      cookie.hostOnly = false;
    }

  } else {
    cookie.hostOnly = true;
    cookie.domain = host;
  }

  //S5.2.4 If the attribute-value is empty or if the first character of the
  //attribute-value is not %x2F ("/"):
  //Let cookie-path be the default-path.
  if (!cookie.path || cookie.path[0] !== '/') {
    cookie.path = defaultPath(context.pathname);
    cookie.pathIsDefault = true;
  }

  // S5.3 step 8: NOOP; secure attribute
  // S5.3 step 9: NOOP; httpOnly attribute

  // S5.3 step 10
  if (options.http === false && cookie.httpOnly) {
    err = new Error("Cookie is HttpOnly and this isn't an HTTP API");
    return cb(options.ignoreError ? null : err);
  }

  var store = this.store;

  if (!store.updateCookie) {
    store.updateCookie = function(oldCookie, newCookie, cb) {
      this.putCookie(newCookie, cb);
    };
  }

  function withCookie(err, oldCookie) {
    if (err) {
      return cb(err);
    }

    var next = function(err) {
      if (err) {
        return cb(err);
      } else {
        cb(null, cookie);
      }
    };

    if (oldCookie) {
      // S5.3 step 11 - "If the cookie store contains a cookie with the same name,
      // domain, and path as the newly created cookie:"
      if (options.http === false && oldCookie.httpOnly) { // step 11.2
        err = new Error("old Cookie is HttpOnly and this isn't an HTTP API");
        return cb(options.ignoreError ? null : err);
      }
      cookie.creation = oldCookie.creation; // step 11.3
      cookie.creationIndex = oldCookie.creationIndex; // preserve tie-breaker
      cookie.lastAccessed = now;
      // Step 11.4 (delete cookie) is implied by just setting the new one:
      store.updateCookie(oldCookie, cookie, next); // step 12

    } else {
      cookie.creation = cookie.lastAccessed = now;
      store.putCookie(cookie, next); // step 12
    }
  }

  store.findCookie(cookie.domain, cookie.path, cookie.key, withCookie);
}
```
- example usage
```shell
...
var tough = require('tough-cookie');
var Cookie = tough.Cookie;
var cookie = Cookie.parse(header);
cookie.value = 'somethingdifferent';
header = cookie.toString();

var cookiejar = new tough.CookieJar();
cookiejar.setCookie(cookie, 'http://currentdomain.example.com/path', cb);
// ...
cookiejar.getCookies('http://example.com/otherpath',function(err,cookies) {
  res.headers['cookie'] = cookies.join('; ');
});
'''

# Installation
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.setCookieSync"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>setCookieSync ()](#apidoc.element.tough-cookie.CookieJar.prototype.setCookieSync)
- description and source-code
```javascript
setCookieSync = function () {
  if (!this.store.synchronous) {
    throw new Error('CookieJar store is not synchronous; use async API instead.');
  }

  var args = Array.prototype.slice.call(arguments);
  var syncErr, syncResult;
  args.push(function syncCb(err, result) {
    syncErr = err;
    syncResult = result;
  });
  this[method].apply(this, args);

  if (syncErr) {
    throw syncErr;
  }
  return syncResult;
}
```
- example usage
```shell
...
  * _http_ - boolean - default 'true' - indicates if this is an HTTP or non-HTTP API.  Affects HttpOnly cookies.
  * _secure_ - boolean - autodetect from url - indicates if this is a "Secure" API.  If the currentUrl starts with 'https:' or '
wss:' then this is defaulted to 'true', otherwise 'false'.
  * _now_ - Date - default 'new Date()' - what to use for the creation/access time of cookies
  * _ignoreError_ - boolean - default 'false' - silently ignore things like parse errors and invalid domains.  'Store' errors aren
't ignored by this option.

As per the RFC, the '.hostOnly' property is set if there was no "Domain=" parameter in the cookie string (or '.domain' was null
on the Cookie object).  The '.domain' property is set to the fully-qualified hostname of 'currentUrl' in this case.  Matching this
 cookie requires an exact hostname match (not a 'domainMatch' as per usual).

### '.setCookieSync(cookieOrString, currentUrl, [{options}])'

Synchronous version of 'setCookie'; only works with synchronous stores (e.g. the default 'MemoryCookieStore').

### '.getCookies(currentUrl, [{options},] cb(err,cookies))'

Retrieve the list of cookies that can be sent in a Cookie header for the current url.
...
```

#### <a name="apidoc.element.tough-cookie.CookieJar.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">tough-cookie.CookieJar.prototype.</span>toJSON ()](#apidoc.element.tough-cookie.CookieJar.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.serializeSync();
}
```
- example usage
```shell
...

### '.canonicalizedDoman()'

### '.cdomain()'

return the canonicalized '.domain' field.  This is lower-cased and punycode (RFC3490) encoded if the domain has any non-ASCII characters
.

### '.toJSON()'

For convenience in using 'JSON.serialize(cookie)'. Returns a plain-old 'Object' that can be JSON-serialized.

Any 'Date' properties (i.e., '.expires', '.creation', and '.lastAccessed') are exported in ISO format ('.toISOString()').

**NOTE**: Custom 'Cookie' properties will be discarded. In tough-cookie 1.x, since there was no '.toJSON' method explicitly defined
, all enumerable properties were captured. If you want a property to be serialized, add the property name to the 'Cookie.serializableProperties
' Array.
...
```



# <a name="apidoc.module.tough-cookie.MemoryCookieStore"></a>[module tough-cookie.MemoryCookieStore](#apidoc.module.tough-cookie.MemoryCookieStore)

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.MemoryCookieStore"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>MemoryCookieStore ()](#apidoc.element.tough-cookie.MemoryCookieStore.MemoryCookieStore)
- description and source-code
```javascript
function MemoryCookieStore() {
  Store.call(this);
  this.idx = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.super_"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.</span>super_ ()](#apidoc.element.tough-cookie.MemoryCookieStore.super_)
- description and source-code
```javascript
function Store() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tough-cookie.MemoryCookieStore.prototype"></a>[module tough-cookie.MemoryCookieStore.prototype](#apidoc.module.tough-cookie.MemoryCookieStore.prototype)

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.prototype.findCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>findCookie (domain, path, key, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.findCookie)
- description and source-code
```javascript
findCookie = function (domain, path, key, cb) {
  if (!this.idx[domain]) {
    return cb(null,undefined);
  }
  if (!this.idx[domain][path]) {
    return cb(null,undefined);
  }
  return cb(null,this.idx[domain][path][key]||null);
}
```
- example usage
```shell
...

Stores are asynchronous by default, but if 'store.synchronous' is set to 'true', then the '*Sync' methods on the of the containing
 'CookieJar' can be used (however, the continuation-passing style

All 'domain' parameters will have been normalized before calling.

The Cookie store must have all of the following methods.

### 'store.findCookie(domain, path, key, cb(err,cookie))'

Retrieve a cookie with the given domain, path and key (a.k.a. name).  The RFC maintains that exactly one of these cookies should
 exist in a store.  If the store is using versioning, this means that the latest/newest such cookie should be returned.

Callback takes an error and the resulting 'Cookie' object.  If no cookie is found then 'null' MUST be passed instead (i.e. not an
 error).

### 'store.findCookies(domain, path, cb(err,cookies))'
...
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.prototype.findCookies"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>findCookies (domain, path, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.findCookies)
- description and source-code
```javascript
findCookies = function (domain, path, cb) {
  var results = [];
  if (!domain) {
    return cb(null,[]);
  }

  var pathMatcher;
  if (!path) {
    // null means "all paths"
    pathMatcher = function matchAll(domainIndex) {
      for (var curPath in domainIndex) {
        var pathIndex = domainIndex[curPath];
        for (var key in pathIndex) {
          results.push(pathIndex[key]);
        }
      }
    };

  } else {
    pathMatcher = function matchRFC(domainIndex) {
       //NOTE: we should use path-match algorithm from S5.1.4 here
       //(see : https://github.com/ChromiumWebApps/chromium/blob/b3d3b4da8bb94c1b2e061600df106d590fda3620/net/cookies/canonical_cookie
.cc#L299)
       Object.keys(domainIndex).forEach(function (cookiePath) {
         if (pathMatch(path, cookiePath)) {
           var pathIndex = domainIndex[cookiePath];

           for (var key in pathIndex) {
             results.push(pathIndex[key]);
           }
         }
       });
     };
  }

  var domains = permuteDomain(domain) || [domain];
  var idx = this.idx;
  domains.forEach(function(curDomain) {
    var domainIndex = idx[curDomain];
    if (!domainIndex) {
      return;
    }
    pathMatcher(domainIndex);
  });

  cb(null,results);
}
```
- example usage
```shell
...

### 'store.findCookie(domain, path, key, cb(err,cookie))'

Retrieve a cookie with the given domain, path and key (a.k.a. name).  The RFC maintains that exactly one of these cookies should
 exist in a store.  If the store is using versioning, this means that the latest/newest such cookie should be returned.

Callback takes an error and the resulting 'Cookie' object.  If no cookie is found then 'null' MUST be passed instead (i.e. not an
 error).

### 'store.findCookies(domain, path, cb(err,cookies))'

Locates cookies matching the given domain and path.  This is most often called in the context of 'cookiejar.getCookies()' above.

If no cookies are found, the callback MUST be passed an empty array.

The resulting list will be checked for applicability to the current request according to the RFC (domain-match, path-match, http
-only-flag, secure-flag, expiry, etc.), so it's OK to use an optimistic search algorithm when implementing this method.  However
, the search algorithm used SHOULD try to find cookies that 'domainMatch()' the domain and 'pathMatch()' the path in order to limit
 the amount of checking that needs to be done.
...
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.prototype.getAllCookies"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>getAllCookies (cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.getAllCookies)
- description and source-code
```javascript
getAllCookies = function (cb) {
  var cookies = [];
  var idx = this.idx;

  var domains = Object.keys(idx);
  domains.forEach(function(domain) {
    var paths = Object.keys(idx[domain]);
    paths.forEach(function(path) {
      var keys = Object.keys(idx[domain][path]);
      keys.forEach(function(key) {
        if (key !== null) {
          cookies.push(idx[domain][path][key]);
        }
      });
    });
  });

  // Sort by creationIndex so deserializing retains the creation order.
  // When implementing your own store, this SHOULD retain the order too
  cookies.sort(function(a,b) {
    return (a.creationIndex||0) - (b.creationIndex||0);
  });

  cb(null, cookies);
}
```
- example usage
```shell
...

Alias of '.deserializeSync' to provide consistency with 'Cookie.fromJSON()'.

### '.clone([store,]cb(err,newJar))'

Produces a deep clone of this jar. Modifications to the original won't affect the clone, and vice versa.

The 'store' argument is optional, but should be an instance of 'Store'. By default, a new instance of 'MemoryCookieStore' is created
. Transferring between store types is supported so long as the source implements '.getAllCookies()' and the destination implements
 '.putCookie()'.

### '.cloneSync([store])'

Synchronous version of '.clone', returning a new 'CookieJar' instance.

The 'store' argument is optional, but must be a _synchronous_ 'Store' instance if specified. If not passed, a new instance of 'MemoryCookieStore
' is used.
...
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.prototype.inspect"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>inspect ()](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.inspect)
- description and source-code
```javascript
inspect = function () {
  return "{ idx: "+util.inspect(this.idx, false, 2)+' }';
}
```
- example usage
```shell
...
MemoryCookieStore.prototype.idx = null;

// Since it's just a struct in RAM, this Store is synchronous
MemoryCookieStore.prototype.synchronous = true;

// force a default depth:
MemoryCookieStore.prototype.inspect = function() {
return "{ idx: "+util.inspect(this.idx, false, 2)+' }';
};

MemoryCookieStore.prototype.findCookie = function(domain, path, key, cb) {
if (!this.idx[domain]) {
  return cb(null,undefined);
}
if (!this.idx[domain][path]) {
...
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.prototype.putCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>putCookie (cookie, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.putCookie)
- description and source-code
```javascript
putCookie = function (cookie, cb) {
  if (!this.idx[cookie.domain]) {
    this.idx[cookie.domain] = {};
  }
  if (!this.idx[cookie.domain][cookie.path]) {
    this.idx[cookie.domain][cookie.path] = {};
  }
  this.idx[cookie.domain][cookie.path][cookie.key] = cookie;
  cb(null);
}
```
- example usage
```shell
...

Alias of '.deserializeSync' to provide consistency with 'Cookie.fromJSON()'.

### '.clone([store,]cb(err,newJar))'

Produces a deep clone of this jar. Modifications to the original won't affect the clone, and vice versa.

The 'store' argument is optional, but should be an instance of 'Store'. By default, a new instance of 'MemoryCookieStore' is created
. Transferring between store types is supported so long as the source implements '.getAllCookies()' and the destination implements
 '.putCookie()'.

### '.cloneSync([store])'

Synchronous version of '.clone', returning a new 'CookieJar' instance.

The 'store' argument is optional, but must be a _synchronous_ 'Store' instance if specified. If not passed, a new instance of 'MemoryCookieStore
' is used.
...
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.prototype.removeCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>removeCookie (domain, path, key, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.removeCookie)
- description and source-code
```javascript
removeCookie = function (domain, path, key, cb) {
  if (this.idx[domain] && this.idx[domain][path] && this.idx[domain][path][key]) {
    delete this.idx[domain][path][key];
  }
  cb(null);
}
```
- example usage
```shell
...

Stores may wish to optimize changing the '.value' of the cookie in the store versus storing a new cookie.  If the implementation
 doesn't define this method a stub that calls 'putCookie(newCookie,cb)' will be added to the store object.

The 'newCookie' and 'oldCookie' objects MUST NOT be modified.

Pass an error if the newCookie cannot be stored.

### 'store.removeCookie(domain, path, key, cb(err))'

Remove a cookie from the store (see notes on 'findCookie' about the uniqueness constraint).

The implementation MUST NOT pass an error if the cookie doesn't exist; only pass an error due to the failure to remove an existing
 cookie.

### 'store.removeCookies(domain, path, cb(err))'
...
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.prototype.removeCookies"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>removeCookies (domain, path, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.removeCookies)
- description and source-code
```javascript
removeCookies = function (domain, path, cb) {
  if (this.idx[domain]) {
    if (path) {
      delete this.idx[domain][path];
    } else {
      delete this.idx[domain];
    }
  }
  return cb(null);
}
```
- example usage
```shell
...

### 'store.removeCookie(domain, path, key, cb(err))'

Remove a cookie from the store (see notes on 'findCookie' about the uniqueness constraint).

The implementation MUST NOT pass an error if the cookie doesn't exist; only pass an error due to the failure to remove an existing
 cookie.

### 'store.removeCookies(domain, path, cb(err))'

Removes matching cookies from the store.  The 'path' parameter is optional, and if missing means all paths in a domain should be
 removed.

Pass an error ONLY if removing any existing cookies failed.

### 'store.getAllCookies(cb(err, cookies))'
...
```

#### <a name="apidoc.element.tough-cookie.MemoryCookieStore.prototype.updateCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.MemoryCookieStore.prototype.</span>updateCookie (oldCookie, newCookie, cb)](#apidoc.element.tough-cookie.MemoryCookieStore.prototype.updateCookie)
- description and source-code
```javascript
updateCookie = function (oldCookie, newCookie, cb) {
  // updateCookie() may avoid updating cookies that are identical.  For example,
  // lastAccessed may not be important to some stores and an equality
  // comparison could exclude that field.
  this.putCookie(newCookie,cb);
}
```
- example usage
```shell
...

Adds a new cookie to the store.  The implementation SHOULD replace any existing cookie with the same '.domain', '.path', and '.key
' properties -- depending on the nature of the implementation, it's possible that between the call to 'fetchCookie' and 'putCookie
' that a duplicate 'putCookie' can occur.

The 'cookie' object MUST NOT be modified; the caller will have already updated the '.creation' and '.lastAccessed' properties.

Pass an error if the cookie cannot be stored.

### 'store.updateCookie(oldCookie, newCookie, cb(err))'

Update an existing cookie.  The implementation MUST update the '.value' for a cookie with the same 'domain', '.path' and '.key'.
The implementation SHOULD check that the old value in the store is equivalent to 'oldCookie' - how the conflict is resolved is up
 to the store.

The '.lastAccessed' property will always be different between the two objects (to the precision possible via JavaScript's clock).
Both '.creation' and '.creationIndex' are guaranteed to be the same.  Stores MAY ignore or defer the '.lastAccessed' change at the
 cost of affecting how cookies are selected for automatic deletion (e.g., least-recently-used, which is up to the store to implement
).

Stores may wish to optimize changing the '.value' of the cookie in the store versus storing a new cookie.  If the implementation
 doesn't define this method a stub that calls 'putCookie(newCookie,cb)' will be added to the store object.
...
```



# <a name="apidoc.module.tough-cookie.Store"></a>[module tough-cookie.Store](#apidoc.module.tough-cookie.Store)

#### <a name="apidoc.element.tough-cookie.Store.Store"></a>[function <span class="apidocSignatureSpan">tough-cookie.</span>Store ()](#apidoc.element.tough-cookie.Store.Store)
- description and source-code
```javascript
function Store() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tough-cookie.Store.prototype"></a>[module tough-cookie.Store.prototype](#apidoc.module.tough-cookie.Store.prototype)

#### <a name="apidoc.element.tough-cookie.Store.prototype.findCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>findCookie (domain, path, key, cb)](#apidoc.element.tough-cookie.Store.prototype.findCookie)
- description and source-code
```javascript
findCookie = function (domain, path, key, cb) {
  throw new Error('findCookie is not implemented');
}
```
- example usage
```shell
...

Stores are asynchronous by default, but if 'store.synchronous' is set to 'true', then the '*Sync' methods on the of the containing
 'CookieJar' can be used (however, the continuation-passing style

All 'domain' parameters will have been normalized before calling.

The Cookie store must have all of the following methods.

### 'store.findCookie(domain, path, key, cb(err,cookie))'

Retrieve a cookie with the given domain, path and key (a.k.a. name).  The RFC maintains that exactly one of these cookies should
 exist in a store.  If the store is using versioning, this means that the latest/newest such cookie should be returned.

Callback takes an error and the resulting 'Cookie' object.  If no cookie is found then 'null' MUST be passed instead (i.e. not an
 error).

### 'store.findCookies(domain, path, cb(err,cookies))'
...
```

#### <a name="apidoc.element.tough-cookie.Store.prototype.findCookies"></a>[function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>findCookies (domain, path, cb)](#apidoc.element.tough-cookie.Store.prototype.findCookies)
- description and source-code
```javascript
findCookies = function (domain, path, cb) {
  throw new Error('findCookies is not implemented');
}
```
- example usage
```shell
...

### 'store.findCookie(domain, path, key, cb(err,cookie))'

Retrieve a cookie with the given domain, path and key (a.k.a. name).  The RFC maintains that exactly one of these cookies should
 exist in a store.  If the store is using versioning, this means that the latest/newest such cookie should be returned.

Callback takes an error and the resulting 'Cookie' object.  If no cookie is found then 'null' MUST be passed instead (i.e. not an
 error).

### 'store.findCookies(domain, path, cb(err,cookies))'

Locates cookies matching the given domain and path.  This is most often called in the context of 'cookiejar.getCookies()' above.

If no cookies are found, the callback MUST be passed an empty array.

The resulting list will be checked for applicability to the current request according to the RFC (domain-match, path-match, http
-only-flag, secure-flag, expiry, etc.), so it's OK to use an optimistic search algorithm when implementing this method.  However
, the search algorithm used SHOULD try to find cookies that 'domainMatch()' the domain and 'pathMatch()' the path in order to limit
 the amount of checking that needs to be done.
...
```

#### <a name="apidoc.element.tough-cookie.Store.prototype.getAllCookies"></a>[function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>getAllCookies (cb)](#apidoc.element.tough-cookie.Store.prototype.getAllCookies)
- description and source-code
```javascript
getAllCookies = function (cb) {
  throw new Error('getAllCookies is not implemented (therefore jar cannot be serialized)');
}
```
- example usage
```shell
...

Alias of '.deserializeSync' to provide consistency with 'Cookie.fromJSON()'.

### '.clone([store,]cb(err,newJar))'

Produces a deep clone of this jar. Modifications to the original won't affect the clone, and vice versa.

The 'store' argument is optional, but should be an instance of 'Store'. By default, a new instance of 'MemoryCookieStore' is created
. Transferring between store types is supported so long as the source implements '.getAllCookies()' and the destination implements
 '.putCookie()'.

### '.cloneSync([store])'

Synchronous version of '.clone', returning a new 'CookieJar' instance.

The 'store' argument is optional, but must be a _synchronous_ 'Store' instance if specified. If not passed, a new instance of 'MemoryCookieStore
' is used.
...
```

#### <a name="apidoc.element.tough-cookie.Store.prototype.putCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>putCookie (cookie, cb)](#apidoc.element.tough-cookie.Store.prototype.putCookie)
- description and source-code
```javascript
putCookie = function (cookie, cb) {
  throw new Error('putCookie is not implemented');
}
```
- example usage
```shell
...

Alias of '.deserializeSync' to provide consistency with 'Cookie.fromJSON()'.

### '.clone([store,]cb(err,newJar))'

Produces a deep clone of this jar. Modifications to the original won't affect the clone, and vice versa.

The 'store' argument is optional, but should be an instance of 'Store'. By default, a new instance of 'MemoryCookieStore' is created
. Transferring between store types is supported so long as the source implements '.getAllCookies()' and the destination implements
 '.putCookie()'.

### '.cloneSync([store])'

Synchronous version of '.clone', returning a new 'CookieJar' instance.

The 'store' argument is optional, but must be a _synchronous_ 'Store' instance if specified. If not passed, a new instance of 'MemoryCookieStore
' is used.
...
```

#### <a name="apidoc.element.tough-cookie.Store.prototype.removeCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>removeCookie (domain, path, key, cb)](#apidoc.element.tough-cookie.Store.prototype.removeCookie)
- description and source-code
```javascript
removeCookie = function (domain, path, key, cb) {
  throw new Error('removeCookie is not implemented');
}
```
- example usage
```shell
...

Stores may wish to optimize changing the '.value' of the cookie in the store versus storing a new cookie.  If the implementation
 doesn't define this method a stub that calls 'putCookie(newCookie,cb)' will be added to the store object.

The 'newCookie' and 'oldCookie' objects MUST NOT be modified.

Pass an error if the newCookie cannot be stored.

### 'store.removeCookie(domain, path, key, cb(err))'

Remove a cookie from the store (see notes on 'findCookie' about the uniqueness constraint).

The implementation MUST NOT pass an error if the cookie doesn't exist; only pass an error due to the failure to remove an existing
 cookie.

### 'store.removeCookies(domain, path, cb(err))'
...
```

#### <a name="apidoc.element.tough-cookie.Store.prototype.removeCookies"></a>[function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>removeCookies (domain, path, cb)](#apidoc.element.tough-cookie.Store.prototype.removeCookies)
- description and source-code
```javascript
removeCookies = function (domain, path, cb) {
  throw new Error('removeCookies is not implemented');
}
```
- example usage
```shell
...

### 'store.removeCookie(domain, path, key, cb(err))'

Remove a cookie from the store (see notes on 'findCookie' about the uniqueness constraint).

The implementation MUST NOT pass an error if the cookie doesn't exist; only pass an error due to the failure to remove an existing
 cookie.

### 'store.removeCookies(domain, path, cb(err))'

Removes matching cookies from the store.  The 'path' parameter is optional, and if missing means all paths in a domain should be
 removed.

Pass an error ONLY if removing any existing cookies failed.

### 'store.getAllCookies(cb(err, cookies))'
...
```

#### <a name="apidoc.element.tough-cookie.Store.prototype.updateCookie"></a>[function <span class="apidocSignatureSpan">tough-cookie.Store.prototype.</span>updateCookie (oldCookie, newCookie, cb)](#apidoc.element.tough-cookie.Store.prototype.updateCookie)
- description and source-code
```javascript
updateCookie = function (oldCookie, newCookie, cb) {
  // recommended default implementation:
  // return this.putCookie(newCookie, cb);
  throw new Error('updateCookie is not implemented');
}
```
- example usage
```shell
...

Adds a new cookie to the store.  The implementation SHOULD replace any existing cookie with the same '.domain', '.path', and '.key
' properties -- depending on the nature of the implementation, it's possible that between the call to 'fetchCookie' and 'putCookie
' that a duplicate 'putCookie' can occur.

The 'cookie' object MUST NOT be modified; the caller will have already updated the '.creation' and '.lastAccessed' properties.

Pass an error if the cookie cannot be stored.

### 'store.updateCookie(oldCookie, newCookie, cb(err))'

Update an existing cookie.  The implementation MUST update the '.value' for a cookie with the same 'domain', '.path' and '.key'.
The implementation SHOULD check that the old value in the store is equivalent to 'oldCookie' - how the conflict is resolved is up
 to the store.

The '.lastAccessed' property will always be different between the two objects (to the precision possible via JavaScript's clock).
Both '.creation' and '.creationIndex' are guaranteed to be the same.  Stores MAY ignore or defer the '.lastAccessed' change at the
 cost of affecting how cookies are selected for automatic deletion (e.g., least-recently-used, which is up to the store to implement
).

Stores may wish to optimize changing the '.value' of the cookie in the store versus storing a new cookie.  If the implementation
 doesn't define this method a stub that calls 'putCookie(newCookie,cb)' will be added to the store object.
...
```



# <a name="apidoc.module.tough-cookie.memstore"></a>[module tough-cookie.memstore](#apidoc.module.tough-cookie.memstore)

#### <a name="apidoc.element.tough-cookie.memstore.MemoryCookieStore"></a>[function <span class="apidocSignatureSpan">tough-cookie.memstore.</span>MemoryCookieStore ()](#apidoc.element.tough-cookie.memstore.MemoryCookieStore)
- description and source-code
```javascript
function MemoryCookieStore() {
  Store.call(this);
  this.idx = {};
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
