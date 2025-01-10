# HyperText Transfer Protocol (HTTP)

### Imp points:
- port 80 and 443
- ctrl+shift+i to open devtools in browser(generally)
- cURL is a GET method


### Imp commands:
- cURL [curl <url>]
	- important extensions: -v(for verbose); -vvv(for extended verbose); -s(for silent mode); -k(specific for https to skip certificate check)

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
	- Referer:  Referer header is intended to let you know where the client is coming from - where it was just before that request **(past)**
	- Accept: */* denotes all media types are accepted
	- Cookie: donates identifier on both client and host sides...maintaining clients access to server.
	- Authorization: also identifies tokens...stored on client which the server requests
- Response..: 
- Security..: