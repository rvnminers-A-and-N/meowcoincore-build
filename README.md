# meowcoincore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install meowcoincore-build
```

and use and require in your gulp file:

```javascript
var gulp = require('gulp');
var meowcoincoreTasks = require('meowcoincore-build');

meowcoincoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var meowcoincoreTasks = require('meowcoincore-build');
meowcoincoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/rvnminers-A-and-N/meowcoincore) on the main meowcoincore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/rvnminers-A-and-N/meowcoincore/blob/master/LICENSE).

