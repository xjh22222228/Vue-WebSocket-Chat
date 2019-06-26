# egg-crypto

[crypto-js](https://github.com/brix/crypto-js) plugin for Egg.js.

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Test coverage][codecov-image]][codecov-url]
[![David deps][david-image]][david-url]
[![Known Vulnerabilities][snyk-image]][snyk-url]
[![npm download][download-image]][download-url]

[npm-image]: https://img.shields.io/npm/v/egg-crypto.svg?style=flat-square
[npm-url]: https://npmjs.org/package/egg-crypto
[travis-image]: https://img.shields.io/travis/eggjs/egg-crypto.svg?style=flat-square
[travis-url]: https://travis-ci.org/eggjs/egg-crypto
[codecov-image]: https://img.shields.io/codecov/c/github/eggjs/egg-crypto.svg?style=flat-square
[codecov-url]: https://codecov.io/github/eggjs/egg-crypto?branch=master
[david-image]: https://img.shields.io/david/eggjs/egg-crypto.svg?style=flat-square
[david-url]: https://david-dm.org/eggjs/egg-crypto
[snyk-image]: https://snyk.io/test/npm/egg-crypto/badge.svg?style=flat-square
[snyk-url]: https://snyk.io/test/npm/egg-crypto
[download-image]: https://img.shields.io/npm/dm/egg-crypto.svg?style=flat-square
[download-url]: https://npmjs.org/package/egg-crypto


[README](README.md) | [中文文档](README.zh_CN.md)


## Install

```bash
$ npm i egg-crypto --save
```

## Usage

```js
// {app_root}/config/plugin.js
exports.mailer = {
  enable: true,
  package: 'egg-crypto',
};
```

## Example

```js
// app/controller/home.js

'use strict';

const Controller = require('egg').Controller;

class HomeController extends Controller {
  async index() {
    this.ctx.body = this.ctx.crypto.MD5('Hi, egg-crypto');
  }
}

module.exports = HomeController;
```

## List

- ```md5```
- ```sha1```
- ```sha256```
- ```sha224```
- ```sha512```
- ```sha384```
- ```sha3```
- ```ripemd160```

---

- ```hmac-md5```
- ```hmac-sha1```
- ```hmac-sha256```
- ```hmac-sha224```
- ```hmac-sha512```
- ```hmac-sha384```
- ```hmac-sha3```
- ```hmac-ripemd160```

---

- ```pbkdf2```

---

- ```aes```
- ```tripledes```
- ```rc4```
- ```rabbit```
- ```rabbit-legacy```
- ```evpkdf```

---

- ```format-openssl```
- ```format-hex```

---

- ```enc-latin1```
- ```enc-utf8```
- ```enc-hex```
- ```enc-utf16```
- ```enc-base64```

---

- ```mode-cfb```
- ```mode-ctr```
- ```mode-ctr-gladman```
- ```mode-ofb```
- ```mode-ecb```

---

- ```pad-pkcs7```
- ```pad-ansix923```
- ```pad-iso10126```
- ```pad-iso97971```
- ```pad-zeropadding```
- ```pad-nopadding```



## Questions & Suggestions

Please open an issue [here](https://github.com/eggjs/egg/issues).

## License

[MIT](LICENSE)
