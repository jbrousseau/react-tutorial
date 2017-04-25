# React-tutorial 

A react tutorial from scratch, with React+React Router+Relay+Webpack+Babel, step by step

## Step 1 - start project

### create directories and init
```bash
mkdir react-tutorial
cd react-tutorial
mkdir src
mkdir dist
touch src/app.js
npm init
```
Then answer the prompt questions
It creates a package.json on root directory.

### install javascript librairies
After, install React library

```bash
npm install --save react
npm install --save react-dom
```

### edit source code
And edit src/app.js (see git)


### install webpack
```bash
npm install webpack --save-dev 
npm install html-webpack-plugin --save-dev
```

And add to package.json
```json
"scripts": {
    "build": "webpack src/app.js dist/bundle.js --color -p --progress --config internals/webpack/webpack.prod.babel.js",
}
```

### install babel
```bash
touch .babelrc
```
fill with (see git)
and 
```bash
npm install babel-loader babel-preset-latest babel-preset-react babel-preset-stage-0 --save-dev  
```
### run it

#### build

```bash
npm run build
```


#### install a simple http-server

```bash
npm install http-server -g
http-server dist/bundle.js
```

## Step 2 - Add test

```bash
npm install jest --save-dev 
```