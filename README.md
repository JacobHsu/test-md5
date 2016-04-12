# test-md5
[![Build Status](https://travis-ci.org/JacobHsu/test-md5.svg?branch=master)](https://travis-ci.org/JacobHsu/test-md5)

# NPMs
[![NPM](https://nodei.co/npm/js-md5.png?stars&downloads)](https://nodei.co/npm/js-md5/)  

A simple MD5 hash function for JavaScript supports UTF-8 encoding.

# Installation
`npm init`  
`npm install js-md5 mocha expect.js --save`

# Usage

```js
md5('Message to hash');
var hash = md5.create();
hash.update('Message to hash');
hash.hex();
```

`$ node index`

# Tests

test-md5\tests  
`$ mocha node-test`

or

package.json
```
"scripts": {
  "test": "mocha tests/node-test.js"
}
```
`$ npm test`

# Example
`md5(''); // d41d8cd98f00b204e9800998ecf8427e`  
// It also supports UTF-8 encoding  
`md5('中文'); // a7bac2239fcdcb3a067903d8077c4a07`

# References

* https://github.com/emn178/js-md5
* [使用mocha在node.js和瀏覽器環境中單元測試](http://emn178.pixnet.net/blog/post/108745297)
* https://travis-ci.org/
* [在Github上使用Travis CI進行持續整合 - Node.js](http://emn178.pixnet.net/blog/post/108785425)
