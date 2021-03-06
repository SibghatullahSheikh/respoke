# Respoke.js

Browser/Client Library for [Respoke](https://www.respoke.io). Use this library in a JavaScript web app to add individual and group messaging, contact discovery, and voice and video calling to web apps. If you want to *use* this library in your app, you probably want to reference it via [this link on our CDN](https://cdn.respoke.io/respoke.min.js).

## Documentation

The documentation for this library resides [on the Respoke website](https://docs.respoke.io/js-library/respoke.html). Also check out the [quickstart guide](https://docs.respoke.io/) and other tutorials.

## Development Dependencies

We welcome [discussion on our community](http://community.respoke.io/) and contributions from the community. To get started contributing back, you'll need to clone this repo and run the following commands.

```
brew install node
# or
# apt-get install nodejs
npm install -g grunt
npm install
```

## Tests

Tests currently cannot run outside of our internal development infrastructure.

### Compilation
Transporter uses CommonJS to manage its dependencies, and the [Webpack](http://webpack.github.io/) module bundler to bundle the library. To create the bundled and minified library suitable for distribution, you can run

```
grunt dist
```

or

```
webpack && npm run build-stats
```

If you want to have the source files watched and built automatically when changes are made, run

```
webpack --watch
```

If you want the watch task to rebuild faster, you can comment out the uglify plugin in `webpack.config.js` for the duration of your development.

### Code Compliance

This project uses jshint.  The configuration for jshint can be found in the repo at `.jshintrc` and `.jshintignore`.

```
jshint respoke/*.js
```

# License

Respoke.js is licensed under the [MIT license](LICENSE).
