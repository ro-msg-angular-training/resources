# Angular Training: Resources

## Contents

 - [Working Mode](#working-mode)
 - [Environment](#environment)
 - [Online Shop](#online-shop)
 - [0. HTML and CSS Basics](#0-html-and-css-basics)
 - [1. Angular Intro](#1-angular-intro)
 - [2. Components](#2-components)
 - [3. Routing](#3-routing)
 - [4. Services using HttpClient](#4-services-using-httpclient)

## Working Mode

The road-map consists of several steps. In each step, a set of theoretical concepts are explored, supported by reference documentation, book chapters, tutorials and videos. In parallel, a simple application will be built with the learned concepts: the *Online Shop* application.

After the learning material for a given step was sufficiently explored, either some new functionality will be added to this application or old functionality will be refactored.

All the code written must be published on GitHub. Access the [this link](https://classroom.github.com/a/Ch8FVRTf) to create your own repository. Commits must be pushed when each individual chapter is finished. In order to request a code review from the trainers, you must [open a pull request](https://help.github.com/en/articles/creating-a-pull-request) from the `develop` to the `master` branch.

## Environment

You can work using your local environment:
 - You need to install [NodeJS](https://nodejs.org/en/) and [VSCode](https://code.visualstudio.com/download).

## Online Shop
The application will simply browse through a catalog of products. It will support:

 - Listing the products,
 - Adding a new product,
 - Updating an existing product,
 - Deleting a product.

## 0. HTML and CSS Basics

Goal: refresh your knowledge about HTML and CSS basic concepts.

Required Reading:

 - [HTML Beginner Guide](https://www.htmldog.com/guides/html/beginner/)
 - [CSS Beginner Guide](https://www.htmldog.com/guides/css/beginner/)

Online Shop: *nothing to do*.

Further Resources:

 - [HTML and CSS Reference](https://www.htmldog.com/references/)
 - [CSS Media Queries](https://www.htmldog.com/guides/css/advanced/mediaqueries/)
 - [W3's Intro Tutorial](https://www.w3.org/Style/Examples/011/firstcss.en.html)

## 1. Angular Intro

Goal: become familiar with Angular.

Required Reading:

 - [Single vs Multiple Page Applications](https://medium.com/@NeotericEU/single-page-application-vs-multiple-page-application-2591588efe58)
 - [TypeScript in 5 minutes](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)
 - [Angular Quick Start](https://angular.io/guide/quickstart)

Online Shop:

 > Install the *Angular CLI* with the help of the NodeJS package manager: `npm install -g @angular/cli`.
 > 
 > Create a new project in the root of your git repository by using the CLI: `ng new online-shop`.
 > 
 > Navigate inside the project folder, Start the project and open its home page in your browser: `ng serve --start`.

Further Resources:

 - [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/basic-types.html)
 - [Difference between AngularJS and Angular 2 / 4](https://www.simplilearn.com/angularjs-vs-angular-2-vs-angular-4-differences-article)

## 2. Components

Goal: get a grip on the basics of Angular Components

Required Reading:

- [Introduction to components](https://angular.io/guide/architecture-components)
- [Angular Components tutorial](https://www.tutorialspoint.com/angular6/angular6_components.htm)

Online Shop:

For the moment, we will use mock data across all components. The data will be defined locally in the Typescript file associated to a component.

 > Create a new Angular Component for displaying a single product's details. You can use the CLI command `ng generate component <component-name>` to achieve this.
 >
 > Create an Angular component for displaying a list of products. Hint: use the `*ngFor` directive.
 >
 > Add some CSS to each of the components to make them look nicer.
 
 Further Resources:
 
 - [The `*ngFor` directive](https://angular.io/guide/displaying-data#showing-an-array-property-with-ngfor)
 - [Types of Bindings](https://angular.io/guide/template-syntax#binding-syntax-an-overview)
 - [Event Binding](https://angular.io/guide/template-syntax#event-binding-event)

## 3. Routing

Goal: understand the basics of Angular Routing and add routing to your project

Required Reading:

 - ["The Basics" chapter from Angular Routing official documentation](https://angular.io/guide/router#the-basics)
 - [Tour of Heroes Routing tutorial](https://angular.io/tutorial/toh-pt5)
 
 Online Shop:
 
 > Add a button next to each product from the product list. You can use it to navigate to a specific product's detail page.
 >
 > Add Routing to your project and implement a navigation between the list of all products and the product detail page. Use [`<router-outlet>`](https://angular.io/guide/router#router-outlet) as a placeholder for the currently displayed component in your app.
 > 
 > Add a navigation which redirects users from the default path ('/') to the '/products' page and displays by default the list of all products.
 >
 > Enhance your app with routing parameters, such that you can navigate to a specific product's detail page. Hint: Use [`snapshot`](https://angular.io/guide/router#snapshot-the-no-observable-alternative) to capture the product's ID as a navigation parameter and display it in the details page. 
 
 Further Resources:
 
  - [Routing with Observable](https://angular.io/guide/router#activated-route-in-action)
  - [Route guards: protecting your app's routes](https://angular.io/guide/router#milestone-5-route-guards)
 
## 4. Services using HttpClient

Goal: practice with Angular HttpClient by connecting your frontend with the backend server

Required Reading:

- [Quick start guide](https://blog.angular-university.io/angular-http/)
- [Angular Http tutrial](https://www.tutorialspoint.com/angular6/angular6_http_client.htm)
- [Official docs](https://angular.io/guide/http)

Online Shop:

 > Required for solving CORS errors: [Proxying a backend server](https://angular.io/guide/build#proxying-to-a-backend-server)
 >
 > Use HttpClient to perform GET requests and display the list of products and a single product's details.
 >
 > Implement a "Delete" functionality for removing products in the backend. 

Further Resources:

 - [Http error handling](https://angular.io/guide/http#error-handling)
 
## 5. Forms and Validation

Goal: dive into Angular Forms and add them to your project

Required Reading:

 - [Forms overview](https://angular.io/guide/forms-overview)
 - [Forms tutorial](https://www.tutorialspoint.com/angular6/angular6_forms.htm)

 > Add Forms to your project for updating a product's details. You can choose either the Template Driven (TD) or reactive / Model Driven  (MD) approach. 
 >
 > Add some validation to your form (ex: check that the fields are not empty, that the price and weight inputs contain only numbers, etc.)

## 6. Internationalization 

## 7. Authorization and Guards

## OPT-1. ngRX for State Management
