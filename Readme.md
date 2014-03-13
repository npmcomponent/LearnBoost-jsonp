*This repository is a mirror of the [component](http://component.io) module [learnboost/jsonp](http://github.com/learnboost/jsonp). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/learnboost-jsonp`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# jsonp

A simple JSONP implementation.

## Installation

Install for node.js or browserify using `npm`:

``` bash
$ npm install jsonp
```

Install for component(1) using `component`:

``` bash
$ component install LearnBoost/jsonp
```

## API

### jsonp(url, opts, fn)

- `url` (`String`) url to fetch
- `opts` (`Object`), optional
  - `param` (`String`) name of the query string parameter to specify
    the callback (defaults to `callback`)
  - `timeout` (`Number`) how long after a timeout error is emitted. `0` to
    disable (defaults to `60000`)
- `fn` callback

The callback is called with `err, data` parameters. 

If it times out, the `err` will be an `Error` object whose `message` is
`Timeout`.

## License

MIT
