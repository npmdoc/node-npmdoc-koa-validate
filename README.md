# api documentation for  [koa-validate (v1.0.7)](https://github.com/RocksonZeta/koa-validate#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-koa-validate.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-koa-validate) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-koa-validate.svg)](https://travis-ci.org/npmdoc/node-npmdoc-koa-validate)
#### A koa params validate middleware.

[![NPM](https://nodei.co/npm/koa-validate.png?downloads=true)](https://www.npmjs.com/package/koa-validate)

[![apidoc](https://npmdoc.github.io/node-npmdoc-koa-validate/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-koa-validate_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-koa-validate/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-koa-validate/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-koa-validate/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/RocksonZeta/koa-validate/issues"
    },
    "dependencies": {
        "json-path": "^0.1.3",
        "validator": "^5.2.0"
    },
    "description": "A koa params validate middleware.",
    "devDependencies": {
        "coveralls": "*",
        "istanbul-harmony": "0",
        "koa": "*",
        "koa-body": "*",
        "koa-router": "*",
        "mocha": "*",
        "mocha-lcov-reporter": "*",
        "should": "*",
        "supertest": "^0.13.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0b7dd3feee83cae1b4694fa06376477d945eb430",
        "tarball": "https://registry.npmjs.org/koa-validate/-/koa-validate-1.0.7.tgz"
    },
    "engines": {
        "node": ">= 0.11.9"
    },
    "gitHead": "a44b4fb8738595530f729e5d9407b725c1a49537",
    "homepage": "https://github.com/RocksonZeta/koa-validate#readme",
    "keywords": [
        "web",
        "koa",
        "koa-validate",
        "validate",
        "validator",
        "format",
        "middleware"
    ],
    "license": "MIT",
    "main": "validate.js",
    "maintainers": [
        {
            "name": "rocksonzeta",
            "email": "RocksonZeta@gmail.com"
        }
    ],
    "name": "koa-validate",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/RocksonZeta/koa-validate.git"
    },
    "scripts": {
        "test": "NODE_ENV=test mocha --harmony --require should --reporter spec",
        "test-cov": "NODE_ENV=test node --harmony ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha -- --require should",
        "test-travis": "NODE_ENV=test node --harmony ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha --report lcovonly -- --require should"
    },
    "version": "1.0.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module koa-validate](#apidoc.module.koa-validate)
1.  [function <span class="apidocSignatureSpan">koa-validate.</span>FileValidator (context, key, value, exists, params, deleteOnCheckFailed)](#apidoc.element.koa-validate.FileValidator)
1.  [function <span class="apidocSignatureSpan">koa-validate.</span>Validator (context, key, value, exists, params , goOn)](#apidoc.element.koa-validate.Validator)
1.  object <span class="apidocSignatureSpan">koa-validate.</span>FileValidator.prototype
1.  object <span class="apidocSignatureSpan">koa-validate.</span>Validator.prototype

#### [module koa-validate.FileValidator](#apidoc.module.koa-validate.FileValidator)
1.  [function <span class="apidocSignatureSpan">koa-validate.</span>FileValidator (context, key, value, exists, params, deleteOnCheckFailed)](#apidoc.element.koa-validate.FileValidator.FileValidator)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.</span>super_ (context, key, value, exists, params , goOn)](#apidoc.element.koa-validate.FileValidator.super_)

#### [module koa-validate.FileValidator.prototype](#apidoc.module.koa-validate.FileValidator.prototype)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>contentTypeMatch (reg, tip)](#apidoc.element.koa-validate.FileValidator.prototype.contentTypeMatch)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>copy (dst, afterCopy)](#apidoc.element.koa-validate.FileValidator.prototype.copy)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>delete ()](#apidoc.element.koa-validate.FileValidator.prototype.delete)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>fileNameMatch (reg, tip)](#apidoc.element.koa-validate.FileValidator.prototype.fileNameMatch)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>isImageContentType (tip)](#apidoc.element.koa-validate.FileValidator.prototype.isImageContentType)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>move (dst, afterMove)](#apidoc.element.koa-validate.FileValidator.prototype.move)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>notEmpty (tip)](#apidoc.element.koa-validate.FileValidator.prototype.notEmpty)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>size (min, max, tip)](#apidoc.element.koa-validate.FileValidator.prototype.size)
1.  [function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>suffixIn (arr, tip)](#apidoc.element.koa-validate.FileValidator.prototype.suffixIn)

#### [module koa-validate.Validator](#apidoc.module.koa-validate.Validator)
1.  [function <span class="apidocSignatureSpan">koa-validate.</span>Validator (context, key, value, exists, params , goOn)](#apidoc.element.koa-validate.Validator.Validator)

#### [module koa-validate.Validator.prototype](#apidoc.module.koa-validate.Validator.prototype)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>addError (tip)](#apidoc.element.koa-validate.Validator.prototype.addError)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>blacklist (s)](#apidoc.element.koa-validate.Validator.prototype.blacklist)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>byteLength (min, max, charset, tip)](#apidoc.element.koa-validate.Validator.prototype.byteLength)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>check (fn , tip, scope)](#apidoc.element.koa-validate.Validator.prototype.check)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>clone (key , value)](#apidoc.element.koa-validate.Validator.prototype.clone)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>contains (s, tip)](#apidoc.element.koa-validate.Validator.prototype.contains)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>decodeBase64 (inBuffer , tip)](#apidoc.element.koa-validate.Validator.prototype.decodeBase64)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>decodeURI (tip)](#apidoc.element.koa-validate.Validator.prototype.decodeURI)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>decodeURIComponent (tip)](#apidoc.element.koa-validate.Validator.prototype.decodeURIComponent)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>default (d)](#apidoc.element.koa-validate.Validator.prototype.default)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>empty ()](#apidoc.element.koa-validate.Validator.prototype.empty)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>encodeBase64 ()](#apidoc.element.koa-validate.Validator.prototype.encodeBase64)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>encodeURI ()](#apidoc.element.koa-validate.Validator.prototype.encodeURI)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>encodeURIComponent ()](#apidoc.element.koa-validate.Validator.prototype.encodeURIComponent)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>ensure (assertion, tip, shouldBail)](#apidoc.element.koa-validate.Validator.prototype.ensure)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>ensureNot (assertion, tip, shouldBail)](#apidoc.element.koa-validate.Validator.prototype.ensureNot)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>eq (l, tip)](#apidoc.element.koa-validate.Validator.prototype.eq)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>escape ()](#apidoc.element.koa-validate.Validator.prototype.escape)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>exist (tip)](#apidoc.element.koa-validate.Validator.prototype.exist)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>filter (cb, scope)](#apidoc.element.koa-validate.Validator.prototype.filter)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>first (index)](#apidoc.element.koa-validate.Validator.prototype.first)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>ge (l, tip)](#apidoc.element.koa-validate.Validator.prototype.ge)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>get (index)](#apidoc.element.koa-validate.Validator.prototype.get)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>gt (l, tip)](#apidoc.element.koa-validate.Validator.prototype.gt)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>hasError ()](#apidoc.element.koa-validate.Validator.prototype.hasError)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>hash (alg , enc)](#apidoc.element.koa-validate.Validator.prototype.hash)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>in (arr, tip)](#apidoc.element.koa-validate.Validator.prototype.in)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isAfter (d, tip)](#apidoc.element.koa-validate.Validator.prototype.isAfter)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isAlpha (tip, locale)](#apidoc.element.koa-validate.Validator.prototype.isAlpha)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isAlphanumeric (tip, locale)](#apidoc.element.koa-validate.Validator.prototype.isAlphanumeric)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isAscii (tip)](#apidoc.element.koa-validate.Validator.prototype.isAscii)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isBase64 (tip)](#apidoc.element.koa-validate.Validator.prototype.isBase64)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isBefore (d, tip)](#apidoc.element.koa-validate.Validator.prototype.isBefore)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isByteLength (min, max, charset, tip)](#apidoc.element.koa-validate.Validator.prototype.isByteLength)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isCreditCard (tip)](#apidoc.element.koa-validate.Validator.prototype.isCreditCard)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isCurrency (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isCurrency)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isDataURI (tip)](#apidoc.element.koa-validate.Validator.prototype.isDataURI)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isDate (tip)](#apidoc.element.koa-validate.Validator.prototype.isDate)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isDivisibleBy (n, tip)](#apidoc.element.koa-validate.Validator.prototype.isDivisibleBy)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isEmail (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isEmail)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isFQDN (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isFQDN)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isFloat (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isFloat)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isFullWidth (tip)](#apidoc.element.koa-validate.Validator.prototype.isFullWidth)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isHalfWidth (tip)](#apidoc.element.koa-validate.Validator.prototype.isHalfWidth)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isHexColor (tip)](#apidoc.element.koa-validate.Validator.prototype.isHexColor)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isHexadecimal (tip)](#apidoc.element.koa-validate.Validator.prototype.isHexadecimal)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isISBN (tip, version)](#apidoc.element.koa-validate.Validator.prototype.isISBN)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isISIN (tip)](#apidoc.element.koa-validate.Validator.prototype.isISIN)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isISO8601 (tip)](#apidoc.element.koa-validate.Validator.prototype.isISO8601)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isIn (arr, tip)](#apidoc.element.koa-validate.Validator.prototype.isIn)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isInt (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isInt)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isIp (tip, version)](#apidoc.element.koa-validate.Validator.prototype.isIp)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isJSON (tip)](#apidoc.element.koa-validate.Validator.prototype.isJSON)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isLength (min, max, tip)](#apidoc.element.koa-validate.Validator.prototype.isLength)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isLowercase (tip)](#apidoc.element.koa-validate.Validator.prototype.isLowercase)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isMACAddress (tip)](#apidoc.element.koa-validate.Validator.prototype.isMACAddress)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isMobilePhone (tip, locale)](#apidoc.element.koa-validate.Validator.prototype.isMobilePhone)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isMultibyte (tip)](#apidoc.element.koa-validate.Validator.prototype.isMultibyte)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isNull (tip)](#apidoc.element.koa-validate.Validator.prototype.isNull)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isNumeric (tip)](#apidoc.element.koa-validate.Validator.prototype.isNumeric)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isSurrogatePair (tip)](#apidoc.element.koa-validate.Validator.prototype.isSurrogatePair)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isTime (tip)](#apidoc.element.koa-validate.Validator.prototype.isTime)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isUUID (tip, ver)](#apidoc.element.koa-validate.Validator.prototype.isUUID)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isUppercase (tip)](#apidoc.element.koa-validate.Validator.prototype.isUppercase)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isUrl (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isUrl)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isVariableWidth (tip)](#apidoc.element.koa-validate.Validator.prototype.isVariableWidth)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>le (l, tip)](#apidoc.element.koa-validate.Validator.prototype.le)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>len (min, max, tip)](#apidoc.element.koa-validate.Validator.prototype.len)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>lt (l, tip)](#apidoc.element.koa-validate.Validator.prototype.lt)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>ltrim (c)](#apidoc.element.koa-validate.Validator.prototype.ltrim)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>match (reg, tip)](#apidoc.element.koa-validate.Validator.prototype.match)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>md5 ()](#apidoc.element.koa-validate.Validator.prototype.md5)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>neq (l, tip)](#apidoc.element.koa-validate.Validator.prototype.neq)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>notBlank (tip)](#apidoc.element.koa-validate.Validator.prototype.notBlank)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>notContains (s, tip)](#apidoc.element.koa-validate.Validator.prototype.notContains)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>notEmpty (tip)](#apidoc.element.koa-validate.Validator.prototype.notEmpty)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>notMatch (reg, tip)](#apidoc.element.koa-validate.Validator.prototype.notMatch)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>optional ()](#apidoc.element.koa-validate.Validator.prototype.optional)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>replace (a, b)](#apidoc.element.koa-validate.Validator.prototype.replace)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>rtrim (c)](#apidoc.element.koa-validate.Validator.prototype.rtrim)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>sha1 ()](#apidoc.element.koa-validate.Validator.prototype.sha1)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>stripLow (nl)](#apidoc.element.koa-validate.Validator.prototype.stripLow)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toBoolean ()](#apidoc.element.koa-validate.Validator.prototype.toBoolean)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toDate ()](#apidoc.element.koa-validate.Validator.prototype.toDate)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toFloat (tip)](#apidoc.element.koa-validate.Validator.prototype.toFloat)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toInt (tip, radix, options)](#apidoc.element.koa-validate.Validator.prototype.toInt)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toJson (tip)](#apidoc.element.koa-validate.Validator.prototype.toJson)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toLow ()](#apidoc.element.koa-validate.Validator.prototype.toLow)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toLowercase ()](#apidoc.element.koa-validate.Validator.prototype.toLowercase)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toUp ()](#apidoc.element.koa-validate.Validator.prototype.toUp)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toUppercase ()](#apidoc.element.koa-validate.Validator.prototype.toUppercase)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>trim (c)](#apidoc.element.koa-validate.Validator.prototype.trim)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>type (t, tip)](#apidoc.element.koa-validate.Validator.prototype.type)
1.  [function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>whitelist (s)](#apidoc.element.koa-validate.Validator.prototype.whitelist)



# <a name="apidoc.module.koa-validate"></a>[module koa-validate](#apidoc.module.koa-validate)

#### <a name="apidoc.element.koa-validate.FileValidator"></a>[function <span class="apidocSignatureSpan">koa-validate.</span>FileValidator (context, key, value, exists, params, deleteOnCheckFailed)](#apidoc.element.koa-validate.FileValidator)
- description and source-code
```javascript
function FileValidator(context, key, value, exists, params, deleteOnCheckFailed){
	Validator.call(this,context, key, value, exists, params ,true);
	this.deleteOnCheckFailed = deleteOnCheckFailed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator"></a>[function <span class="apidocSignatureSpan">koa-validate.</span>Validator (context, key, value, exists, params , goOn)](#apidoc.element.koa-validate.Validator)
- description and source-code
```javascript
function Validator(context, key, value, exists, params , goOn) {
	this.params = params;
	this.context = context;
	this.key = key;
	this.value = value;
	this.exists = exists;
	this.goOn = (false===goOn?false:true);
	if(this.value && this instanceof FileValidator && 'goOn' in this.value ){
		this.goOn = this.value.goOn;
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-validate.FileValidator"></a>[module koa-validate.FileValidator](#apidoc.module.koa-validate.FileValidator)

#### <a name="apidoc.element.koa-validate.FileValidator.FileValidator"></a>[function <span class="apidocSignatureSpan">koa-validate.</span>FileValidator (context, key, value, exists, params, deleteOnCheckFailed)](#apidoc.element.koa-validate.FileValidator.FileValidator)
- description and source-code
```javascript
function FileValidator(context, key, value, exists, params, deleteOnCheckFailed){
	Validator.call(this,context, key, value, exists, params ,true);
	this.deleteOnCheckFailed = deleteOnCheckFailed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.FileValidator.super_"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.</span>super_ (context, key, value, exists, params , goOn)](#apidoc.element.koa-validate.FileValidator.super_)
- description and source-code
```javascript
function Validator(context, key, value, exists, params , goOn) {
	this.params = params;
	this.context = context;
	this.key = key;
	this.value = value;
	this.exists = exists;
	this.goOn = (false===goOn?false:true);
	if(this.value && this instanceof FileValidator && 'goOn' in this.value ){
		this.goOn = this.value.goOn;
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-validate.FileValidator.prototype"></a>[module koa-validate.FileValidator.prototype](#apidoc.module.koa-validate.FileValidator.prototype)

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.contentTypeMatch"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>contentTypeMatch (reg, tip)](#apidoc.element.koa-validate.FileValidator.prototype.contentTypeMatch)
- description and source-code
```javascript
contentTypeMatch = function (reg, tip){
	if (this.goOn && (!this.value || !reg.test(this.value.type))) {
		this.addError(tip || "file "+ (this.value && this.value.name||this.key) + " is bad format.");
		if(this.deleteOnCheckFailed){
			delFileAsync(this.value &&this.value.path);
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.copy"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>copy (dst, afterCopy)](#apidoc.element.koa-validate.FileValidator.prototype.copy)
- description and source-code
```javascript
function* (dst, afterCopy){
	if (this.goOn && this.value ) {
		var dstFile = dst;
		if('function' == typeof dst){
			if(isGeneratorFunction(dst)){
				dstFile = yield dst(this.value,this.key,this.context);
			}else{
				dstFile = dst(this.value,this.key,this.context);
			}
		}
		if(!(yield coFsExists(this.value.path))){
			this.addError('upload file not exists');
			return;
		}
		if(dstFile.length-1 == dstFile.lastIndexOf('/') ||dstFile.length-1 == dstFile.lastIndexOf('\\')||(yield coFsExists(dstFile)) && (
yield coFsIsDir(dstFile))){
			dstFile = path.join(dstFile , path.basename(this.value.path));
		}
		yield ensureDir(path.dirname(dstFile));
		yield coFsCopy(this.value.path,dstFile);
		this.value.newPath = dstFile;
		if('function' == typeof afterCopy){
			if(isGeneratorFunction(afterCopy)){
				yield afterCopy(this.value,this.key,this.context);
			}else{
				afterCopy(this.value,this.key,this.context);
			}
		}
	}
	return this;
}
```
- example usage
```shell
...
- **size(min,max,[tip])** - limit the file size.
- **contentTypeMatch(reg,[tip])** - check the file's contentType with regular expression.
- **isImageContentType([tip])** - check the file's contentType if is image content type.
- **fileNameMatch(reg,[tip])** - check the file's name with regular expression.
- **suffixIn(arr,[tip])** - check the suffix of file's if in specified arr. 'arr' eg. ['png','jpg']

#### Sanitizers:
File sanitizers are generators,we should use 'yield' to execute them. eg. 'yield this.checkFile('file').notEmpty().copy('/')';

- **move(target,[afterMove])** - move upload file to the target location. target can be a 'string' or 'function' or 'function*'.
if target end with '/' or '\\',the target will be deemed as directory.
target function interface:'string function(fileObject,fieldName,context)'.this function will return a string of the target file.
afterMove:it can be a 'function' or 'function*'.interface:'function(fileObject,fieldName,context)'
- **copy(target,[afterCopy])** - move upload file to the target location. target can be a 'string' or 'function' or 'function*'.
target function interface:'function (fileObject,fieldName,context)' .
afterCopy:it can be a 'function' or 'function*'.interface:'function(fileObject,fieldName,context)'
- **delete()** - delete upload file.
...
```

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.delete"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>delete ()](#apidoc.element.koa-validate.FileValidator.prototype.delete)
- description and source-code
```javascript
function* (){
	if (this.goOn && this.value ) {
		yield coFsDel(this.value.path);
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.fileNameMatch"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>fileNameMatch (reg, tip)](#apidoc.element.koa-validate.FileValidator.prototype.fileNameMatch)
- description and source-code
```javascript
fileNameMatch = function (reg, tip){
	if (this.goOn && (!this.value || !reg.test(this.value.name))) {
		this.addError(tip || "file "+ (this.value && this.value.name||this.key) + " is bad file type.");
		if(this.deleteOnCheckFailed){
			delFileAsync(this.value&&this.value.path);
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.isImageContentType"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>isImageContentType (tip)](#apidoc.element.koa-validate.FileValidator.prototype.isImageContentType)
- description and source-code
```javascript
isImageContentType = function (tip){
	if (this.goOn && (!this.value || 0!==this.value.type.indexOf('image/'))) {
		this.addError(tip || "file "+ (this.value && this.value.name||this.key) + " is not a image format.");
		if(this.deleteOnCheckFailed){
			delFileAsync(this.value &&this.value.path);
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.move"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>move (dst, afterMove)](#apidoc.element.koa-validate.FileValidator.prototype.move)
- description and source-code
```javascript
function* (dst, afterMove){
	if (this.goOn && this.value ) {
		yield this.copy(dst);
		yield coFsDel(this.value.path);
		if('function' == typeof afterMove){
			if(isGeneratorFunction(afterMove)){
				yield afterMove(this.value,this.key,this.context);
			}else{
				afterMove(this.value,this.key,this.context);
			}
		}
	}
	return this;
}
```
- example usage
```shell
...
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
		//resize image
	});
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
...
```

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.notEmpty"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>notEmpty (tip)](#apidoc.element.koa-validate.FileValidator.prototype.notEmpty)
- description and source-code
```javascript
notEmpty = function (tip){
	if (this.goOn && (!this.value||this.value.size<=0)) {
		this.addError(tip || "file "+ this.key + " can not be a empty file.");
		if(this.deleteOnCheckFailed){
			delFileAsync(this.value&&this.value.path);
		}
	}
	return this;
}
```
- example usage
```shell
...

app.use(require('koa-body')({multipart:true , formidable:{keepExtensions:true}}));
app.use(router.routes()).use(router.allowedMethods());
router.post('/signup', function * () {
	//optional() means this param may not in the params.
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
		//resize image
	});
...
```

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.size"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>size (min, max, tip)](#apidoc.element.koa-validate.FileValidator.prototype.size)
- description and source-code
```javascript
size = function (min, max, tip){
	if (this.goOn && (!this.value||this.value.size<min || this.value.size>max)) {
		this.addError(tip || "file "+(this.value && this.value.name||this.key) + "' length must between "+formatSize(min)+" and "+formatSize
(max)+".");
		if(this.deleteOnCheckFailed){
			delFileAsync(this.value &&this.value.path);
		}
	}
	return this;
}
```
- example usage
```shell
...
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
		//resize image
	});
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
...
```

#### <a name="apidoc.element.koa-validate.FileValidator.prototype.suffixIn"></a>[function <span class="apidocSignatureSpan">koa-validate.FileValidator.prototype.</span>suffixIn (arr, tip)](#apidoc.element.koa-validate.FileValidator.prototype.suffixIn)
- description and source-code
```javascript
suffixIn = function (arr, tip){
	if (this.goOn && (!this.value || -1==arr.indexOf(-1==this.value.name.lastIndexOf('.')?"":this.value.name.substring(this.value.name
.lastIndexOf('.')+1)))) {
		this.addError(tip || "file "+ (this.value && this.value.name||this.key) + " is bad file type.");
		if(this.deleteOnCheckFailed){
			delFileAsync(this.value &&this.value.path);
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-validate.Validator"></a>[module koa-validate.Validator](#apidoc.module.koa-validate.Validator)

#### <a name="apidoc.element.koa-validate.Validator.Validator"></a>[function <span class="apidocSignatureSpan">koa-validate.</span>Validator (context, key, value, exists, params , goOn)](#apidoc.element.koa-validate.Validator.Validator)
- description and source-code
```javascript
function Validator(context, key, value, exists, params , goOn) {
	this.params = params;
	this.context = context;
	this.key = key;
	this.value = value;
	this.exists = exists;
	this.goOn = (false===goOn?false:true);
	if(this.value && this instanceof FileValidator && 'goOn' in this.value ){
		this.goOn = this.value.goOn;
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.koa-validate.Validator.prototype"></a>[module koa-validate.Validator.prototype](#apidoc.module.koa-validate.Validator.prototype)

#### <a name="apidoc.element.koa-validate.Validator.prototype.addError"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>addError (tip)](#apidoc.element.koa-validate.Validator.prototype.addError)
- description and source-code
```javascript
addError = function (tip) {
	this.goOn = false;
	if(this.value && this instanceof FileValidator ){
		this.value.goOn = false;
	}
	if (!this.context.errors) {
		this.context.errors = [];
	}
	var e = {};
	e[this.key] = tip;
	this.context.errors.push(e);
}
```
- example usage
```shell
...
	if (!this.exists) {
		this.goOn = false;
	}
	return this;
};
Validator.prototype.notEmpty = function(tip) {
	if (this.goOn && (null==this.value||'undefined'==typeof(this.value) || ('string' == typeof(this.value) &&!this.value))) {
		this.addError(tip || this.key + " can not be empty.");
	}
	return this;
};
Validator.prototype.empty = function() {
	if (this.goOn) {
		if (!this.value) {
			this.goOn = false;
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.blacklist"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>blacklist (s)](#apidoc.element.koa-validate.Validator.prototype.blacklist)
- description and source-code
```javascript
blacklist = function (s) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.blacklist(this.value,s);
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.whitelist(this.value,s);
	}
	return this;
};
Validator.prototype.blacklist = function(s) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.blacklist(this.value,s);
	}
	return this;
};
Validator.prototype.encodeURI = function() {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = encodeURI(this.value);
	}
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.byteLength"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>byteLength (min, max, charset, tip)](#apidoc.element.koa-validate.Validator.prototype.byteLength)
- description and source-code
```javascript
byteLength = function (min, max, charset, tip) {
	min = min || 0;
	max = max || Number.MAX_VALUE;
	charset = charset||'utf8';
	this.notEmpty(tip);
	if (this.goOn) {
		var bl = Buffer.byteLength(this.value , charset);
		tip = 'number' != typeof max ? max : tip;
		if (bl<min || bl>max) {
			this.addError(tip || this.key + "'s byte lenth great than " + min +" and less than " + max + "." );
		}
	}
	return this;
}
```
- example usage
```shell
...
};
Validator.prototype.isByteLength = function(min, max,charset,tip) {
	min = min || 0;
	max = max || Number.MAX_VALUE;
	charset = charset||'utf8';
	this.notEmpty(tip);
	if (this.goOn) {
		var bl = Buffer.byteLength(this.value , charset);
		tip = 'number' != typeof max ? max : tip;
		if (bl<min || bl>max) {
			this.addError(tip || this.key + "'s byte lenth great than " + min +" and less than " + max + "." );
		}
	}
	return this;
};
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.check"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>check (fn , tip, scope)](#apidoc.element.koa-validate.Validator.prototype.check)
- description and source-code
```javascript
check = function (fn , tip, scope) {
	if(this.goOn && !this.hasError()&&!fn.call(scope||this,this.value,this.key,this.context)) {
		this.addError(tip||this.key+" check failed.")
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.clone"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>clone (key , value)](#apidoc.element.koa-validate.Validator.prototype.clone)
- description and source-code
```javascript
clone = function (key , value) {
	if (!this.hasError()&&this.value) {
		this.value = this.params[key] = ('undefined' == typeof value?this.value:value);
		this.key = key;
	}
	return this;
}
```
- example usage
```shell
...
- **whitelist(value)** - remove characters that do not appear in the whitelist.
- **blacklist(value)** - remove characters that appear in the blacklist.
- **encodeURI()** - ref mdn [encodeURI](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/encodeURI
)
- **decodeURI([tip])** - ref mdn [decodeURI](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/decodeURI
)
- **encodeURIComponent()** - ref mdn [encodeURIComponent](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects
/encodeURIComponent)
- **decodeURIComponent([tip])** - ref mdn [decodeURIComponent](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference
/Global_Objects/decodeURIComponent)
- **replace(regexp|substr, newSubStr|function)** - the same as [String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/
Reference/Global_Objects/String/replace) replace
- **clone(newKey,[newValue])** - clone current value to the new key, if newValue supplied , use it. eg. 'this.checkBody('v1').clone
('md5').md5()'; then your can use 'this.request.body.md5'.
- **encodeBase64()** - encode current value to base64 string.
- **decodeBase64([inBuffer],[tip])** - decode current base64 to a normal string,if inBuffer is true , the value will be a Buffer
.
- **hash(alg , [encoding])** - hash current value use specified algorithm and encoding(if supplied , default is 'hex'). ref [hash
](http://nodejs.org/api/crypto.html#crypto_class_hash)
- **md5()** - md5 current value into hex string.
- **sha1()** - sha1 current value into hex string.

### For json path:
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.contains"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>contains (s, tip)](#apidoc.element.koa-validate.Validator.prototype.contains)
- description and source-code
```javascript
contains = function (s, tip) {
	if (this.goOn && (!isString(this.value) ||!v.contains(this.value,s))) {
		this.addError(tip || this.key + " is must contain " + s + ".");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.le = function(l, tip) {
	if (this.goOn && this.value > l) {
		this.addError(tip || this.key + " must less than or equal " + l + ".");
	}
	return this;
};
Validator.prototype.contains = function(s, tip) {
	if (this.goOn && (!isString(this.value) ||!v.contains(this.value,s))) {
		this.addError(tip || this.key + " is must contain " + s + ".");
	}
	return this;
};
Validator.prototype.notContains = function(s, tip) {
	if (this.goOn && (!isString(this.value) ||v.contains(this.value,s))) {
		this.addError(tip || this.key + " is must not contain " + s + ".");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.decodeBase64"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>decodeBase64 (inBuffer , tip)](#apidoc.element.koa-validate.Validator.prototype.decodeBase64)
- description and source-code
```javascript
decodeBase64 = function (inBuffer , tip) {
	if (!this.hasError()&&this.value) {
		try{
			if(inBuffer){
				this.value = this.params[this.key] = new Buffer(this.value , 'base64');
			}else{
				this.value = this.params[this.key] = new Buffer(this.value , 'base64').toString();
			}
		}catch(e){
			this.addError(tip||"bad base64 format value");
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.decodeURI"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>decodeURI (tip)](#apidoc.element.koa-validate.Validator.prototype.decodeURI)
- description and source-code
```javascript
decodeURI = function (tip) {
	if (this.goOn && !this.hasError()&&this.value) {
		try{
			this.value = this.params[this.key] = decodeURI(this.value);
		}catch(e){
			this.addError(tip||'bad uri to decode.');
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.decodeURIComponent"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>decodeURIComponent (tip)](#apidoc.element.koa-validate.Validator.prototype.decodeURIComponent)
- description and source-code
```javascript
decodeURIComponent = function (tip) {
	if (this.goOn && !this.hasError()&&this.value) {
		try{
			this.value = this.params[this.key] = decodeURIComponent(this.value);
		}catch(e){
			this.addError(tip||'bad uri to decode.');
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.default"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>default (d)](#apidoc.element.koa-validate.Validator.prototype.default)
- description and source-code
```javascript
default = function (d) {
	if(!this.hasError()&&!this.value){
		this.value = this.params[this.key] = d;
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.empty"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>empty ()](#apidoc.element.koa-validate.Validator.prototype.empty)
- description and source-code
```javascript
empty = function () {
	if (this.goOn) {
		if (!this.value) {
			this.goOn = false;
		}
	}
	return this;
}
```
- example usage
```shell
...
app.use(router.routes()).use(router.allowedMethods());
router.post('/signup', function * () {
	//optional() means this param may not in the params.
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
		//resize image
	});
	if (this.errors) {
		this.body = this.errors;
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.encodeBase64"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>encodeBase64 ()](#apidoc.element.koa-validate.Validator.prototype.encodeBase64)
- description and source-code
```javascript
encodeBase64 = function () {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = new Buffer(this.value).toString('base64');
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.encodeURI"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>encodeURI ()](#apidoc.element.koa-validate.Validator.prototype.encodeURI)
- description and source-code
```javascript
encodeURI = function () {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = encodeURI(this.value);
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.encodeURIComponent"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>encodeURIComponent ()](#apidoc.element.koa-validate.Validator.prototype.encodeURIComponent)
- description and source-code
```javascript
encodeURIComponent = function () {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = encodeURIComponent(this.value);
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.ensure"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>ensure (assertion, tip, shouldBail)](#apidoc.element.koa-validate.Validator.prototype.ensure)
- description and source-code
```javascript
ensure = function (assertion, tip, shouldBail) {
  if (shouldBail) this.goOn = false;
    if (this.goOn && !assertion) {
        this.addError(tip || this.key + ' failed an assertion.');
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.ensureNot"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>ensureNot (assertion, tip, shouldBail)](#apidoc.element.koa-validate.Validator.prototype.ensureNot)
- description and source-code
```javascript
ensureNot = function (assertion, tip, shouldBail) {
  if (shouldBail) this.goOn = false;
    if (this.goOn && !!assertion) {
        this.addError(tip || this.key + ' failed an assertion.');
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.eq"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>eq (l, tip)](#apidoc.element.koa-validate.Validator.prototype.eq)
- description and source-code
```javascript
eq = function (l, tip) {
	if (this.goOn && this.value != l) {
		this.addError(tip || this.key + " is must equal " + l + ".");
	}
	return this;
}
```
- example usage
```shell
...
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
//json body,we can check it using [json path](https://github.com/flitbit/json-path)(like xpath)
router.post('/json' , function*(){
	this.checkBody('/store/book[0]/price').get(0).eq(8.95);
	this.checkBody('#/store/book[0]/category').first().trim().eq('reference');
	if (this.errors) {
		this.body = this.errors;
		return;
	}
})
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.escape"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>escape ()](#apidoc.element.koa-validate.Validator.prototype.escape)
- description and source-code
```javascript
escape = function () {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.escape(this.value);
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.rtrim(this.value,c);
	}
	return this;
};
Validator.prototype.escape = function() {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.escape(this.value);
	}
	return this;
};
Validator.prototype.stripLow = function(nl) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.stripLow(this.value, nl);
	}
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.exist"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>exist (tip)](#apidoc.element.koa-validate.Validator.prototype.exist)
- description and source-code
```javascript
exist = function (tip) {
	if (this.goOn && !this.exists) {
		 this.addError(tip || this.key +" should exists!");
	}
	return this;
}
```
- example usage
```shell
...
	return this;
};

Validator.prototype.isLength = function(min, max, tip) {
	min = min || 0;
	tip = 'number' != typeof max ? max : tip;
	max = 'number' == typeof max ? max :-1;
	this.exist(tip);
	if (this.goOn) {
		if(this.value.length<min) {
			this.addError(tip || this.key + "'s length must equal or great than " + min+".");
			return this;
		}
		if (-1!=max&&this.value.length>max) {
			this.addError(tip || this.key + "'s length must equal or less than " + max + ".");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.filter"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>filter (cb, scope)](#apidoc.element.koa-validate.Validator.prototype.filter)
- description and source-code
```javascript
filter = function (cb, scope) {
	if (this.value&&this.value.length>0) {
		var vs = []
		for(var i = 0 ;i<this.value.length;i++) {
			if(cb.call(scope||this,this.value[i],i,this.key,this.context)){
				vs.push(this.value[i])
			}
		}
		this.value=vs;
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.first"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>first (index)](#apidoc.element.koa-validate.Validator.prototype.first)
- description and source-code
```javascript
first = function (index) {
	return this.get(0);
}
```
- example usage
```shell
...
		this.body = this.errors;
		return;
	}
});
//json body,we can check it using [json path](https://github.com/flitbit/json-path)(like xpath)
router.post('/json' , function*(){
	this.checkBody('/store/book[0]/price').get(0).eq(8.95);
	this.checkBody('#/store/book[0]/category').first().trim().eq('reference');
	if (this.errors) {
		this.body = this.errors;
		return;
	}
})

app.listen(3000);
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.ge"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>ge (l, tip)](#apidoc.element.koa-validate.Validator.prototype.ge)
- description and source-code
```javascript
ge = function (l, tip) {
	if (this.goOn && this.value < l) {
		this.addError(tip || this.key + " must great than or equal " + l + ".");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.get"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>get (index)](#apidoc.element.koa-validate.Validator.prototype.get)
- description and source-code
```javascript
get = function (index) {
	if (this.value) {
		this.value = this.value[index||0]
	}
	return this;
}
```
- example usage
```shell
...
		//resize image
	});
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
router.get('/users', function * () {
	this.checkQuery('department').empty().in(["sale","finance"], "not support this department!").len(3, 20);	
	this.checkQuery('name').empty().len(2,20,"bad name.").trim().toLow();
	this.checkQuery('age').empty().gt(10,"too young!").lt(30,"to old!").toInt();
	if (this.errors) {
		this.body = this.errors;
		return;
	}
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.gt"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>gt (l, tip)](#apidoc.element.koa-validate.Validator.prototype.gt)
- description and source-code
```javascript
gt = function (l, tip) {
	if (this.goOn && this.value <= l) {
		this.addError(tip || this.key + " must great than " + l + ".");
	}
	return this;
}
```
- example usage
```shell
...
		this.body = this.errors;
		return;
	}
});
router.get('/users', function * () {
	this.checkQuery('department').empty().in(["sale","finance"], "not support this department!").len(3, 20);	
	this.checkQuery('name').empty().len(2,20,"bad name.").trim().toLow();
	this.checkQuery('age').empty().gt(10,"too young!").lt(30,"to old!").toInt();
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
router.get('/user/:id', function * () {
	this.checkParams('id').toInt(0);
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.hasError"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>hasError ()](#apidoc.element.koa-validate.Validator.prototype.hasError)
- description and source-code
```javascript
hasError = function () {
	return this.context.errors && this.context.errors.length > 0 ? true : false;
}
```
- example usage
```shell
...
	}
	return this;
};


//Sanitizers
Validator.prototype.default = function(d) {
	if(!this.hasError()&&!this.value){
		this.value = this.params[this.key] = d;
	}
	return this;
};
Validator.prototype.toDate = function() {
	this.isDate();
	if (this.goOn && !this.hasError()) {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.hash"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>hash (alg , enc)](#apidoc.element.koa-validate.Validator.prototype.hash)
- description and source-code
```javascript
hash = function (alg , enc) {
	if (!this.hasError()&&this.value) {
		enc = enc ||'hex';
		this.value = this.params[this.key] =require('crypto').createHash(alg).update(this.value).digest(enc);
	}
	return this;
}
```
- example usage
```shell
...
	if (!this.hasError()&&this.value) {
		enc = enc ||'hex';
		this.value = this.params[this.key] =require('crypto').createHash(alg).update(this.value).digest(enc);
	}
	return this;
};
Validator.prototype.md5 = function() {
	this.hash('md5');
	return this;
};
Validator.prototype.sha1 = function() {
	this.hash('sha1');
	return this;
};
Validator.prototype.clone = function(key , value) {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.in"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>in (arr, tip)](#apidoc.element.koa-validate.Validator.prototype.in)
- description and source-code
```javascript
in = function (arr, tip) {
	if (this.goOn && arr) {
		for(var i = 0 ; i < arr.length ;i++){
			if(this.value == arr[i]){
				return this;
			}
		}
		this.addError(tip || this.key + " must be in [" + arr.join(',') + "].");
	}
	return this;
}
```
- example usage
```shell
...
	});
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
router.get('/users', function * () {
	this.checkQuery('department').empty().in(["sale","finance"], "not support this department!").len(3, 20);	
	this.checkQuery('name').empty().len(2,20,"bad name.").trim().toLow();
	this.checkQuery('age').empty().gt(10,"too young!").lt(30,"to old!").toInt();
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isAfter"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isAfter (d, tip)](#apidoc.element.koa-validate.Validator.prototype.isAfter)
- description and source-code
```javascript
isAfter = function (d, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isAfter(this.value, d))) {
		this.addError(tip || this.key + " must after " + d + ".");
	}
	return this;
}
```
- example usage
```shell
...
	if(this.goOn && ! timeReg.test(this.value)){
		this.addError(tip || this.key + " is not a time format.");
	}
	return this;
};

Validator.prototype.isAfter = function(d, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isAfter(this.value, d))) {
		this.addError(tip || this.key + " must after " + d + ".");
	}
	return this;
};
Validator.prototype.isBefore = function(d, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isBefore(this.value, d))) {
		this.addError(tip || this.key + " must before " + d + ".");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isAlpha"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isAlpha (tip, locale)](#apidoc.element.koa-validate.Validator.prototype.isAlpha)
- description and source-code
```javascript
isAlpha = function (tip, locale) {
	if (this.goOn && (!isString(this.value) ||!v.isAlpha(this.value,locale))) {
		this.addError(tip || this.key + " is not an alpha string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isIp = function(tip,version) {
	if (this.goOn && (!isString(this.value) ||!v.isIP(this.value,version))) {
		this.addError(tip || this.key + " is not ip format.");
	}
	return this;
};
Validator.prototype.isAlpha = function(tip,locale) {
	if (this.goOn && (!isString(this.value) ||!v.isAlpha(this.value,locale))) {
		this.addError(tip || this.key + " is not an alpha string.");
	}
	return this;
};
Validator.prototype.isNumeric = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isNumeric(this.value))) {
		this.addError(tip || this.key + " is  not numeric.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isAlphanumeric"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isAlphanumeric (tip, locale)](#apidoc.element.koa-validate.Validator.prototype.isAlphanumeric)
- description and source-code
```javascript
isAlphanumeric = function (tip, locale) {
	if (this.goOn && (!isString(this.value) ||!v.isAlphanumeric(this.value,locale))) {
		this.addError(tip || this.key + " is not an aphanumeric string.");
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && (!isString(this.value) ||!v.isNumeric(this.value))) {
		this.addError(tip || this.key + " is  not numeric.");
	}
	return this;
};

Validator.prototype.isAlphanumeric = function(tip,locale) {
	if (this.goOn && (!isString(this.value) ||!v.isAlphanumeric(this.value,locale))) {
		this.addError(tip || this.key + " is not an aphanumeric string.");
	}
	return this;
};
Validator.prototype.isBase64 = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isBase64(this.value))) {
		this.addError(tip || this.key + " is not a base64 string.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isAscii"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isAscii (tip)](#apidoc.element.koa-validate.Validator.prototype.isAscii)
- description and source-code
```javascript
isAscii = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isAscii(this.value))) {
		this.addError(tip || this.key + " is not a ascii string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isMultibyte = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isMultibyte(this.value))) {
		this.addError(tip || this.key + " is not a multibyte string.");
	}
	return this;
};
Validator.prototype.isAscii = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isAscii(this.value))) {
		this.addError(tip || this.key + " is not a ascii string.");
	}
	return this;
};
Validator.prototype.isFullWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isFullWidth(this.value))) {
		this.addError(tip || this.key + " is not a full width string.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isBase64"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isBase64 (tip)](#apidoc.element.koa-validate.Validator.prototype.isBase64)
- description and source-code
```javascript
isBase64 = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isBase64(this.value))) {
		this.addError(tip || this.key + " is not a base64 string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isAlphanumeric = function(tip,locale) {
	if (this.goOn && (!isString(this.value) ||!v.isAlphanumeric(this.value,locale))) {
		this.addError(tip || this.key + " is not an aphanumeric string.");
	}
	return this;
};
Validator.prototype.isBase64 = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isBase64(this.value))) {
		this.addError(tip || this.key + " is not a base64 string.");
	}
	return this;
};
Validator.prototype.isHexadecimal = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHexadecimal(this.value))) {
		this.addError(tip || this.key + " is not a hexa decimal string.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isBefore"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isBefore (d, tip)](#apidoc.element.koa-validate.Validator.prototype.isBefore)
- description and source-code
```javascript
isBefore = function (d, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isBefore(this.value, d))) {
		this.addError(tip || this.key + " must before " + d + ".");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isAfter = function(d, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isAfter(this.value, d))) {
		this.addError(tip || this.key + " must after " + d + ".");
	}
	return this;
};
Validator.prototype.isBefore = function(d, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isBefore(this.value, d))) {
		this.addError(tip || this.key + " must before " + d + ".");
	}
	return this;
};
Validator.prototype.isCreditCard = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isCreditCard(this.value))) {
		this.addError(tip || this.key + " is not credit card format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isByteLength"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isByteLength (min, max, charset, tip)](#apidoc.element.koa-validate.Validator.prototype.isByteLength)
- description and source-code
```javascript
isByteLength = function (min, max, charset, tip) {
	min = min || 0;
	max = max || Number.MAX_VALUE;
	charset = charset||'utf8';
	this.notEmpty(tip);
	if (this.goOn) {
		var bl = Buffer.byteLength(this.value , charset);
		tip = 'number' != typeof max ? max : tip;
		if (bl<min || bl>max) {
			this.addError(tip || this.key + "'s byte lenth great than " + min +" and less than " + max + "." );
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isCreditCard"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isCreditCard (tip)](#apidoc.element.koa-validate.Validator.prototype.isCreditCard)
- description and source-code
```javascript
isCreditCard = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isCreditCard(this.value))) {
		this.addError(tip || this.key + " is not credit card format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isBefore = function(d, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isBefore(this.value, d))) {
		this.addError(tip || this.key + " must before " + d + ".");
	}
	return this;
};
Validator.prototype.isCreditCard = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isCreditCard(this.value))) {
		this.addError(tip || this.key + " is not credit card format.");
	}
	return this;
};
Validator.prototype.isISBN = function(tip,version) {
	if (this.goOn && (!isString(this.value) ||!v.isISBN(this.value,version))) {
		this.addError(tip || this.key + " is not a ISBN format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isCurrency"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isCurrency (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isCurrency)
- description and source-code
```javascript
isCurrency = function (tip, options) {
	if (this.goOn && (!isString(this.value) ||!v.isCurrency(this.value,options))) {
		this.addError(tip || this.key + " is not a currency format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isSurrogatePair = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isSurrogatePair(this.value))) {
		this.addError(tip || this.key + " is not a surrogate pair string.");
	}
	return this;
};
Validator.prototype.isCurrency = function(tip,options) {
	if (this.goOn && (!isString(this.value) ||!v.isCurrency(this.value,options))) {
		this.addError(tip || this.key + " is not a currency format.");
	}
	return this;
};
Validator.prototype.isDataURI = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isDataURI(this.value))) {
		this.addError(tip || this.key + " is not a data uri format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isDataURI"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isDataURI (tip)](#apidoc.element.koa-validate.Validator.prototype.isDataURI)
- description and source-code
```javascript
isDataURI = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isDataURI(this.value))) {
		this.addError(tip || this.key + " is not a data uri format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isCurrency = function(tip,options) {
	if (this.goOn && (!isString(this.value) ||!v.isCurrency(this.value,options))) {
		this.addError(tip || this.key + " is not a currency format.");
	}
	return this;
};
Validator.prototype.isDataURI = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isDataURI(this.value))) {
		this.addError(tip || this.key + " is not a data uri format.");
	}
	return this;
};
Validator.prototype.isMobilePhone = function(tip,locale) {
	if (this.goOn && (!isString(this.value) ||!v.isMobilePhone(this.value,locale))) {
		this.addError(tip || this.key + " is not a mobile phone format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isDate"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isDate (tip)](#apidoc.element.koa-validate.Validator.prototype.isDate)
- description and source-code
```javascript
isDate = function (tip) {
	if (this.goOn && !util.isDate(this.value)  && (!isString(this.value) ||!v.isDate(this.value))) {
		this.addError(tip || this.key + " is not a date format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isUUID = function(tip,ver) {
	if (this.goOn && (!isString(this.value) ||!v.isUUID(this.value,ver))) {
		this.addError(tip || this.key + " is not a UUID format.");
	}
	return this;
};
Validator.prototype.isDate = function(tip) {
	if (this.goOn && !util.isDate(this.value)  && (!isString(this.value) ||!v.isDate(this.value))) {
		this.addError(tip || this.key + " is not a date format.");
	}
	return this;
};
Validator.prototype.isTime = function(tip) {
	var timeReg = /^(([0-1]?[0-9])|([2][0-3])):([0-5]?[0-9])(:([0-5]?[0-9]))?$/;
	if(this.goOn && ! timeReg.test(this.value)){
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isDivisibleBy"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isDivisibleBy (n, tip)](#apidoc.element.koa-validate.Validator.prototype.isDivisibleBy)
- description and source-code
```javascript
isDivisibleBy = function (n, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isDivisibleBy(this.value, n))) {
		this.addError(tip || this.key + " can not divide by" + n + ".");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isUppercase = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isUppercase(this.value))) {
		this.addError(tip || this.key + " is not a upper case string.");
	}
	return this;
};
Validator.prototype.isDivisibleBy = function(n, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isDivisibleBy(this.value, n))) {
		this.addError(tip || this.key + " can not divide by" + n + ".");
	}
	return this;
};
Validator.prototype.isNull = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isNull(this.value))) {
		this.addError(tip || this.key + " is not null.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isEmail"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isEmail (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isEmail)
- description and source-code
```javascript
isEmail = function (tip, options) {
	if (this.goOn && (!isString(this.value) ||!v.isEmail(this.value,options))) {
		this.addError(tip || this.key + " is not email format.");
	}
	return this;
}
```
- example usage
```shell
...
require('koa-validate')(app);

app.use(require('koa-body')({multipart:true , formidable:{keepExtensions:true}}));
app.use(router.routes()).use(router.allowedMethods());
router.post('/signup', function * () {
	//optional() means this param may not in the params.
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
		//resize image
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isFQDN"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isFQDN (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isFQDN)
- description and source-code
```javascript
isFQDN = function (tip, options) {
	if (this.goOn && (!isString(this.value) ||!v.isFQDN(this.value,options))) {
		this.addError(tip || this.key + " is not a fully qualified domain name format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isISIN = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isISIN(this.value))) {
		this.addError(tip || this.key + " is not a ISIN format.");
	}
	return this;
};
Validator.prototype.isFQDN = function(tip,options) {
	if (this.goOn && (!isString(this.value) ||!v.isFQDN(this.value,options))) {
		this.addError(tip || this.key + " is not a fully qualified domain name format.");
	}
	return this;
};


//Sanitizers
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isFloat"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isFloat (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isFloat)
- description and source-code
```javascript
isFloat = function (tip, options) {
	if (this.goOn && !v.isFloat(String(this.value), options)) {
		this.addError(tip || this.key + " is not float.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isInt = function(tip, options) {
	if (this.goOn&& !v.isInt(String(this.value), options)) {
		this.addError(tip || this.key + " is not integer.");
	}
	return this;
};
Validator.prototype.isFloat = function(tip,options) {
	if (this.goOn && !v.isFloat(String(this.value), options)) {
		this.addError(tip || this.key + " is not float.");
	}
	return this;
};

Validator.prototype.isLength = function(min, max, tip) {
	min = min || 0;
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isFullWidth"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isFullWidth (tip)](#apidoc.element.koa-validate.Validator.prototype.isFullWidth)
- description and source-code
```javascript
isFullWidth = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isFullWidth(this.value))) {
		this.addError(tip || this.key + " is not a full width string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isAscii = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isAscii(this.value))) {
		this.addError(tip || this.key + " is not a ascii string.");
	}
	return this;
};
Validator.prototype.isFullWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isFullWidth(this.value))) {
		this.addError(tip || this.key + " is not a full width string.");
	}
	return this;
};
Validator.prototype.isHalfWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHalfWidth(this.value))) {
		this.addError(tip || this.key + " is not a half width string.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isHalfWidth"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isHalfWidth (tip)](#apidoc.element.koa-validate.Validator.prototype.isHalfWidth)
- description and source-code
```javascript
isHalfWidth = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHalfWidth(this.value))) {
		this.addError(tip || this.key + " is not a half width string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isFullWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isFullWidth(this.value))) {
		this.addError(tip || this.key + " is not a full width string.");
	}
	return this;
};
Validator.prototype.isHalfWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHalfWidth(this.value))) {
		this.addError(tip || this.key + " is not a half width string.");
	}
	return this;
};
Validator.prototype.isVariableWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isVariableWidth(this.value))) {
		this.addError(tip || this.key + " is not a variable width string.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isHexColor"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isHexColor (tip)](#apidoc.element.koa-validate.Validator.prototype.isHexColor)
- description and source-code
```javascript
isHexColor = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHexColor(this.value))) {
		this.addError(tip || this.key + " is  not hex color format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isHexadecimal = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHexadecimal(this.value))) {
		this.addError(tip || this.key + " is not a hexa decimal string.");
	}
	return this;
};
Validator.prototype.isHexColor = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHexColor(this.value))) {
		this.addError(tip || this.key + " is  not hex color format.");
	}
	return this;
};
Validator.prototype.isLowercase = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isLowercase(this.value))) {
		this.addError(tip || this.key + " is not a lowwer case string");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isHexadecimal"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isHexadecimal (tip)](#apidoc.element.koa-validate.Validator.prototype.isHexadecimal)
- description and source-code
```javascript
isHexadecimal = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHexadecimal(this.value))) {
		this.addError(tip || this.key + " is not a hexa decimal string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isBase64 = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isBase64(this.value))) {
		this.addError(tip || this.key + " is not a base64 string.");
	}
	return this;
};
Validator.prototype.isHexadecimal = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHexadecimal(this.value))) {
		this.addError(tip || this.key + " is not a hexa decimal string.");
	}
	return this;
};
Validator.prototype.isHexColor = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHexColor(this.value))) {
		this.addError(tip || this.key + " is  not hex color format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isISBN"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isISBN (tip, version)](#apidoc.element.koa-validate.Validator.prototype.isISBN)
- description and source-code
```javascript
isISBN = function (tip, version) {
	if (this.goOn && (!isString(this.value) ||!v.isISBN(this.value,version))) {
		this.addError(tip || this.key + " is not a ISBN format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isCreditCard = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isCreditCard(this.value))) {
		this.addError(tip || this.key + " is not credit card format.");
	}
	return this;
};
Validator.prototype.isISBN = function(tip,version) {
	if (this.goOn && (!isString(this.value) ||!v.isISBN(this.value,version))) {
		this.addError(tip || this.key + " is not a ISBN format.");
	}
	return this;
};
Validator.prototype.isJSON = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isJSON(this.value))) {
		this.addError(tip || this.key + " is not a json format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isISIN"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isISIN (tip)](#apidoc.element.koa-validate.Validator.prototype.isISIN)
- description and source-code
```javascript
isISIN = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isISIN(this.value))) {
		this.addError(tip || this.key + " is not a ISIN format.");
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && (!isString(this.value) ||!v.isMACAddress(this.value))) {
		this.addError(tip || this.key + " is not a MAC address format.");
	}
	return this;
};

Validator.prototype.isISIN = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isISIN(this.value))) {
		this.addError(tip || this.key + " is not a ISIN format.");
	}
	return this;
};
Validator.prototype.isFQDN = function(tip,options) {
	if (this.goOn && (!isString(this.value) ||!v.isFQDN(this.value,options))) {
		this.addError(tip || this.key + " is not a fully qualified domain name format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isISO8601"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isISO8601 (tip)](#apidoc.element.koa-validate.Validator.prototype.isISO8601)
- description and source-code
```javascript
isISO8601 = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isISO8601(this.value))) {
		this.addError(tip || this.key + " is not a ISO8601 string format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isMobilePhone = function(tip,locale) {
	if (this.goOn && (!isString(this.value) ||!v.isMobilePhone(this.value,locale))) {
		this.addError(tip || this.key + " is not a mobile phone format.");
	}
	return this;
};
Validator.prototype.isISO8601 = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isISO8601(this.value))) {
		this.addError(tip || this.key + " is not a ISO8601 string format.");
	}
	return this;
};
Validator.prototype.isMACAddress = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isMACAddress(this.value))) {
		this.addError(tip || this.key + " is not a MAC address format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isIn"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isIn (arr, tip)](#apidoc.element.koa-validate.Validator.prototype.isIn)
- description and source-code
```javascript
isIn = function (arr, tip) {
	if (this.goOn && arr) {
		for(var i = 0 ; i < arr.length ;i++){
			if(this.value == arr[i]){
				return this;
			}
		}
		this.addError(tip || this.key + " must be in [" + arr.join(',') + "].");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isInt"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isInt (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isInt)
- description and source-code
```javascript
isInt = function (tip, options) {
	if (this.goOn&& !v.isInt(String(this.value), options)) {
		this.addError(tip || this.key + " is not integer.");
	}
	return this;
}
```
- example usage
```shell
...
    if (this.goOn && !assertion) {
        this.addError(tip || this.key + ' failed an assertion.');
    }
    return this;
};

Validator.prototype.isInt = function(tip, options) {
	if (this.goOn&& !v.isInt(String(this.value), options)) {
		this.addError(tip || this.key + " is not integer.");
	}
	return this;
};
Validator.prototype.isFloat = function(tip,options) {
	if (this.goOn && !v.isFloat(String(this.value), options)) {
		this.addError(tip || this.key + " is not float.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isIp"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isIp (tip, version)](#apidoc.element.koa-validate.Validator.prototype.isIp)
- description and source-code
```javascript
isIp = function (tip, version) {
	if (this.goOn && (!isString(this.value) ||!v.isIP(this.value,version))) {
		this.addError(tip || this.key + " is not ip format.");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isJSON"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isJSON (tip)](#apidoc.element.koa-validate.Validator.prototype.isJSON)
- description and source-code
```javascript
isJSON = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isJSON(this.value))) {
		this.addError(tip || this.key + " is not a json format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isISBN = function(tip,version) {
	if (this.goOn && (!isString(this.value) ||!v.isISBN(this.value,version))) {
		this.addError(tip || this.key + " is not a ISBN format.");
	}
	return this;
};
Validator.prototype.isJSON = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isJSON(this.value))) {
		this.addError(tip || this.key + " is not a json format.");
	}
	return this;
};

Validator.prototype.isMultibyte = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isMultibyte(this.value))) {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isLength"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isLength (min, max, tip)](#apidoc.element.koa-validate.Validator.prototype.isLength)
- description and source-code
```javascript
isLength = function (min, max, tip) {
	min = min || 0;
	tip = 'number' != typeof max ? max : tip;
	max = 'number' == typeof max ? max :-1;
	this.exist(tip);
	if (this.goOn) {
		if(this.value.length<min) {
			this.addError(tip || this.key + "'s length must equal or great than " + min+".");
			return this;
		}
		if (-1!=max&&this.value.length>max) {
			this.addError(tip || this.key + "'s length must equal or less than " + max + ".");
			return this;
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isLowercase"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isLowercase (tip)](#apidoc.element.koa-validate.Validator.prototype.isLowercase)
- description and source-code
```javascript
isLowercase = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isLowercase(this.value))) {
		this.addError(tip || this.key + " is not a lowwer case string");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isHexColor = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHexColor(this.value))) {
		this.addError(tip || this.key + " is  not hex color format.");
	}
	return this;
};
Validator.prototype.isLowercase = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isLowercase(this.value))) {
		this.addError(tip || this.key + " is not a lowwer case string");
	}
	return this;
};
Validator.prototype.isUppercase = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isUppercase(this.value))) {
		this.addError(tip || this.key + " is not a upper case string.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isMACAddress"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isMACAddress (tip)](#apidoc.element.koa-validate.Validator.prototype.isMACAddress)
- description and source-code
```javascript
isMACAddress = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isMACAddress(this.value))) {
		this.addError(tip || this.key + " is not a MAC address format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isISO8601 = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isISO8601(this.value))) {
		this.addError(tip || this.key + " is not a ISO8601 string format.");
	}
	return this;
};
Validator.prototype.isMACAddress = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isMACAddress(this.value))) {
		this.addError(tip || this.key + " is not a MAC address format.");
	}
	return this;
};

Validator.prototype.isISIN = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isISIN(this.value))) {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isMobilePhone"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isMobilePhone (tip, locale)](#apidoc.element.koa-validate.Validator.prototype.isMobilePhone)
- description and source-code
```javascript
isMobilePhone = function (tip, locale) {
	if (this.goOn && (!isString(this.value) ||!v.isMobilePhone(this.value,locale))) {
		this.addError(tip || this.key + " is not a mobile phone format.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isDataURI = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isDataURI(this.value))) {
		this.addError(tip || this.key + " is not a data uri format.");
	}
	return this;
};
Validator.prototype.isMobilePhone = function(tip,locale) {
	if (this.goOn && (!isString(this.value) ||!v.isMobilePhone(this.value,locale))) {
		this.addError(tip || this.key + " is not a mobile phone format.");
	}
	return this;
};
Validator.prototype.isISO8601 = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isISO8601(this.value))) {
		this.addError(tip || this.key + " is not a ISO8601 string format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isMultibyte"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isMultibyte (tip)](#apidoc.element.koa-validate.Validator.prototype.isMultibyte)
- description and source-code
```javascript
isMultibyte = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isMultibyte(this.value))) {
		this.addError(tip || this.key + " is not a multibyte string.");
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && (!isString(this.value) ||!v.isJSON(this.value))) {
		this.addError(tip || this.key + " is not a json format.");
	}
	return this;
};

Validator.prototype.isMultibyte = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isMultibyte(this.value))) {
		this.addError(tip || this.key + " is not a multibyte string.");
	}
	return this;
};
Validator.prototype.isAscii = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isAscii(this.value))) {
		this.addError(tip || this.key + " is not a ascii string.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isNull"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isNull (tip)](#apidoc.element.koa-validate.Validator.prototype.isNull)
- description and source-code
```javascript
isNull = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isNull(this.value))) {
		this.addError(tip || this.key + " is not null.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isDivisibleBy = function(n, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isDivisibleBy(this.value, n))) {
		this.addError(tip || this.key + " can not divide by" + n + ".");
	}
	return this;
};
Validator.prototype.isNull = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isNull(this.value))) {
		this.addError(tip || this.key + " is not null.");
	}
	return this;
};
Validator.prototype.isByteLength = function(min, max,charset,tip) {
	min = min || 0;
	max = max || Number.MAX_VALUE;
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isNumeric"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isNumeric (tip)](#apidoc.element.koa-validate.Validator.prototype.isNumeric)
- description and source-code
```javascript
isNumeric = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isNumeric(this.value))) {
		this.addError(tip || this.key + " is  not numeric.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isAlpha = function(tip,locale) {
	if (this.goOn && (!isString(this.value) ||!v.isAlpha(this.value,locale))) {
		this.addError(tip || this.key + " is not an alpha string.");
	}
	return this;
};
Validator.prototype.isNumeric = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isNumeric(this.value))) {
		this.addError(tip || this.key + " is  not numeric.");
	}
	return this;
};

Validator.prototype.isAlphanumeric = function(tip,locale) {
	if (this.goOn && (!isString(this.value) ||!v.isAlphanumeric(this.value,locale))) {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isSurrogatePair"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isSurrogatePair (tip)](#apidoc.element.koa-validate.Validator.prototype.isSurrogatePair)
- description and source-code
```javascript
isSurrogatePair = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isSurrogatePair(this.value))) {
		this.addError(tip || this.key + " is not a surrogate pair string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isVariableWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isVariableWidth(this.value))) {
		this.addError(tip || this.key + " is not a variable width string.");
	}
	return this;
};
Validator.prototype.isSurrogatePair = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isSurrogatePair(this.value))) {
		this.addError(tip || this.key + " is not a surrogate pair string.");
	}
	return this;
};
Validator.prototype.isCurrency = function(tip,options) {
	if (this.goOn && (!isString(this.value) ||!v.isCurrency(this.value,options))) {
		this.addError(tip || this.key + " is not a currency format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isTime"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isTime (tip)](#apidoc.element.koa-validate.Validator.prototype.isTime)
- description and source-code
```javascript
isTime = function (tip) {
	var timeReg = /^(([0-1]?[0-9])|([2][0-3])):([0-5]?[0-9])(:([0-5]?[0-9]))?$/;
	if(this.goOn && ! timeReg.test(this.value)){
		this.addError(tip || this.key + " is not a time format.");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isUUID"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isUUID (tip, ver)](#apidoc.element.koa-validate.Validator.prototype.isUUID)
- description and source-code
```javascript
isUUID = function (tip, ver) {
	if (this.goOn && (!isString(this.value) ||!v.isUUID(this.value,ver))) {
		this.addError(tip || this.key + " is not a UUID format.");
	}
	return this;
}
```
- example usage
```shell
...
			this.addError(tip || this.key + "'s byte lenth great than " + min +" and less than " + max + "." );
		}
	}
	return this;
};
Validator.prototype.byteLength = Validator.prototype.isByteLength;
Validator.prototype.isUUID = function(tip,ver) {
	if (this.goOn && (!isString(this.value) ||!v.isUUID(this.value,ver))) {
		this.addError(tip || this.key + " is not a UUID format.");
	}
	return this;
};
Validator.prototype.isDate = function(tip) {
	if (this.goOn && !util.isDate(this.value)  && (!isString(this.value) ||!v.isDate(this.value))) {
		this.addError(tip || this.key + " is not a date format.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isUppercase"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isUppercase (tip)](#apidoc.element.koa-validate.Validator.prototype.isUppercase)
- description and source-code
```javascript
isUppercase = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isUppercase(this.value))) {
		this.addError(tip || this.key + " is not a upper case string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isLowercase = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isLowercase(this.value))) {
		this.addError(tip || this.key + " is not a lowwer case string");
	}
	return this;
};
Validator.prototype.isUppercase = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isUppercase(this.value))) {
		this.addError(tip || this.key + " is not a upper case string.");
	}
	return this;
};
Validator.prototype.isDivisibleBy = function(n, tip) {
	if (this.goOn && (!isString(this.value) ||!v.isDivisibleBy(this.value, n))) {
		this.addError(tip || this.key + " can not divide by" + n + ".");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isUrl"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isUrl (tip, options)](#apidoc.element.koa-validate.Validator.prototype.isUrl)
- description and source-code
```javascript
isUrl = function (tip, options) {
	if (this.goOn && (!isString(this.value) ||!v.isURL(this.value,options))) {
		this.addError(tip || this.key + " is not url format.");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.isVariableWidth"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>isVariableWidth (tip)](#apidoc.element.koa-validate.Validator.prototype.isVariableWidth)
- description and source-code
```javascript
isVariableWidth = function (tip) {
	if (this.goOn && (!isString(this.value) ||!v.isVariableWidth(this.value))) {
		this.addError(tip || this.key + " is not a variable width string.");
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.isHalfWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isHalfWidth(this.value))) {
		this.addError(tip || this.key + " is not a half width string.");
	}
	return this;
};
Validator.prototype.isVariableWidth = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isVariableWidth(this.value))) {
		this.addError(tip || this.key + " is not a variable width string.");
	}
	return this;
};
Validator.prototype.isSurrogatePair = function(tip) {
	if (this.goOn && (!isString(this.value) ||!v.isSurrogatePair(this.value))) {
		this.addError(tip || this.key + " is not a surrogate pair string.");
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.le"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>le (l, tip)](#apidoc.element.koa-validate.Validator.prototype.le)
- description and source-code
```javascript
le = function (l, tip) {
	if (this.goOn && this.value > l) {
		this.addError(tip || this.key + " must less than or equal " + l + ".");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.len"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>len (min, max, tip)](#apidoc.element.koa-validate.Validator.prototype.len)
- description and source-code
```javascript
len = function (min, max, tip) {
	min = min || 0;
	tip = 'number' != typeof max ? max : tip;
	max = 'number' == typeof max ? max :-1;
	this.exist(tip);
	if (this.goOn) {
		if(this.value.length<min) {
			this.addError(tip || this.key + "'s length must equal or great than " + min+".");
			return this;
		}
		if (-1!=max&&this.value.length>max) {
			this.addError(tip || this.key + "'s length must equal or less than " + max + ".");
			return this;
		}
	}
	return this;
}
```
- example usage
```shell
...
var router = require('koa-router')();
require('koa-validate')(app);

app.use(require('koa-body')({multipart:true , formidable:{keepExtensions:true}}));
app.use(router.routes()).use(router.allowedMethods());
router.post('/signup', function * () {
	//optional() means this param may not in the params.
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.lt"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>lt (l, tip)](#apidoc.element.koa-validate.Validator.prototype.lt)
- description and source-code
```javascript
lt = function (l, tip) {
	if (this.goOn && this.value >= l) {
		this.addError(tip || this.key + " must less than " + l + ".");
	}
	return this;
}
```
- example usage
```shell
...
		this.body = this.errors;
		return;
	}
});
router.get('/users', function * () {
	this.checkQuery('department').empty().in(["sale","finance"], "not support this department!").len(3, 20);	
	this.checkQuery('name').empty().len(2,20,"bad name.").trim().toLow();
	this.checkQuery('age').empty().gt(10,"too young!").lt(30,"to old!").toInt();
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
router.get('/user/:id', function * () {
	this.checkParams('id').toInt(0);
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.ltrim"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>ltrim (c)](#apidoc.element.koa-validate.Validator.prototype.ltrim)
- description and source-code
```javascript
ltrim = function (c) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.ltrim(this.value,c);
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.trim(this.value,c);
	}
	return this;
};
Validator.prototype.ltrim = function(c) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.ltrim(this.value,c);
	}
	return this;
};
Validator.prototype.rtrim = function(c) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.rtrim(this.value,c);
	}
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.match"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>match (reg, tip)](#apidoc.element.koa-validate.Validator.prototype.match)
- description and source-code
```javascript
match = function (reg, tip) {
	if (this.goOn && !reg.test(this.value)) {
		this.addError(tip || this.key + " is bad format.");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.md5"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>md5 ()](#apidoc.element.koa-validate.Validator.prototype.md5)
- description and source-code
```javascript
md5 = function () {
	this.hash('md5');
	return this;
}
```
- example usage
```shell
...

app.use(require('koa-body')({multipart:true , formidable:{keepExtensions:true}}));
app.use(router.routes()).use(router.allowedMethods());
router.post('/signup', function * () {
	//optional() means this param may not in the params.
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
		//resize image
	});
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.neq"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>neq (l, tip)](#apidoc.element.koa-validate.Validator.prototype.neq)
- description and source-code
```javascript
neq = function (l, tip) {
	if (this.goOn && this.value == l) {
		this.addError(tip || this.key + " is must not equal " + l + ".");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.notBlank"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>notBlank (tip)](#apidoc.element.koa-validate.Validator.prototype.notBlank)
- description and source-code
```javascript
notBlank = function (tip) {
	if (this.goOn && (null==this.value||'undefined'==typeof(this.value) || ('string' == typeof(this.value) &&(/^\s*$/gi).test(this.
value)))) {
		this.addError(tip || this.key + " can not be blank.");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.notContains"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>notContains (s, tip)](#apidoc.element.koa-validate.Validator.prototype.notContains)
- description and source-code
```javascript
notContains = function (s, tip) {
	if (this.goOn && (!isString(this.value) ||v.contains(this.value,s))) {
		this.addError(tip || this.key + " is must not contain " + s + ".");
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.notEmpty"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>notEmpty (tip)](#apidoc.element.koa-validate.Validator.prototype.notEmpty)
- description and source-code
```javascript
notEmpty = function (tip) {
	if (this.goOn && (null==this.value||'undefined'==typeof(this.value) || ('string' == typeof(this.value) &&!this.value))) {
		this.addError(tip || this.key + " can not be empty.");
	}
	return this;
}
```
- example usage
```shell
...

app.use(require('koa-body')({multipart:true , formidable:{keepExtensions:true}}));
app.use(router.routes()).use(router.allowedMethods());
router.post('/signup', function * () {
	//optional() means this param may not in the params.
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
		//resize image
	});
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.notMatch"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>notMatch (reg, tip)](#apidoc.element.koa-validate.Validator.prototype.notMatch)
- description and source-code
```javascript
notMatch = function (reg, tip) {
    if (this.goOn && reg.test(this.value)) {
        this.addError(tip || this.key + ' is bad format.');
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.optional"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>optional ()](#apidoc.element.koa-validate.Validator.prototype.optional)
- description and source-code
```javascript
optional = function () {
	if (!this.exists) {
		this.goOn = false;
	}
	return this;
}
```
- example usage
```shell
...
var router = require('koa-router')();
require('koa-validate')(app);

app.use(require('koa-body')({multipart:true , formidable:{keepExtensions:true}}));
app.use(router.routes()).use(router.allowedMethods());
router.post('/signup', function * () {
	//optional() means this param may not in the params.
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.replace"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>replace (a, b)](#apidoc.element.koa-validate.Validator.prototype.replace)
- description and source-code
```javascript
replace = function (a, b) {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = this.value.replace(a,b);
	}
	return this;
}
```
- example usage
```shell
...
			this.addError(tip||'bad uri to decode.');
		}
	}
	return this;
};
Validator.prototype.replace = function(a,b) {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = this.value.replace(a,b);
	}
	return this;
};
Validator.prototype.encodeBase64 = function() {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = new Buffer(this.value).toString('base64');
	}
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.rtrim"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>rtrim (c)](#apidoc.element.koa-validate.Validator.prototype.rtrim)
- description and source-code
```javascript
rtrim = function (c) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.rtrim(this.value,c);
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.ltrim(this.value,c);
	}
	return this;
};
Validator.prototype.rtrim = function(c) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.rtrim(this.value,c);
	}
	return this;
};
Validator.prototype.escape = function() {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.escape(this.value);
	}
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.sha1"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>sha1 ()](#apidoc.element.koa-validate.Validator.prototype.sha1)
- description and source-code
```javascript
sha1 = function () {
	this.hash('sha1');
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.stripLow"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>stripLow (nl)](#apidoc.element.koa-validate.Validator.prototype.stripLow)
- description and source-code
```javascript
stripLow = function (nl) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.stripLow(this.value, nl);
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.escape(this.value);
	}
	return this;
};
Validator.prototype.stripLow = function(nl) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.stripLow(this.value, nl);
	}
	return this;
};
Validator.prototype.whitelist = function(s) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.whitelist(this.value,s);
	}
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toBoolean"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toBoolean ()](#apidoc.element.koa-validate.Validator.prototype.toBoolean)
- description and source-code
```javascript
toBoolean = function () {
	if (this.goOn && !this.hasError()) {
		if('boolean' == typeof(this.value)) {
			return this;
		}
		if('string' == typeof(this.value)){
			this.value = this.params[this.key] = v.toBoolean(this.value);
		}
	}
	return this;
}
```
- example usage
```shell
...
Validator.prototype.toUp = Validator.prototype.toUppercase;
Validator.prototype.toBoolean = function() {
	if (this.goOn && !this.hasError()) {
		if('boolean' == typeof(this.value)) {
			return this;
		}
		if('string' == typeof(this.value)){
			this.value = this.params[this.key] = v.toBoolean(this.value);
		}
	}
	return this;
};
Validator.prototype.trim = function(c) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.trim(this.value,c);
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toDate"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toDate ()](#apidoc.element.koa-validate.Validator.prototype.toDate)
- description and source-code
```javascript
toDate = function () {
	this.isDate();
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.toDate(this.value);
	}
	return this;
}
```
- example usage
```shell
...
		this.value = this.params[this.key] = d;
	}
	return this;
};
Validator.prototype.toDate = function() {
	this.isDate();
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.toDate(this.value);
	}
	return this;
};
Validator.prototype.toInt = function(tip, radix, options) {
	this.isInt(tip, options);
	if (this.goOn && !this.hasError()) {
		if('number' == typeof(this.value)) {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toFloat"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toFloat (tip)](#apidoc.element.koa-validate.Validator.prototype.toFloat)
- description and source-code
```javascript
toFloat = function (tip) {
	this.isFloat(tip);
	if (this.goOn && !this.hasError()) {
		if('number' == typeof(this.value)) {
			return this;
		}
		this.value = this.params[this.key] = v.toFloat(this.value);
	}
	return this;
}
```
- example usage
```shell
...
};
Validator.prototype.toFloat = function(tip) {
	this.isFloat(tip);
	if (this.goOn && !this.hasError()) {
		if('number' == typeof(this.value)) {
			return this;
		}
		this.value = this.params[this.key] = v.toFloat(this.value);
	}
	return this;
};
Validator.prototype.toJson = function(tip) {
	if (this.goOn && !this.hasError()) {
		try{
			if('object' == typeof(this.value)) {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toInt"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toInt (tip, radix, options)](#apidoc.element.koa-validate.Validator.prototype.toInt)
- description and source-code
```javascript
toInt = function (tip, radix, options) {
	this.isInt(tip, options);
	if (this.goOn && !this.hasError()) {
		if('number' == typeof(this.value)) {
			return this;
		}
		this.value = this.params[this.key] = v.toInt(this.value, radix);
	}
	return this;
}
```
- example usage
```shell
...
	//optional() means this param may not in the params.
	this.checkBody('name').optional().len(2, 20,"are you kidding me?");
	this.checkBody('email').isEmail("your enter a bad email.");
	this.checkBody('password').notEmpty().len(3, 20).md5();
	//empty() mean this param can be a empty string.
	this.checkBody('nick').optional().empty().len(3, 20);
	//also we can get the sanitized value
	var age = this.checkBody('age').toInt().value;
	yield this.checkFile('icon').notEmpty().size(0,300*1024,'file too large').move("/static/icon/" , function*(file,context){
		//resize image
	});
	if (this.errors) {
		this.body = this.errors;
		return;
	}
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toJson"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toJson (tip)](#apidoc.element.koa-validate.Validator.prototype.toJson)
- description and source-code
```javascript
toJson = function (tip) {
	if (this.goOn && !this.hasError()) {
		try{
			if('object' == typeof(this.value)) {
				return this;
			}
			this.value = this.params[this.key] = JSON.parse(this.value);
		}catch(e){
			this.addError(tip||'not json format');
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toLow"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toLow ()](#apidoc.element.koa-validate.Validator.prototype.toLow)
- description and source-code
```javascript
toLow = function () {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = this.value.toLowerCase();
	}
	return this;
}
```
- example usage
```shell
...
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
router.get('/users', function * () {
	this.checkQuery('department').empty().in(["sale","finance"], "not support this department!").len(3, 20);	
	this.checkQuery('name').empty().len(2,20,"bad name.").trim().toLow();
	this.checkQuery('age').empty().gt(10,"too young!").lt(30,"to old!").toInt();
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
router.get('/user/:id', function * () {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toLowercase"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toLowercase ()](#apidoc.element.koa-validate.Validator.prototype.toLowercase)
- description and source-code
```javascript
toLowercase = function () {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = this.value.toLowerCase();
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toUp"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toUp ()](#apidoc.element.koa-validate.Validator.prototype.toUp)
- description and source-code
```javascript
toUp = function () {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = this.value.toUpperCase();
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.toUppercase"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>toUppercase ()](#apidoc.element.koa-validate.Validator.prototype.toUppercase)
- description and source-code
```javascript
toUppercase = function () {
	if (this.goOn && !this.hasError()&&this.value) {
		this.value = this.params[this.key] = this.value.toUpperCase();
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.trim"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>trim (c)](#apidoc.element.koa-validate.Validator.prototype.trim)
- description and source-code
```javascript
trim = function (c) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.trim(this.value,c);
	}
	return this;
}
```
- example usage
```shell
...
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
router.get('/users', function * () {
	this.checkQuery('department').empty().in(["sale","finance"], "not support this department!").len(3, 20);	
	this.checkQuery('name').empty().len(2,20,"bad name.").trim().toLow();
	this.checkQuery('age').empty().gt(10,"too young!").lt(30,"to old!").toInt();
	if (this.errors) {
		this.body = this.errors;
		return;
	}
});
router.get('/user/:id', function * () {
...
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.type"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>type (t, tip)](#apidoc.element.koa-validate.Validator.prototype.type)
- description and source-code
```javascript
type = function (t, tip) {
	if(this.value){
		if('boolean'==t || 'string'==t|| 'number' == t || 'object' == t || 'undefined' ==t){
			if(t!=typeof(this.value)) this.addError(tip|| this.key+" is not "+t+"");
		}else if ('array' == t){
			if(!util.isArray(this.value)) this.addError(tip|| this.key+" is not array");
		}else if ('date' == t){
			if(!util.isDate(this.value)) this.addError(tip|| this.key+" is not date.");
		}else if ('null' == t){
			if(!util.isNull(this.value)) this.addError(tip|| this.key+" is not null.");
		}else if ('nullorundefined' == t.toLowerCase()){
			if(!util.isNullOrUndefined(this.value)) this.addError(tip|| this.key+" is not primitive type.");
		}else if ('primitive' == t){
			if(!util.isPrimitive(this.value)) this.addError(tip|| this.key+" is not primitive type.");
		}else{
			console.warn("not support this type check,type:'"+t+"'")
		}
	}
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-validate.Validator.prototype.whitelist"></a>[function <span class="apidocSignatureSpan">koa-validate.Validator.prototype.</span>whitelist (s)](#apidoc.element.koa-validate.Validator.prototype.whitelist)
- description and source-code
```javascript
whitelist = function (s) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.whitelist(this.value,s);
	}
	return this;
}
```
- example usage
```shell
...
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.stripLow(this.value, nl);
	}
	return this;
};
Validator.prototype.whitelist = function(s) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.whitelist(this.value,s);
	}
	return this;
};
Validator.prototype.blacklist = function(s) {
	if (this.goOn && !this.hasError()) {
		this.value = this.params[this.key] = v.blacklist(this.value,s);
	}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
