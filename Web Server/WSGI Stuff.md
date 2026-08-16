so to run a django application or any frontend framework application on any server
wsgi is used
its a compatibility layer that allows this to happen
WSGI- Web Server Gateway Interface

it allows you to mix and match your Web servers and Web frameworks
## code snippet 
from the webserver2.py

```
def run_application(application):
    """Server code."""
    # This is where an application/framework stores
    # an HTTP status and HTTP response headers for the server
    # to transmit to the client
    headers_set = []
    # Environment dictionary with WSGI/CGI variables
    environ = {}

    def start_response(status, response_headers, exc_info=None):
        headers_set[:] = [status, response_headers]

    # Server invokes the ‘application' callable and gets back the
    # response body
    result = application(environ, start_response)
    # Server builds an HTTP response and transmits it to the client
    ...

def app(environ, start_response):
    """A barebones WSGI app."""
    start_response('200 OK', [('Content-Type', 'text/plain')])
    return [b'Hello world!']

run_application(app)

```

### How it works
basically
- the framework like "flask" provides an application callable 
- the server envokes the callable for each request it recieves from the HTTP client. it then passes the dictionary "environ" containing the WSGI/CGI variables
- the framework application generates an http status and http response headers and passes them to the "start_response" callable for the server to store them.
- the server combines the status, the response header and response body into an HTTP response and transmits it to the client

---
## Now what does the server transmits to the client

similar in the web_server basics
but with additional stuff
**Content-Type, Content-Length,Date, and Server**

### what is environ dictionary
its a python dictionary that must contain certain WSGI and CGI variables predescribed by the wgsi Specification.
like server_name. or Server_port
