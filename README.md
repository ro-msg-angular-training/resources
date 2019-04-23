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

## 4. Services using HttpClient
