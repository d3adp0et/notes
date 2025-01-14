# HyperText Transfer Protocol (HTTP) Fundamentals


### Imp points:
- port 80 and 443
- ctrl+shift+i to open **DEVTOOLS** in browser(generally)
- cURL is a GET method


### Imp commands:
- cURL [curl <url>]
	- important extensions: -v(for verbose); -vvv(for extended verbose); -s(for silent mode); -k(specific for https to skip certificate check)
	- -I to only display response headers

## HTTP Headers
### types:
- General (..Headers): contextuat, used to describe message rather than the content
	- date
	- connection close/open
- Entity..: used to describe the content transferred by a message, found in responses and POST/PUT request
	- Content-Type
	- Media-Type
	- Boundary: to set boundary between messages
	- Content-Length
	- Content-Encoding
- Request..: sent during a request from client to host, does not contain any info on content of the message
	- Host: domain the request is being sent to **(future)**
	- User-Agent: to reveal things about client
	- Referrer:  Referrer header is intended to let you know where the client is coming from - where it was just before that request **(past)**
	- Accept: */* denotes all media types are accepted
	- Cookie: donates identifier on both client and host sides...maintaining clients access to server.
	- Authorization: also identifies tokens...stored on client which the server requests
- Response..: used in HTTP response from server to client
	- Server
	- Set-Cookie
	- WWW-Authenticate: type of authentication to access requested resource
- Security..: A class of response headers, used to specify certain rules and policies for the browser to follow while accessing the website
	- Content-Security-Policy: Dictates the website's policy towards externally injected resources. This could be JavaScript code as well as script resources. This header instructs the browser to accept resources only from certain 				   trusted domains, hence preventing attacks such as Cross-site scripting (XSS).
	- Strict-Transport-Security: Prevents the browser from accessing the website over the plaintext HTTP protocol, and forces all communication to be carried over the secure HTTPS protocol.
	- Referrer-Policy: Dictates whether the browser should include the value specified via the Referer header or not. It can help in avoiding disclosing sensitive URLs and information while browsing the website.

 
# HyperText Transfer Protocol (HTTP) Methods

- HTTP supports multiple methods for accessing a resource.
- commonly used methods:
	- GET: req a specific resource
	- POST: sends data to server (pdf, text, other binary data in the request's body section)
	- HEAD
	- PUT: 	Creates new resources on the server. Allowing this method without proper controls can lead to uploading malicious resources.
	- DELETE: Deletes an existing resource on the webserver. If not properly secured, can lead to Denial of Service (DoS) by deleting critical files on the web server.
	- OPTIONS
	- PATCH

---
Note: Most modern web applications mainly rely on the GET and POST methods. However, any web application that utilizes REST APIs also rely on PUT and DELETE, which are used to update and delete data on the API endpoint, respectively. Refer to the Introduction to Web Applications module for more details.
---

### Response Codes
- HTTP status codes are used to tell the client the status of their request.
- five types of response headers:
	- 1xx : returns status without affecting the process
	- 2xx : returns when process succeeds
	- 3xx : returns when the server redirects the client
	- 4xx : improper request from client
	- 5xx : returned when the server has a problem
- common examples of response codes:
	- 200 OK
	- 302 Found
	- 400 Bad Request
	- 403 Forbidden
	- 404 Not Found
	- 500 Internet Error

### GET
to obtain any remote resources when accessing an URL.