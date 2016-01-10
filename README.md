# Project Setup

## Objectives

- Download the latest version of Angular 1.x
- Setup the directory structure for your Angular application
 
## Instructions

Go to the [Angular website](https://angularjs.org/) and download the latest version.

Setup your directory structure. From the root directory, the structure should be as follows (you can find the index.html in this repo) -

- js/
  - app/
    - directives/
    - controllers/
    - services/
    - templates/
      - partials/
      - views/
  - angular.js
- img/
- css/
- index.html

Make sure you put the Angular code you downloaded into the `js/` folder!

Let's create some files so we can have something pretty displayed in browser. No need to worry with what this code does yet, we will be covering it all very shortly!

### app.js

Inside the `js/app/` folder, create a new file called `app.js`. This file is very simple, and again - no need to worry about what it does just yet!

Put this inside `app.js`.
```js
angular
  .module('app', []);
```

### MainController.js

Next, go to `js/app/controllers`. Make a new file called `MainController.js` and put this inside of it -

```js
function MainController($scope) {
  $scope.name = 'PUT YOUR NAME HERE!';
}

angular
  .module('app')
  .controller('MainController', MainController);
```

### Hello, your name!

Now open up index.html and you should see `Hello, your name`! Wow - our first small Angular application. 

Have a play around with `MainController.js` and see what else you can do!