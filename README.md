# React Starter

A React starter boilerplate I created as a base for my React apps.

**Features:**

* React with router
* Redux with React router, selectors and Sagas
* Server-side rendering (Universal Javascript)
* Complete ES6 with some ES7 goodies
* Hot-reloading

Mind that this starter is quite opinionated - I primarily created it for myself, however, any suggestions and pull requests ale wholeheartly welcome.

### TODO:

* Tests
* I18n
* favicon
* image loaders

### Tasks

Simply `npm i`. Then you have these following tasks available:

* `npm start` - run when you want to develop
* `npm run build` - builds assets for production
* `npm run build:beta` - bu ilds assets for beta
* `npm run server` - runs the server for production (note: no static asset serving)
* `npm run server:beta` - runs the server for beta
* `npm run lint` - runs eslint
* `npm run lint:fix` - runs eslint and fixes problems, if it can

### Philosophy

Compilation is done by **Webpack**, however I tried to keep it as barebones as possible - no special Webpack stuff scattered in the source files. Thus I omitted any importing of any other files other than `.js` and `.jsx` to the main bundle or anything that would make me having to stick to Webpack forever and ever.

The only thing I couldn't pass on was hot-reloading, though. That is way too awesome to miss.

### WARNING:

Keep in mind that I'm using Webpack's built-in hot module reloading. There is neither `react-hot-loader`, nor `react-transform` taking place. This is because I keep all of my state in **Redux**.

If you'd like to keep your state in your application, feel free to include one of the implementations. However, keeping state in Redux has many benefits, I highly recommend this approach.
