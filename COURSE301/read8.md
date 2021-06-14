## What does REST stand for?
is an architectural style for building distributed systems based on hypermedia.
## REST APIs are designed around a ____.
resources
## What is an identifer of a resource? Give an example.
https://adventure-works.com/orders/1
## What are the most common HTTP verbs?
GET, POST, PUT, PATCH, and DELETE.
## What should the URIs be based on?
nouns (the resource) and not verbs (the operations on the resource)
## Give an example of a good URI.
/customers/1/orders/99/products
## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
it's bad because it's expose a large number of small resources.
## What status code does a successful GET request return?
returns HTTP status code 200 (OK)
## What status code does an unsuccessful GET request return?
the method should return 404 (Not Found).
## What status code does a successful POST request return?
return HTTP status code 200 and include the result of the operation in the response body.
## What status code does a successful DELETE request return?
the web server can return HTTP 404 (Not Found).