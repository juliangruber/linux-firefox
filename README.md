# linux-firefox

Launch a fresh Firefox on Linux.

## Example

```js
const firefox = require('linux-firefox')

firefox({ uri: 'https://github.com/' }, (err, ps) => {
  if (err) throw err    
  ps.on('error', console.error)
})
```

## Installation

```js
$ npm install linux-firefox
```

Firefox needs to be installed on your system as well.

## API

### firefox(opts, cb)

Options:

- `display`: Launch Firefox on `:${opts.display}`
- `proxy`: Proxy server settings
- `noProxy`: Proxy routes to skip

## License

MIT
