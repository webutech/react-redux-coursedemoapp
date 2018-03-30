# react-redux-coursedemoapp
Author :  Pankaj Sharma
## Guide

* [package.json configuration](#package.json-configuration)
* [webpack setup](#webpack-setup)
* [setup editorconfig](#setup-editorconfig)
* [setup babel](#setup-babel)
* [setup express](#setup-express)
* [create start script](#create-start-script)
* [create start message](#create-start-message)



## package.json configuration
- Create package.json file in the root folder.
- Open package.json file from this repository,copy and paste the code in your file.
- Remove the script entry

## webpack setup
webpack is a static module bundler for modern JavaScript applications. When webpack processes your application, it recursively builds a dependency graph that includes every module your application needs, then packages all of those modules into one or more bundles.

- Taken the reference from *[webpack ref] (https://webpack.js.org/)
- Create a file in root of your application (react-redux-coursedemoapp/webpack.config.dev.js)
- Copy and paste the code from webpack.config.dev.js file in your file

## setup editorconfig
- Create (.editorconfig) file in the root of your application
- The code in this file is used to configure the indentation, spacing of the code in the application
- In this file we create rule for the editor.
- Copy and paste the code from the respective file.

## setup babel
- Create (.babelrc) file in the root of your application
- Copy and paste the code from the respective file

## setup express
- Create (tools) folder in the root of your application
- Copy and paste the code from the respective file.
- Taken the reference from *[express ref] (https://expressjs.com/)

## create start script
- add below code in the script property in the package.json file
```
"scripts": {
  "start":"babel-node tools/srcServer.js"
 }
```
now run the [npm start] command on the terminal window

## create start message
- Here we will be configuring start message that will be displayed when you will run your application.
- create (startMessage.js) file in the tools folder and copy and paste the code from the respective folder.
- add the prestart entry in the scripts section of package.json file
```
"scripts": {
  "prestart":"babel-node tools/startMessage.js",
  "start":"babel-node tools/srcServer.js"
 }
```
- now run the application and check the browser.
