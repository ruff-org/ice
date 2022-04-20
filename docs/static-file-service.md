# Static file service
## What?
Each Ice server is capable of serving a variety of static files, which can be loaded, loaded & hydrated, or dynamically built. The static file service is also capable of building and bundling scripts, libraries, and multimedia files. When building API's, the static file service can also build/deliver JSON objects.

## Why?
A standard Ice server must implement the HTTP/1.1 protocol [(RFC-2616)](https://www.w3.org/Protocols/rfc2616/rfc2616.html), which allows the transfer of a data entity (given the response code permits such) within the response object. Note: Static files (such as .html, .js, .css, etc.) must be requested and delivered one-at-a-time via URI GET requests (ex: GET:http://example.com/, GET:http://example.com/js/script.js).

## How?
At its simplist, an Ice server will simply host all files within the /public directory, and will automatically create routes to access them. However, if one wishes to use server-side rendering (SSR), they must configure a controller and a route to load one or more views using the presenter interface. The developer can set default MIME types within the respective application's configuration.

* **Generated files can be cached to conserve resources**
* **A compression library can be used to deliver lighter files**
* **MIME types are set in the application config**

### Ice also supports data URL's
* Example:
```html
 <img src="data:image/gif;base64,R0lGODdhMAAwAPAAAAAAAP///ywAAAAAMAAw
   AAAC8IyPqcvt3wCcDkiLc7C0qwyGHhSWpjQu5yqmCYsapyuvUUlvONmOZtfzgFz
   ByTB10QgxOR0TqBQejhRNzOfkVJ+5YiUqrXF5Y5lKh/DeuNcP5yLWGsEbtLiOSp
   a/TPg7JpJHxyendzWTBfX0cxOnKPjgBzi4diinWGdkF8kjdfnycQZXZeYGejmJl
   ZeGl9i2icVqaNVailT6F5iJ90m6mvuTS4OK05M0vDk0Q4XUtwvKOzrcd3iq9uis
   F81M1OIcR7lEewwcLp7tuNNkM3uNna3F2JQFo97Vriy/Xl4/f1cf5VWzXyym7PH
   hhx4dbgYKAAA7" />
```

Please refer to the documentation of the framework you wish to implement.