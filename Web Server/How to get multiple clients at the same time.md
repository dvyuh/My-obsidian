## SOCKET PAIR

The _socket pair_ for a TCP connection is a 4-tuple that identifies two endpoints of the TCP connection,
- the local IP address
- local port
- foreign IP address
- foreign port
A socket pair uniquely identifies every TCP connection on a network. The two values that identify each endpoint, an IP address and a port number, are often called a _socket_.

how code works:
```
def serve_forever()
```

#### The server creates a TCP/IP socket:
```
listen_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
```

#### The server might set some socket options
```
listen_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
```
#### the server binds the address. The _bind_ function assigns a local protocol address to the socket.

```
listen_socket.bind(SERVER_ADDRESS)
```
#### then, the server makes the socket a listening socket
```
listen_socket.listen(REQUEST_QUEUE_SIZE)
```


---

## PROCESS
A _process_ is just an instance of an executing program. When the server code is executed, for example, it’s loaded into memory and an instance of that executing program is called a process.


## FILE DESCRIPTOR
A _file descriptor_ is a non-negative integer that the kernel returns to a process when it opens an existing file, creates a new file or when it creates a new socket.

