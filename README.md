# myproject

#### 07/20/2018
Recently (2 days ago) I realized that while I use webpack quite often, I do not know how to configure it myself. So, in an attempt to make better use of webpack and its degree of granularity , I decided to learn about its core concepts and how to set it up from scratch.

This project is the product of my experimentation with various webpack's feature and highly customizable configurations.

Restructured directory structure.

#### 07/21/2018

Started setting up the infrastructure for a full stack, server side rendered application using Express on the back-end and React, along with React-Router, on the front-end.

Still figuring out how to bring all the pieces together to achieve expected behavior.

The script `npm run server` is currently using `concurrently` to simultaneously run express server (on PORT 300) and webpack-dev-server (on PORT 9000). Playing with `proxy` property of devServer in webpack configurations but haven't fully achieved expected behavior yet.

The goal is for the React Application to be served when the client reaches `/` (root) route, and for React-Router to handle any subsequent routing.

#### 07/22/2018

Added logic to connect to database. Nature of connection is based on value of `NODE_ENV`. For instance:

`NOVE_ENV=production` will open connection to DB in cloud (via mLab). `NODE_ENV=development` will open connection to local MongoDB. If `NODE_ENV` is set to `"development"`, be sure to run the `mongod` command in your terminal before starting the server.

<!--  
### Info about directories and subdirectories

Directory structure
|   - ./server```
|- ./myproject (root)
|   - ./build-utils
|     - ./common-paths.js
|     - ./webpack.common.js
|     - ./webpack.dev.js
|     - ./webpack.prod.js
|   - ./client
|     - ./src
|       - ./components
|         - ./Layout
|           - ./footer
|             -  ./Nav.js
|           - ./header
|             -  ./Footer.js
|           - ./main
|           - ./Layout.js
|         - ./IndexPage.js
|         - ./NotFoundPage.js
|       - ./routing
|         - ./history.js
|         - ./routes.js
|       - ./styles
|         - ./index.css
|         - ./index.scss
|       - ./App.js
|       - ./index.html
|       - ./index.js
|   - ./node_modules
|   - ./server
|     - ./server.js
|   - ./.babelrc
|   - ./gitignore
|   - ./package-lock.json
|   - ./package.json
|   - ./README.md
|   - ./webpack.config.json
|-
```
-->

<hr >

## dependencies to install

- react
- react-dom
- express
- react-router-dom
- history
- bulma
- mongoose

## dev dependencies to install

- webpack
- webpack-cli
- webpack-dev-server
- webpack-merge
- chalk
- morgan
- nodemon

## loaders and plugins to install

- babel-loader
- babel-core
- babel-preset-es2015
- babel-preset-react
- style-loader
- css-loader
- sass-loader
- node-sass
- url-loader
- file-loader
- compression-webpack-plugin
- extract-text-webpack-plugin
- html-webpack-plugin
- uglifyjs-webpack-plugin
