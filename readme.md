# @esm2cjs/escape-string-regexp

This is a fork of https://github.com/sindresorhus/escape-string-regexp, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i escape-string-regexp@npm:@esm2cjs/escape-string-regexp
```

```jsonc
// package.json
"dependencies": {
    "escape-string-regexp": "npm:@esm2cjs/escape-string-regexp"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/escape-string-regexp
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/escape-string-regexp": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import escapeStringRegexp from "@esm2cjs/escape-string-regexp";

// Using CommonJS require()
const escapeStringRegexp = require("@esm2cjs/escape-string-regexp").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/escape-string-regexp).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/escape-string-regexp).
