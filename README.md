# ice
Blazed Ice Core Library &amp; Docs

## Servers
- Arctic/Apache
- Arctic/*NIX
- Arctic/Tomcat

## Utilities
- [Sky](https://github.com/ruff-org/sky)
- [Ice (PHP)](https://github.com/blazed-space/ice)

## Versions
- [Ice/Php](https://github.com/blazed-space/blz-ice-php)
- [Ice/Python](https://github.com/blazed-space/blz-ice-py)
- [Ice/Node](https://github.com/blazed-space/blz-ice-node)
- Ice/Java
- Ice/Go
- Ice/Ruby
- Ice/C#

## Core Objectives
* Authority (Origin grouping)
  * Protocol (ex: https)
  * Host/Root Zone (ex: example.com)
  * Port/Application Zone (ex: 8080)
    * URI EX: {Protocol}://{Host}:{Port}/
* Controllers
* Routing (Server-side/Request based)
  * Relative-part zoning (ie. http://example.com/about/)
  * Query string (?...)
  * Fragment string (#...)
* Static file service
    * MD5 digest header (for integrity check)
    * Standard encoding (ex: utf-8) or compression (ex: gzip)
	* MIME types
	* Caching
* Presenter service
  * Markdown (or other front-matter) parser
  * Document object (for rendering the HTML document)
  * SSR Template Hydration (using the presenter)
* State service
  * Cookies
  * Sessions
    * Authentication (IAM)
* Redirects & Errors
* TLS & HTTPS
* HTTP2

## Advanced Objectives
### Database ORMs and connectors
- API or static file
  - JSON, CSV, Text, etc.
- Database
  - MySQL
  - PostgresSQL
  - MongoDB
  - Redis
### Content management systems
- Admin-access site editor
- Role based CRUD user interfaces (and APIs)
- Service-based virtual containers
### Authentication systems
- B2C: Business to customer
  - Email & password
  - Phone number & password
  - Username & password
  - Facebook, Google, Github, etc.
  - Temporary or guest accounts
- B2B: Business to business
  - SAML
  - LDAP
  - Active Directory
- B2E: Business to employee