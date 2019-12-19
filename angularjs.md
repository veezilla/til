# AnguluarJS

## Conceptual Overview

| Concept              | Description                                                  |
| -------------------- | ------------------------------------------------------------ |
| Template             | HTML with additional markup                                  |
| Directives           | Extend HTML with custom attributes and elements              |
| Model                | The data shown to the user in the view and with which the user interacts |
| Scope                | Context where the model is stored so that controllers, directives and expressions can access it |
| Expressions          | Access variablers and functions from the scope               |
| Compiler             | Parses the template and instantiates directives and expressions |
| Filter               | Formates the value of an expression for display to the user  |
| View                 | What the user sees (the DOM)                                 |
| Data Binding         | Sync data between the model and the view                     |
| Controller           | The business logic behind the views                          |
| Dependency Injection | Creats and wires objects and functions                       |
| Injector             | Dependency injection container                               |
| Module               | A container for the different parts of an app including controllers, services, filters, directives which configures the Injector |
| Service              | Reusable business logic independent of views                 |

- The purpose of controllers is to expose variables and functionality to expressions and directives.
- Everything within AngularJS (directives, filters, controllers, services, ...) is created and wired using dependency injection.

## Data Binding

- The automatic synchronization of data between the model and view components.
- Lets you treat the model as the single-source-of-truth.
- When the model changes, the view reflects the change, and vice versa.
- Classical template systems
  - One-way data binding, once the view is rendered, that is done. You have to write more code to handle a post.
- AngularJS Templates
  - First the template is compiled by the browser. This produces a live view.
  - Any changes to the view are immediately reflected in the model.
  - Any changes in the model are propagated to the view.
  - Think of the view as an instant projection of your model.

## Controllers

- Set up the initial state of the `$scope` object
- Add behaviour to the `$scope` object
- In general, a Controller shouldn't try to do too much. It should contain only the business logic needed for a single view.
- Adding behaviour to a Scope Object
  - Attaching methods to the `$scope`
  - Methods assigned to the scope are available in the template / view, can be invoked via AngularJS expressions `{{}}` and `ng` event handler directives e.g. `ngClick`.
- Nested Controllers leads to scope inheritance.
  - The scope that each Controller receives will have access to properties and methods defined by Controllers higher up the hierarchy.
  - Scope Inheritance works with methods in the same way as it does properties.
  - Children can override (aka shadow) methods and properties by using the same name

## Services

- Used to organise and share code across your app.
- Lazily instantiated.
- Singletons.
- Built-in services always start with a `$`
- Note that you are not registering a service instance, but rather a factory function that will create this instance when called.

## Scopes



## Components

- A special kind of directive that uses a simpler config, suitable for a component-based application structure.
- 

## Pluralsight - AngularJS: Get Started by Scott Allen

- Can only have one `ng-app` directive
- 

