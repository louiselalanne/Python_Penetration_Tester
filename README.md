# Python Penetration Tester

Sockets are the endpoints of a bidirectional communication channel. They may communicate within a process, between processes on the same machine or between processes on different machines. On a similar note, a network socket is one endpoint in a communication flow between two programs running over a computer network such as the Internet. It is purely a virtual thing and does not mean any hardware. Network socket can be identified by a unique combination of an IP address and port number. Network sockets may be implemented over a number of different channel types like TCP, UDP, and so on.

The different terms related to socket used in network programming are as follows:

- Domain
Domain is the family of protocols that is used as the transport mechanism. These values are constants such as AF_INET, PF_INET, PF_UNIX, PF_X25, and so on.

- Type
Type means the kind of communication between two endpoints, typically SOCK_STREAM for connection-oriented protocols and SOCK_DGRAM for connectionless protocols.

- Protocol
This may be used to identify a variant of a protocol within a domain and type. Its default value is 0. This is usually left out.

- Hostname
This works as the identifier of a network interface. A hostname nay be a string, a dotted-quad address, or an IPV6 address in colon (and possibly dot) notation.

- Port
Each server listens for clients calling on one or more ports. A port may be a Fixnum port number, a string containing a port number, or the name of a service.

# Python’s Socket Module for Socket Programming
To implement socket programming in python, we need to use the Socket module. Following is a simple syntax to create a Socket:
~~~
import socket
s = socket.socket (socket_family, socket_type, protocol = 0)
~~~
Here, we need to import the socket library and then make a simple socket. Following are the different parameters used while making socket:

- socket_family − This is either AF_UNIX or AF_INET.
- socket_type − This is either SOCK_STREAM or SOCK_DGRAM.
- protocol − This is usually left out, defaulting to 0.
