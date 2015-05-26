# Artist Seach Engine

[Live Demo](http://artist-search-engine.herokuapp.com)

### Introduction

Artist Search Engine is a **web application** that provides a convenient user interface for searching and accessing artists' profiles. 
This is first web application using **AngularJs**. I built the website in my free time right after the midterm of my sophomore year.

### Features

* Single page web application.
* Friendly and fast user interface.
* Enhanced animation by utilizing angular-animate library.

### Libraries

* angular.js
* angular-route.js
* angular-animate.js

### App Structure

#### home.html and index.php

The entire single page will be loaded by `home.html`, `index.php` is created for hosting the project on Heroku.
#### /css

Contain stylesheets for the page.

#### /images

Contain some mock images for artists to be used for testing the page.

#### /partials

Contain the main templates that will be rendered inside home.html without reloading the entire page. The templates include:
* `list.html` - Contains a search box with options search by name or search by reknown, arrange in ascending or descending orders. The box will populate the list of artists and nicely display match results below the search box. Clicking on match artist will lead to the detail page of that artist.
* `details.html` - Contains information about the match artist.

#### /js

* `app.js` - Contains the main model `myApp` for the entire web app. It also configures routes and associated views and controllers.
* `controllers.js` - Contains the main module `artistControllers` that will be used in `app.js`. This module consists of two controllers: `ListController` - populate the mock list of artists, and `DetailsController` - handle information page for match artists when the user clicks.


