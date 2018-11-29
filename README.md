![CF](http://i.imgur.com/7v5ASc8.png) LAB
=================================================

## Lab 31

### Author: Jen Carrigan

### Links and Resources
* [Assignment1](https://codesandbox.io/s/5y2zllkp0x)
* [Assignment2](https://codesandbox.io/s/rlqxw05pxq)

### Assignment 1
#### `index.js`
Imports React, ReactDOM, Provider from Redux, and our App component
Creates a store
Feeds that store into the component
Renders Main

### Store
#### `store/index.js`
Imports createStore, combineReducers, applyMiddleware from redux, as well as our logger, and our reducers
Combines the reducers into a state object with keys and functions as values.
exports the store with reducers and middleware

#### `reducer.js`
Sets initialState for foo
Exports state based on payload

#### `actions.js`
Exports object with type and payload

### Components
#### `app.js`
Imports React, connect from redux, and appActions from app-actions
Instantiates class App
* `render` renders markup based on click
Two separate functions
* `mapStateToProps` sets the objects key and its current state
* `mapDispatchToProps` maps the button clicks in the markup above to a dispatch for redux
Exports the App after connected to store

### Assignment 2
#### `index.js`
Imports React, ReactDOM, Provider from Redux, and our App and Num components
Creates a store
Feeds that store into the components
Renders Main

### Store
#### `store/index.js`
Imports createStore, combineReducers, applyMiddleware from redux, as well as our logger, and our reducers
Combines the reducers into a state object with keys and functions as values.
exports the store with reducers and middleware

#### `app-reducer.js`
Sets initialState for name
Exports state based on payload

#### `number-reducer.js`
Sets initialState for number
Exports state based on payload

#### `app-actions.js`
Exports object with type and payload

#### `number-actions.js`
Exports object with type and payload

### Components
#### `app.js`
Imports React, connect from redux, and appActions from app-actions
Instantiates class App
* `changeMyName` calls dispatch with random word from array
* `render` renders markup
Two separate functions
* `mapStateToProps` sets the objects key and its current state
* `mapDispatchToProps` maps the changeMyName method above to a dispatch for redux
Exports the App after connected to store

#### `number.js`
Imports React, connect from redux, and numActions from number-actions
Instantiates class Num
* `render` renders markup
Two separate functions
* `mapStateToProps` sets the objects key and its current state
* `mapDispatchToProps` maps calls in the render to a dispatch for redux
Exports the Num after connected to store

#### UML
![Assignment1](https://raw.githubusercontent.com/JenCarrigan/data-structures-and-algorithms/master/%3Aassets/Assignment1.jpg)
![Assignment2](https://raw.githubusercontent.com/JenCarrigan/data-structures-and-algorithms/master/%3Aassets/Assignment2.jpg)
