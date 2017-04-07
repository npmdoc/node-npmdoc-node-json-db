# api documentation for  [node-json-db (v0.7.3)](https://github.com/Belphemur/node-json-db)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-json-db.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-json-db) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-json-db.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-json-db)
#### Database using JSON file as storage for Node.JS

[![NPM](https://nodei.co/npm/node-json-db.png?downloads=true)](https://www.npmjs.com/package/node-json-db)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-json-db/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-json-db_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-json-db/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-json-db/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-json-db/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Antoine Aflalo",
        "email": "antoineaf+npm@admincmd.com"
    },
    "bugs": {
        "url": "https://github.com/Belphemur/node-json-db/issues"
    },
    "dependencies": {
        "mkdirp": "0.5.x"
    },
    "description": "Database using JSON file as storage for Node.JS",
    "devDependencies": {
        "expect.js": "0.3.x",
        "grunt": "0.4.x",
        "grunt-cli": "0.1.x",
        "grunt-contrib-jshint": "0.11.x",
        "grunt-simple-mocha": "0.4.x",
        "mocha": "2.4.x"
    },
    "directories": {},
    "dist": {
        "shasum": "bf631ff4d4cf4211cbdffe6cae6aaafe6ee54cdf",
        "tarball": "https://registry.npmjs.org/node-json-db/-/node-json-db-0.7.3.tgz"
    },
    "gitHead": "d335bc9a83b3db3c8a4dcf8cfa394a07c4870370",
    "homepage": "https://github.com/Belphemur/node-json-db",
    "keywords": [
        "database",
        "json",
        "db"
    ],
    "license": "MIT",
    "main": "./JsonDB.js",
    "maintainers": [
        {
            "name": "belphemur",
            "email": "antoineaf+npm@admincmd.com"
        }
    ],
    "name": "node-json-db",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/Belphemur/node-json-db.git"
    },
    "scripts": {
        "test": "mocha test/test.js"
    },
    "version": "0.7.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-json-db](#apidoc.module.node-json-db)
1.  [function <span class="apidocSignatureSpan">node-json-db.</span>ArrayInfo (property, index)](#apidoc.element.node-json-db.ArrayInfo)
1.  [function <span class="apidocSignatureSpan">node-json-db.</span>DBParentData (parent, data, jsonDB, dataPath)](#apidoc.element.node-json-db.DBParentData)
1.  object <span class="apidocSignatureSpan">node-json-db.</span>ArrayInfo.prototype
1.  object <span class="apidocSignatureSpan">node-json-db.</span>DBParentData.prototype
1.  object <span class="apidocSignatureSpan">node-json-db.</span>Errors
1.  object <span class="apidocSignatureSpan">node-json-db.</span>utils

#### [module node-json-db.ArrayInfo](#apidoc.module.node-json-db.ArrayInfo)
1.  [function <span class="apidocSignatureSpan">node-json-db.</span>ArrayInfo (property, index)](#apidoc.element.node-json-db.ArrayInfo.ArrayInfo)

#### [module node-json-db.ArrayInfo.prototype](#apidoc.module.node-json-db.ArrayInfo.prototype)
1.  [function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>delete (data)](#apidoc.element.node-json-db.ArrayInfo.prototype.delete)
1.  [function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>getData (data)](#apidoc.element.node-json-db.ArrayInfo.prototype.getData)
1.  [function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>getIndex (data, avoidProperty)](#apidoc.element.node-json-db.ArrayInfo.prototype.getIndex)
1.  [function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>isValid (data)](#apidoc.element.node-json-db.ArrayInfo.prototype.isValid)
1.  [function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>setData (data, value)](#apidoc.element.node-json-db.ArrayInfo.prototype.setData)

#### [module node-json-db.DBParentData](#apidoc.module.node-json-db.DBParentData)
1.  [function <span class="apidocSignatureSpan">node-json-db.</span>DBParentData (parent, data, jsonDB, dataPath)](#apidoc.element.node-json-db.DBParentData.DBParentData)

#### [module node-json-db.DBParentData.prototype](#apidoc.module.node-json-db.DBParentData.prototype)
1.  [function <span class="apidocSignatureSpan">node-json-db.DBParentData.prototype.</span>_checkArray (deletion)](#apidoc.element.node-json-db.DBParentData.prototype._checkArray)
1.  [function <span class="apidocSignatureSpan">node-json-db.DBParentData.prototype.</span>delete ()](#apidoc.element.node-json-db.DBParentData.prototype.delete)
1.  [function <span class="apidocSignatureSpan">node-json-db.DBParentData.prototype.</span>getData ()](#apidoc.element.node-json-db.DBParentData.prototype.getData)
1.  [function <span class="apidocSignatureSpan">node-json-db.DBParentData.prototype.</span>setData (toSet)](#apidoc.element.node-json-db.DBParentData.prototype.setData)

#### [module node-json-db.Errors](#apidoc.module.node-json-db.Errors)
1.  [function <span class="apidocSignatureSpan">node-json-db.Errors.</span>DataError (msg, id, nested)](#apidoc.element.node-json-db.Errors.DataError)
1.  [function <span class="apidocSignatureSpan">node-json-db.Errors.</span>DatabaseError (msg, id, nested)](#apidoc.element.node-json-db.Errors.DatabaseError)

#### [module node-json-db.utils](#apidoc.module.node-json-db.utils)
1.  [function <span class="apidocSignatureSpan">node-json-db.utils.</span>mergeObject ()](#apidoc.element.node-json-db.utils.mergeObject)
1.  [function <span class="apidocSignatureSpan">node-json-db.utils.</span>processArray (property)](#apidoc.element.node-json-db.utils.processArray)
1.  [function <span class="apidocSignatureSpan">node-json-db.utils.</span>removeTrailingSlash (dataPath)](#apidoc.element.node-json-db.utils.removeTrailingSlash)
1.  [function <span class="apidocSignatureSpan">node-json-db.utils.</span>strEndWith (str, suffix)](#apidoc.element.node-json-db.utils.strEndWith)



# <a name="apidoc.module.node-json-db"></a>[module node-json-db](#apidoc.module.node-json-db)

#### <a name="apidoc.element.node-json-db.ArrayInfo"></a>[function <span class="apidocSignatureSpan">node-json-db.</span>ArrayInfo (property, index)](#apidoc.element.node-json-db.ArrayInfo)
- description and source-code
```javascript
function ArrayInfo(property, index) {
    this.property = property;
    this.index = index;
    this.append = index === "";
    if (isInt(this.index)) {
        this.index = parseInt(this.index);
    } else if (!this.append) {
        throw new DataError("Only numerical values accepted for array index", 200)
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-json-db.DBParentData"></a>[function <span class="apidocSignatureSpan">node-json-db.</span>DBParentData (parent, data, jsonDB, dataPath)](#apidoc.element.node-json-db.DBParentData)
- description and source-code
```javascript
function DBParentData(parent, data, jsonDB, dataPath) {
    this.parent = parent;
    this.data = data;
    this.db = jsonDB;
    this.dataPath = dataPath;

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-json-db.ArrayInfo"></a>[module node-json-db.ArrayInfo](#apidoc.module.node-json-db.ArrayInfo)

#### <a name="apidoc.element.node-json-db.ArrayInfo.ArrayInfo"></a>[function <span class="apidocSignatureSpan">node-json-db.</span>ArrayInfo (property, index)](#apidoc.element.node-json-db.ArrayInfo.ArrayInfo)
- description and source-code
```javascript
function ArrayInfo(property, index) {
    this.property = property;
    this.index = index;
    this.append = index === "";
    if (isInt(this.index)) {
        this.index = parseInt(this.index);
    } else if (!this.append) {
        throw new DataError("Only numerical values accepted for array index", 200)
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-json-db.ArrayInfo.prototype"></a>[module node-json-db.ArrayInfo.prototype](#apidoc.module.node-json-db.ArrayInfo.prototype)

#### <a name="apidoc.element.node-json-db.ArrayInfo.prototype.delete"></a>[function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>delete (data)](#apidoc.element.node-json-db.ArrayInfo.prototype.delete)
- description and source-code
```javascript
delete = function (data) {
    var index = this.getIndex(data);
    data[this.property].splice(index, 1);
}
```
- example usage
```shell
...
} catch(error) {
//The error will tell you where the DataPath stopped. In this case test1
//Since /test1/test does't exist.
    console.error(error);
}

//Deleting data
db.delete("/test1");

//Save the data (useful if you disable the saveOnPush)
db.save();

//In case you have a exterior change to the databse file and want to reload it
//use this method
db.reload();
...
```

#### <a name="apidoc.element.node-json-db.ArrayInfo.prototype.getData"></a>[function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>getData (data)](#apidoc.element.node-json-db.ArrayInfo.prototype.getData)
- description and source-code
```javascript
getData = function (data) {
    if (this.append) {
        throw new DataError("Can't get data when appending", 100);
    }
    var index = this.getIndex(data);
    return data[this.property][index];
}
```
- example usage
```shell
...
*/
//You can't merge primitive.
//If you do this:
db.push("/test2/my/test/",10,false);
//the data will be overriden

//Get the data from the root
var data = db.getData("/");

//From a particular DataPath
var data = db.getData("/test1");

//If you try to get some data from a DataPath that doesn't exists
//You'll get an Error
try {
...
```

#### <a name="apidoc.element.node-json-db.ArrayInfo.prototype.getIndex"></a>[function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>getIndex (data, avoidProperty)](#apidoc.element.node-json-db.ArrayInfo.prototype.getIndex)
- description and source-code
```javascript
getIndex = function (data, avoidProperty) {
    if (avoidProperty === undefined) {
        avoidProperty = false;
    }
    var index = this.index;
    if (index == -1) {
        var dataIterable = avoidProperty ? data : data[this.property];

        if (dataIterable.length === 0) {
            return 0;
        }
        return dataIterable.length - 1;
    }
    return index;
}
```
- example usage
```shell
...
 * @returns {*}
 * @constructor
 */
ArrayInfo.prototype.getData = function (data) {
    if (this.append) {
        throw new DataError("Can't get data when appending", 100);
    }
    var index = this.getIndex(data);
    return data[this.property][index];
};

/**
 * Set the data for the array
 * @param data
 * @param value
...
```

#### <a name="apidoc.element.node-json-db.ArrayInfo.prototype.isValid"></a>[function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>isValid (data)](#apidoc.element.node-json-db.ArrayInfo.prototype.isValid)
- description and source-code
```javascript
isValid = function (data) {
    var index = this.getIndex(data);
    return data[this.property].hasOwnProperty(index);
}
```
- example usage
```shell
...
 */
DBParentData.prototype._checkArray = function (deletion) {
    if(typeof deletion === undefined) {
        deletion = false;
    }
    var arrayInfo = JsonUtils.processArray(this.parent);
    if (arrayInfo) {
        if ((!arrayInfo.append || deletion) && !arrayInfo.isValid(this.data)) {
            throw new DataError("DataPath: /" + this.dataPath + ". Can't find index " + arrayInfo.index + " in array " + arrayInfo
.property, 10);
        }
    }
    return arrayInfo;
};

DBParentData.prototype.getData = function () {
...
```

#### <a name="apidoc.element.node-json-db.ArrayInfo.prototype.setData"></a>[function <span class="apidocSignatureSpan">node-json-db.ArrayInfo.prototype.</span>setData (data, value)](#apidoc.element.node-json-db.ArrayInfo.prototype.setData)
- description and source-code
```javascript
setData = function (data, value) {
    if (this.append) {
        data[this.property].push(value);
    } else {
        var index = this.getIndex(data);
        data[this.property][index] = value;
    }
}
```
- example usage
```shell
...
    var arrayInfo = JsonUtils.processArray(this.parent);
    if (arrayInfo) {
        if (!this.data.hasOwnProperty(arrayInfo.property)) {
            this.data[arrayInfo.property] = [];
        } else if (!Array.isArray(this.data[arrayInfo.property])) {
            throw new DataError("DataPath: /" + this.dataPath + ". " + arrayInfo.property + " is not an array.", 11);
        }
        arrayInfo.setData(this.data, toSet);
    } else {
        this.data[this.parent] = toSet;
    }
};

DBParentData.prototype.delete = function () {
    if (this.parent === undefined) {
...
```



# <a name="apidoc.module.node-json-db.DBParentData"></a>[module node-json-db.DBParentData](#apidoc.module.node-json-db.DBParentData)

#### <a name="apidoc.element.node-json-db.DBParentData.DBParentData"></a>[function <span class="apidocSignatureSpan">node-json-db.</span>DBParentData (parent, data, jsonDB, dataPath)](#apidoc.element.node-json-db.DBParentData.DBParentData)
- description and source-code
```javascript
function DBParentData(parent, data, jsonDB, dataPath) {
    this.parent = parent;
    this.data = data;
    this.db = jsonDB;
    this.dataPath = dataPath;

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-json-db.DBParentData.prototype"></a>[module node-json-db.DBParentData.prototype](#apidoc.module.node-json-db.DBParentData.prototype)

#### <a name="apidoc.element.node-json-db.DBParentData.prototype._checkArray"></a>[function <span class="apidocSignatureSpan">node-json-db.DBParentData.prototype.</span>_checkArray (deletion)](#apidoc.element.node-json-db.DBParentData.prototype._checkArray)
- description and source-code
```javascript
_checkArray = function (deletion) {
    if(typeof deletion === undefined) {
        deletion = false;
    }
    var arrayInfo = JsonUtils.processArray(this.parent);
    if (arrayInfo) {
        if ((!arrayInfo.append || deletion) && !arrayInfo.isValid(this.data)) {
            throw new DataError("DataPath: /" + this.dataPath + ". Can't find index " + arrayInfo.index + " in array " + arrayInfo
.property, 10);
        }
    }
    return arrayInfo;
}
```
- example usage
```shell
...
    return arrayInfo;
};

DBParentData.prototype.getData = function () {
    if (this.parent === undefined) {
        return this.data;
    }
    var arrayInfo = this._checkArray();
    if (arrayInfo) {
        return arrayInfo.getData(this.data);
    } else {
        return this.data[this.parent];
    }
};
...
```

#### <a name="apidoc.element.node-json-db.DBParentData.prototype.delete"></a>[function <span class="apidocSignatureSpan">node-json-db.DBParentData.prototype.</span>delete ()](#apidoc.element.node-json-db.DBParentData.prototype.delete)
- description and source-code
```javascript
delete = function () {
    if (this.parent === undefined) {
        this.db.data = {};
    }
    var arrayInfo = this._checkArray(true);
    if (arrayInfo) {
        arrayInfo.delete(this.data);
    } else {
        delete this.data[this.parent];
    }
}
```
- example usage
```shell
...
} catch(error) {
//The error will tell you where the DataPath stopped. In this case test1
//Since /test1/test does't exist.
    console.error(error);
}

//Deleting data
db.delete("/test1");

//Save the data (useful if you disable the saveOnPush)
db.save();

//In case you have a exterior change to the databse file and want to reload it
//use this method
db.reload();
...
```

#### <a name="apidoc.element.node-json-db.DBParentData.prototype.getData"></a>[function <span class="apidocSignatureSpan">node-json-db.DBParentData.prototype.</span>getData ()](#apidoc.element.node-json-db.DBParentData.prototype.getData)
- description and source-code
```javascript
getData = function () {
    if (this.parent === undefined) {
        return this.data;
    }
    var arrayInfo = this._checkArray();
    if (arrayInfo) {
        return arrayInfo.getData(this.data);
    } else {
        return this.data[this.parent];
    }
}
```
- example usage
```shell
...
*/
//You can't merge primitive.
//If you do this:
db.push("/test2/my/test/",10,false);
//the data will be overriden

//Get the data from the root
var data = db.getData("/");

//From a particular DataPath
var data = db.getData("/test1");

//If you try to get some data from a DataPath that doesn't exists
//You'll get an Error
try {
...
```

#### <a name="apidoc.element.node-json-db.DBParentData.prototype.setData"></a>[function <span class="apidocSignatureSpan">node-json-db.DBParentData.prototype.</span>setData (toSet)](#apidoc.element.node-json-db.DBParentData.prototype.setData)
- description and source-code
```javascript
setData = function (toSet) {
    if (this.parent === undefined) {
        this.db.data = toSet;
        return;
    }
    var arrayInfo = JsonUtils.processArray(this.parent);
    if (arrayInfo) {
        if (!this.data.hasOwnProperty(arrayInfo.property)) {
            this.data[arrayInfo.property] = [];
        } else if (!Array.isArray(this.data[arrayInfo.property])) {
            throw new DataError("DataPath: /" + this.dataPath + ". " + arrayInfo.property + " is not an array.", 11);
        }
        arrayInfo.setData(this.data, toSet);
    } else {
        this.data[this.parent] = toSet;
    }
}
```
- example usage
```shell
...
    var arrayInfo = JsonUtils.processArray(this.parent);
    if (arrayInfo) {
        if (!this.data.hasOwnProperty(arrayInfo.property)) {
            this.data[arrayInfo.property] = [];
        } else if (!Array.isArray(this.data[arrayInfo.property])) {
            throw new DataError("DataPath: /" + this.dataPath + ". " + arrayInfo.property + " is not an array.", 11);
        }
        arrayInfo.setData(this.data, toSet);
    } else {
        this.data[this.parent] = toSet;
    }
};

DBParentData.prototype.delete = function () {
    if (this.parent === undefined) {
...
```



# <a name="apidoc.module.node-json-db.Errors"></a>[module node-json-db.Errors](#apidoc.module.node-json-db.Errors)

#### <a name="apidoc.element.node-json-db.Errors.DataError"></a>[function <span class="apidocSignatureSpan">node-json-db.Errors.</span>DataError (msg, id, nested)](#apidoc.element.node-json-db.Errors.DataError)
- description and source-code
```javascript
function DataError(msg, id, nested) {
    var error = NestedError.call(this, msg, id, nested);
    error.name = 'DataError';
    return error;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-json-db.Errors.DatabaseError"></a>[function <span class="apidocSignatureSpan">node-json-db.Errors.</span>DatabaseError (msg, id, nested)](#apidoc.element.node-json-db.Errors.DatabaseError)
- description and source-code
```javascript
function DatabaseError(msg, id, nested) {
    var error = NestedError.call(this, msg, id, nested);
    error.name = 'DatabaseError';
    return error;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-json-db.utils"></a>[module node-json-db.utils](#apidoc.module.node-json-db.utils)

#### <a name="apidoc.element.node-json-db.utils.mergeObject"></a>[function <span class="apidocSignatureSpan">node-json-db.utils.</span>mergeObject ()](#apidoc.element.node-json-db.utils.mergeObject)
- description and source-code
```javascript
mergeObject = function () {
    var destination = {},
        sources = [].slice.call(arguments, 0);
    sources.forEach(function (source) {
        var prop;
        for (prop in source) {

            if (prop in destination && destination[prop] === null) {
                destination[prop] = source[prop];
            }
            else if (prop in destination && Array.isArray(destination[prop])) {

                // Concat Arrays
                destination[prop] = destination[prop].concat(source[prop]);

            } else if (prop in destination && typeof destination[prop] === "object") {

                // Merge Objects
                destination[prop] = merge(destination[prop], source[prop]);

            } else {

                // Set new values
                destination[prop] = source[prop];

            }
        }
    });
    return destination;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-json-db.utils.processArray"></a>[function <span class="apidocSignatureSpan">node-json-db.utils.</span>processArray (property)](#apidoc.element.node-json-db.utils.processArray)
- description and source-code
```javascript
processArray = function (property) {
    var match = arrayIndexRegex.exec(property);
    if (match != null) {
        return new ArrayInfo(match[1], match[2]);
    }
    return null;
}
```
- example usage
```shell
...
 * @returns {ArrayInfo}
 * @private
 */
DBParentData.prototype._checkArray = function (deletion) {
    if(typeof deletion === undefined) {
        deletion = false;
    }
    var arrayInfo = JsonUtils.processArray(this.parent);
    if (arrayInfo) {
        if ((!arrayInfo.append || deletion) && !arrayInfo.isValid(this.data)) {
            throw new DataError("DataPath: /" + this.dataPath + ". Can't find index " + arrayInfo.index + " in array " + arrayInfo
.property, 10);
        }
    }
    return arrayInfo;
};
...
```

#### <a name="apidoc.element.node-json-db.utils.removeTrailingSlash"></a>[function <span class="apidocSignatureSpan">node-json-db.utils.</span>removeTrailingSlash (dataPath)](#apidoc.element.node-json-db.utils.removeTrailingSlash)
- description and source-code
```javascript
function removeTrailingSlash(dataPath) {
    if(dataPath.length > 1 && endsWith(dataPath,"/")) {
        return dataPath.substring(0, dataPath.length - 1);
    }
    return dataPath;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-json-db.utils.strEndWith"></a>[function <span class="apidocSignatureSpan">node-json-db.utils.</span>strEndWith (str, suffix)](#apidoc.element.node-json-db.utils.strEndWith)
- description and source-code
```javascript
strEndWith = function (str, suffix) {
    return str.indexOf(suffix, str.length - suffix.length) !== -1;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
