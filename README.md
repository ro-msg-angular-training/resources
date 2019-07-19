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
 - [5. Forms and Validation](#5-forms-and-validation)
 - [6. Authorization and Guards](#6-authorization-and-guards)
 - [OPT-1. Material Components](#opt-1-use-material-components)
 - [OPT-2. Internationalization](#opt-2-internationalization)

## Working Mode

The road-map consists of several steps. In each step, a set of theoretical concepts are explored, supported by reference documentation, book chapters, tutorials and videos. In parallel, a simple application will be built with the learned concepts: the *Online Shop* application.

After the learning material for a given step was sufficiently explored, either some new functionality will be added to this application or old functionality will be refactored.

All the code written must be published on GitHub. Access the [this link](https://classroom.github.com/a/Ch8FVRTf) to create your own repository. Commits must be pushed when each individual chapter is finished. In order to request a code review from the trainers, you must [open a pull request](https://help.github.com/en/articles/creating-a-pull-request) from the `develop` to the `master` branch.

## Environment

You can work using your local environment:
 - You need to install [NodeJS](https://nodejs.org/en/) and [VSCode](https://code.visualstudio.com/download).

In the `backend` folder you can find a server-side implementation for the online shop. Tu run this server perform the following:
 - Open the `backend` folder in your terminal
 - `npm ci` (only needed the first time your run the server)
 - `npm start`
 - Open [http://localhost:3000](http://localhost:3000) in your browser.

## Online Shop
The application will simply browse through a catalog of products. It will support:

 - Listing the products,
 - Adding a new product,
 - Updating an existing product,
 - Deleting a product.
 
The online shop has a "shopping cart" functionality:
 - The user may add items into the cart,
 - He may increment and decrement the quantity of each product or even remove a product completely from the cart,
 - Lastly, he may checkout the cart and place an order (resulting in the creation of an order in the backend).

Mockups describing the user interface structure can be found in the [mockups](./mockups/mockups.pdf) folder.
These mockups should be used as a guideline, but improvements or deviations from them is allowed. 

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
 > From the detail page of the product, the user may add it to his shopping cart (by pressing a button).
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

 > Use HttpClient to read the products from the backend to fill in the product list. 
 > 
 > When navigating to the product detail page, read the product information from the backend.
 >
 > Add a new "Delete" button on the detail page, which calls the backend to remove a product from the catalogue.
 >
 > Add a new "Checkout" button on the shopping cart page, which creates a new order on the backend.

Further Resources:

 - [CORS: Proxy-ing a backend server](https://angular.io/guide/build#proxying-to-a-backend-server)
 - [Http error handling](https://angular.io/guide/http#error-handling)
 
## 5. Forms and Validation

Goal: dive into Angular Forms and add them to your project.

Required Reading:

 - [Forms overview](https://angular.io/guide/forms-overview)
 - [Forms tutorial](https://www.tutorialspoint.com/angular6/angular6_forms.htm)

Online Shop:

 > Add a new "Edit" button on the detail page. Pressing it should open a new view, which uses reactive forms to update the properties of the product. The view should have two buttons: "Cancel" (which undos all the changes) and "Save" (which calls the backend to persist the changes).
 >
 > Add some validation to your form (ex: check that the fields are not empty, that the price and weight inputs contain only numbers, etc.)
 >
 > Also create a new "Add" button on the product list. Pressing this button should open a view for creating a new product (which the same structure and buttons as the edit view).

Further Resources:

 - [Custom form controls](https://blog.thoughtram.io/angular/2016/07/27/custom-form-controls-in-angular-2.html)

## 6. Authorization and Guards

Goal: get familiar with Route Guards and protect your app's routes from unauthorized access.

Required Reading:

 - [Route Guards](https://angular.io/guide/router#milestone-5-route-guards)

Online Shop:

 > Create a new login view, containing a text input for the username, a password input for the password and a login button.
 >
 > Automatically redirect the user to the login view each time he opens or refreshes the application. When pressing the login button, send an appropriate request to the backend. If the request succeeds, redirect the user to the product page, otherwise display an error message.
 >
 > Use the roles returned by the backend to disable the edit, create and delete buttons if the user is not an administrator. Only allow customers to view the shopping cart and to add products in it.

Further Resources:

 - [Angular Role-based Authorization](https://jasonwatmore.com/post/2018/11/22/angular-7-role-based-authorization-tutorial-with-example)

## OPT-1. Use Material Components

Required Reading:

 - [Material - Introduction](https://material.io/design/introduction/)

Online Shop:

> Install and use [Material Design](https://material.angular.io/guide/getting-started) in your Online Shop app. Replace your "plain" HTML components with [Material Components](https://material.angular.io/components/categories).

## OPT-2. Internationalization

Goal: Translate the user interface in multiple languages.

Required Reading:

 - [Angular: i18n](https://angular.io/guide/i18n)

Online Shop:

 > Translate all the labels, headings, titles and buttons of our shop in English and Romanian.

Further Resources:

 - [How to use Internationalization (i18n) in Angular](https://alligator.io/angular/internationalization/)

## OPT-3. Simple NGRX

Goal: Use NGRX for state management.

Required Reading:

 - [Angular: NGRX a clean and clear Introduction](https://medium.com/frontend-fun/angular-ngrx-a-clean-and-clear-introduction-4ed61c89c1fc)
 - [Getting started with NGRX](https://ngrx.io/guide/store)

Online Shop:

 > Add NGRX to your app by:
 >  - Creating a reducer for each page,
 >  - Adding actions for each user input handler, data load event, etc.
 >  - Adding effects to react on the data loading actions and call the services,
 >  - Dispatching the actions and selecting the state **only** inside the smart components.
 >
 > Hints:
 >  - Make sure to also have a loading flag indicator in each page's state,
 >  - Use the async pipe inside the smart components to not pass `Observable`s to dumb components,
 >  - Install the [Redux DevTools](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en) Chrome plugin to be able to debug your store.

Further Resources:
 - [NGRX Tips and Tricks](https://blog.angularindepth.com/ngrx-tips-tricks-69feb20a42a7)
 - [NGRX Docs](https://ngrx.io/docs)

## OPT-4. Normalized NGRX

*Prerequisite: OPT-3. Simple NGRX*

Goal: Normalize the NGRX state.

Required Reading:
 - [Normalizing State Shape](https://redux.js.org/recipes/structuring-reducers/normalizing-state-shape)
 - [The benefits of application state normalization in Angular](https://blog.angularindepth.com/the-benefits-of-application-state-normalization-in-angular-f93392ca9f44)

Online Shop:

 > Split your application state into two parts:
 >  - `data`: The portion which will hold the normalized data collections,
 >  - `ui`: The portion which will hold the sub-states used in the app pages.
 >
 > Inside the `data` sub-tree, you should have a `products` map (between ID and the entity itself).
 > For each product, you should also store an indicator if the product is fully loaded or just the header is loaded.
 > You should only make a call to the backend if it is really necessary (if the entity / entity set is not loaded).
 >
 > Inside the `ui` sub-tree, you should never copy product data, just have the IDs to reference the corresponding 
 > entry from the `data` sub-tree.
 >
 > You should define selectors to denormalize the data back to what you need in your pages.
