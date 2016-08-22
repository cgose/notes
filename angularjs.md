# AngularJS

## Controllers
- Is responsible for setting scope
- Responsible for handing data to view

## Services
- Handle all non view logic
- communicates with the server
- holds data & state
- DOM manipulation

## Directives
- can include controller and a view
- DOM manipulation should be handled in directive
- Receive View Events

## Views
- Display the Application
- Declare Bindings & Directives
-
> is it okay to manipulate a the DOM in the controller? No
> Is it okay to manupulate the DOM from a service? Depends, should really use a directive. Should really be rare
> Business logic belongs in services

## Minifications
- remove white spaces
- Shorten Variables & Parameters

Minification can cause problems in Angular because it  uses refelction to get function and object names
### Best practices
- Don't minify??? - Minifying for most applications doesn't make a difference
- Manually Minsafe
- use ngmin
- Don't mangle parameter name

> Main benefits of minification: Size and Obscurity
> 2 methods of minifying code: Removing whitespace and renaming variables and parameters
> Minification isn't always safe

# Understanding Controllers
- A controller cordinates the view with the model.
- Don't have too many collaborators
- Can use Angular.module().value(name, object) can inject into controller this way
- Is it testable? If it is hard to test you can break it down into smaller controllers or simplify the code
-
# Understanding Services
- handle non-view logic
- Communicate with Server
- Hold data & state
## Create a service
Can use the following:
- value
- constant
- factory
- service
- provider
- Filters are also a service

## Services design
- SRP
- Cohesive
- Loosely Coupled
- Good Interface
- Testable

    Services should be the meat of your application

### SRP (Single Responsibility Principle)
- Service should be responsible for one thing
- If it handles multiple things then the service will need to be updated when for too many things
### Cohesive
- Like SRP it should encompass everything needed to handle its purpose
### Loosely Couple
- Shouldn't be dependent on to many couplings. 
- If service is being used multiple times to 
### Good Interface
- Should be able to call one method to get what you want
### Testable
- Everything should be testable

## Service Types
- Factories
- Stateful Singletons
- Functions

### Factories
> Factories are used to create objects
```javascript
//TODO: Add example
```

### Stateful Singletons
> Hold user state as they travel through your app
```javascript
//TODO: Add Example
```

### Functions
> Service can be used to return a single function
> Rare but can be used when a service is required to run a single calculation or something to that nature
```javascript
//TODO: Add Example
```
