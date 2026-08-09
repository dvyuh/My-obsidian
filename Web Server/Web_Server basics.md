a combination of computer hardware and software that stores website files and delivers them to a user's web browser over the internet using HTTP or HTTPS protocols.

## A URL
basically the url is the address of the webserver it needs to find and share it with the host browser.

**http- Hyper Text Transfer Protocol**

before any http request is made browser needs to make a "TCP connection"

### TCP or Transmission Control Protocol
is a core transport layer communication standard. I**t ensures reliable, ordered, and error-checked delivery of data** between applications across a network. Working alongside the Internet Protocol (IP), it breaks data into segments, tracks packet sequence numbers, and retransmits any lost data

The client and server use **Sockets** to form a TCP connection
so what are Sockets?

### Sockets
A software endpoint that enables two-way data communication between different programs on a network or the same computer.
Formed by combining an IP address and a port number.

---

Rn to learn this im using telnet. its a command line tool to connect to the localhost server.

---

so using this i simulated the browesr.
```
GET /hello HTTP/1.1
```
get is the http method
hello is the path
http/1.1 is the http version
the original url was aka the server url
```
http://localhost:8888/hello
```

The response status line _HTTP/1.1 200 OK_ consists of 
the _HTTP Version_,
the _HTTP status code_ and 
the _HTTP status code reason_ phrase _OK_.

---
## so how does a webserver works?

The Webserver creates a listening socket.  and accepts new connection in a loop. aka a hole(socket)
now the client(us) have another socket and we create a TCP connection 
now after creating the connection we send a HTTP request
that contains the address of the thing we want and then the server responds with an HTTP response.
