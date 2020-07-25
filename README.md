#2 Ways of setting up React

###Create React App

1. Set up development environment

```
npx create-react-app my-app
```

2. Run app in development mode

```
npm start
```

3. Production ready build

```
npm run build
```

###Set up React from scratch

1. `npm init`

2. Create `public`, `src` folder, `.gitignore` file and `index.html` file in `public` folder

3. Set up Babel

```
npm install --save-dev @babel/core@7.1.0 @babel/cli@7.1.0 @babel/preset-env@7.1.0 @babel/preset-react@7.0.0
```

Create `.babelrc` file:

```
{
  "presets": ["@babel/env", "@babel/preset-react"]
}
```

4. Set up Webpack

```
npm install --save-dev webpack@4.19.1 webpack-cli@3.1.1 webpack-dev-server@3.1.8 style-loader@0.23.0 css-loader@1.0.0 babel-loader@8.0.2
```

Create `webpack.config.js` file

5. Install React and React-DOM

```
npm install react
npm install react-dom
```

6. Create `index.js` and `App.js` file in `src` folder

7. Script to start dev server
   In package.json

```
"start": "webpack-dev-server --mode development"
```

8. Install `react-hot-loader`
   Import the loader to `App.js`

```
import {hot} from "react-hot-loader";

...

export default hot(module)(App);
```

9. Webpack build script

```
webpack --mode development
webpack --mode production
```
