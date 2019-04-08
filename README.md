[![Build Status](https://travis-ci.org/kaelzhang/roe-plugin-env.svg?branch=master)](https://travis-ci.org/kaelzhang/roe-plugin-env)
[![Coverage](https://codecov.io/gh/kaelzhang/roe-plugin-env/branch/master/graph/badge.svg)](https://codecov.io/gh/kaelzhang/roe-plugin-env)
<!-- optional appveyor tst
[![Windows Build Status](https://ci.appveyor.com/api/projects/status/github/kaelzhang/roe-plugin-env?branch=master&svg=true)](https://ci.appveyor.com/project/kaelzhang/roe-plugin-env)
-->
<!-- optional npm version
[![NPM version](https://badge.fury.io/js/roe-plugin-env.svg)](http://badge.fury.io/js/roe-plugin-env)
-->
<!-- optional npm downloads
[![npm module downloads per month](http://img.shields.io/npm/dm/roe-plugin-env.svg)](https://www.npmjs.org/package/roe-plugin-env)
-->
<!-- optional dependency status
[![Dependency Status](https://david-dm.org/kaelzhang/roe-plugin-env.svg)](https://david-dm.org/kaelzhang/roe-plugin-env)
-->

# roe-plugin-env

[Roe](https://github.com/kaelzhang/roe) plugin to allow the sanbox to inherit extra environment variables from the current process

## Install

```sh
$ npm i roe-plugin-env
```

## Usage

```js
const EnvPlugin = require('roe-plugin-env')

module.exports = {
  plugins: [
    // Allow sandbox to inherit `process.env.REDIS_HOST` of the parent process.
    new EnvPlugin(['REDIS_HOST'])
  ]
}
```

## License

MIT
