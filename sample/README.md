# Sample MERN app structure

```yml
- client
    - main.js
- server
    - devBundle.js
    - server.js
- dist
- package.json
- nodemon.json
- .babelrc
- webpack.config.client.js
- webpack.config.client.production.js
- webpack.config.server.js
```

## Yarn

- package manager

## Express

- used as backend

```bash
yarn add express
```

## React

- used for frontend

```bash
yarn add react
yarn add react-dom
```

## Babel

- to convert `ES6` and `JSX` to suitable javascript for all browsers
- `@babel/core` `babel-loader` - for transpiling javascript with webpack
- `@babel/preset-env` - support for latest javascript feaetures
- `@babel/preset-react` - support for latest react features


## Webpack

- module bundler
- `webpack`
- `webpack-cli` to run webpack commands
- `webpack-node-externals` - for ignoring external node modues
- `webpack-dev-middleware` - to serve file emitted during development
- `webpack-hot-middleware` - to add hot module reloading into an existing server by connecting 
  a browser client to a Webpack server and receiving updates as code changes during development.

## Live reloading

- `nodemon` - to watch server-side changes during development, so the server can be reloaded to put changes into effect.

### Hot Reloading

- `react-hot-loader` - for faster development on the client side.
    - Every time a file changes in the React frontend, `react-hot-loader` enables the browser app to update without re-bundling the whole frontend code.
- `@hot-loader/react-dom` to enable hot-reloading support for **React hooks**. 
    - It essentially replaces the react-dom package of the same version, but with additional patches to support hot reloading.
