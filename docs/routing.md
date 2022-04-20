# Routing (Server-side)
## What?
Server-side routing allows for the mapping of url endpoints to methods within controllers.

## Why?
For the most part, routes allow controller methods to remain protected (not accessable unless mapped).
But routes also help an application define its zones and endpoints.

## How?
Each framework will have its own methods and rules for defining routes.
However, each framework will also have some things in common, like:
- Ability to map endpoints (such as http://example.com/test), zones (such as http://example.com/zone_1/about), and wilcard variables (http://example.com/profile/1) to controller methods.
- Ability accept or deny GET / POST requests
- Ability to permit or deny Cross-Origin Resource Sharing (CORS)
- Ability to modify/read query (?...) & fragment (#...) strings 

Please refer to the documentation of the framework you wish to implement.