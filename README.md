# Stats plugin for webpack

Writes the stats of a build to a file.


## Installation

```sh
$ npm install --save stats-webpack-plugin
```


## Usage

```js
var StatsPlugin = require('stats-webpack-plugin');

module.exports = {
  plugins: [
    new StatsPlugin(path.join(__dirname, 'build', 'stats.json'), {
      chunkModules: true,
      exclude: [/node_modules[\\\/]react/]
    })
  ]
};
```


## API

```js
new StatsPlugin(filename: string, [options])
```

* `filename` the filename of the result file.
* `options` options passed to [stats.toJson](http://webpack.github.io/docs/node.js-api.html#stats-tojson)


## Meta

* Code: `git clone git://github.com/unindented/stats-webpack-plugin.git`
* Home: <https://github.com/unindented/stats-webpack-plugin/>


## Contributors

* Daniel Perez Alvarez ([unindented@gmail.com](mailto:unindented@gmail.com))


## License

Copyright (c) 2014 Daniel Perez Alvarez ([unindented.org](http://unindented.org/)). This is free software, and may be redistributed under the terms specified in the LICENSE file.