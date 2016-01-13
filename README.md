# Project Setup

## Objectives

- Download the latest version of Angular 1.x
- Setup the directory structure for your Angular application
 
## Instructions

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

You can find `angular.js` in this repo - make sure you put it into the `js/` folder!

Let's create some files so we can have something pretty displayed in browser. No need to worry with what this code does yet, we will be covering it all very shortly!

### app.js

Inside the `js/app/` folder, create a new file called `app.js`. This file is very simple - it tells Angular that we want to create a new module. We can then reference that module later on.

Put this inside `app.js`:

```js
angular
  .module('app', []);
```

### MainController.js

Next, go to `js/app/controllers`. Make a new file called `MainController.js` and put this inside of it:

```js
function MainController($scope) {
  $scope.name = 'PUT YOUR NAME HERE!';
}
```

Here we've defined the main controller for our app. No need to worry about the specifics just yet, we are going to look at Controllers in depth very soon.

Next, we need to tell Angular about our controller. Add this to the bottom of `MainController.js`:

```js
angular
  .module('app')
  .controller('MainController', MainController);
```

### Hello, your name!

Now open up index.html in Google Chrome and you should see `Hello, your name`! Wow - our first small Angular application. 

Have a play around with `MainController.js` and see what else you can do!
