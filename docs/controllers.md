# Controllers
## What?
Controllers hold most application logic, and also help bootstrap views and data into a response body. 

## Why?
Controllers enforce a clear separation between application logic, configuration, the presenter, and views.

## How?
Each framework will have its own methods and rules for defining controllers.
However, each framework will also have some things in common, like:
- Control over a "zone" of the application 
- Ability to forge & mutate response object
- Ability to access request object
- Ability to define/override routes
- Ability to load/hydrate view files (using a singleton "presenter" interface)
- Ability to Create, Read, Update, and Detele data via models
- Ability to implement access control within zones (using authentication middleware)

Please refer to the documentation of the framework you wish to implement.