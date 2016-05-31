# aem-slang
==============

## Install

```shell
    npm install aem-slang --save-dev
```

## Example
```js
var slang = require('aem-slang');

slang.setOptions({
    port: 4503,
    host: 'localhost'
});

slang.up('file.js').then(function(status) {
    // any action for after successful upload
}).catch(function(err) {
    // handle error
});
```

## Options
If `#setOptions` is not called before `#up`, it falls back to defaults
### host
Type: `string`
Default: `localhost`

hostname to running sling instance.
### port
Type: `number`
Default: `4502`

Port for running sling instance.
### username
Type: `string`
Default: `admin`

Username for authentication.
### password
Type: `string`
Default: `admin`

Password for authentication.

## Development
Clone this repo, then `npm install`

after any changes, run `npm run build` to compile
