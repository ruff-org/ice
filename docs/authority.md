# Authority
## What?
Trust within an application context is established using zones; wherein a same-site strategy prefers local resources within the root zone. The root zone is the base-url of the current application context.

## Why?
The same-site strategy helps mitigate the risk of man-in-the-middle attacks, but it is not perfect. It is preferred to use HTTPS (TLS) in production, but in development, the same-site strategy allows HTTP resources to be linked along-side external (CDN) resources.

## How?
The following model demonstrates the parts of a URI string:
```
[scheme]://[host]:[port]/[path]?[query]=[value]#{fragment}
```

* Scheme: Defines the protocol of access (such as: file, ftp, git, http, https)
* Host: Defines the root zone (such as: localhost or www.example.com)
* Port: Defines the bound listening port of the server (such as: 8080 or 443)
* Path: Defines the requested resource tree (such as: cities/boston/all.html)
* Query: Defines an optional query string key argument, passed to the server at each request (such as: name)
* Value: Defines the supplied value for the preceding key argument (such as: bob)
* **Additional query string arguments can be suppied, given they are seperated by an "&"**
* Fragment: Defines an optional fragment string (such as: section1)
* **Fragment strings are not passed to the server, instead they control client-side routing**

Please refer to the documentation of the framework you wish to implement.