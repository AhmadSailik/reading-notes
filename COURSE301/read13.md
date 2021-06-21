## In your own words, describe what each group of status code represents:
- 100’s =its request will fail before they start sending the body
- 200’s =its request was accepted
- 300’s =These are redirection codes
- 400’s =These are the client error codes like missing authentication
- 500’s =These are the server error codes
## What is a status code 202?
This code tells the client that the request was valid, but its processing will finish sometime in the future.
## What is a status code 308?
This tells the client to use another URL to access the resource and not use the current URL anymore
## What code would you use if an update didn’t return data to a client?
204 No Content
## What code would you use if a resource used to exist but no longer does?
414 Request-URI Too Long
## What is the ‘Forbidden’ status code?
The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## What does a 500 error status code mean?
Internal Server Error
## What is the difference between a status 200 and a status 201?
200 it's  tell the client everything went good but not create endpointlik 201