# The Internet

### Why should I know how the internet works?

As developers, we need to understand how the internet works because it is the backbone of our applications. Knowing how the internet works will help us to understand how to build applications that are fast, reliable, and scalable. 

### What is the internet?

The internet is a global network of computers that are connected to each other. 
And what is a `network`?
A network is a group of computers that are connected to each other.
So, the internet is a network of networks.

### How does the internet work?

In easy words, the internet works by connecting computers to each other using standardized protocols, and these protocols are responsible for defining how computers communicate with each other effectively and securely.

At its core, internet is a global network of interconnected routers, which are responsible for routing data packets between computers. When you send a message to a friend, the message is broken down into small packets of data and sent to the router. The router then routes the packet to the destination computer.

To ensure that the data packets are delivered to the correct destination, the routers use a protocol called IP (Internet Protocol). IP is responsible for addressing the data packets and routing them to the correct destination.

The other protocol that is responsible for ensuring that the data packets are delivered accurately and securely is TCP (Transmission Control Protocol). TCP is responsible for ensuring that the data packets are delivered in the correct order.

Some other protocols that are used to ensure that the data packets are delivered accurately and securely are HTTP (Hypertext Transfer Protocol), HTTPS (Hypertext Transfer Protocol Secure), DNS (Domain Name System) and SSL/TLS (Secure Sockets Layer/Transport Layer Security).

### Terminologies

- **IP Address**: An IP address is a unique identifier assigned to each device connected to the internet. It is used to identify the device on the network and to route data packets to the correct destination.
- **Domain Name**: A domain name is a human-readable name that is used to identify a computer on the internet. It is used to make it easier to remember the IP address of a computer.
- **DNS**: DNS is a system that is used to translate domain names into IP addresses.
- **HTTP**: HTTP is a protocol that is used to transfer data between a web server and a web browser.
- **HTTPS**: HTTPS is a secure version of HTTP that is used to transfer data between a web server and a web browser.
- **SSL/TLS**: SSL/TLS is a protocol that is used to secure the communication between a web server and a web browser.
- **Packet**: A packet is a small unit of data that is sent over the internet.
- **Router**: A router is a device that is used to direct data packets between computers.
- **Server**: A server is a computer that is used to store and serve data to other computers.
- **Client**: A client is a computer that is used to request data from a server.

The benifit of following standardized protocols is different devices can communicate with each other effectively and securely, as long as they follow the same protocols.

## IP Address and Domain Names

IP addresses are used to identify devices on a network. They are made up of a series of numbers separated by dots. For example, 192.168.1.1 is an IP address.

Domain names are used to identify computers on the internet. They are made up of a series of words separated by dots. For example, www.google.com is a domain name.

Domain names are easier to remember than IP addresses, and they are easier to type. 

### How does DNS work?

DNS is a system that is used to translate domain names into IP addresses. When you type a domain name into your web browser, the DNS server will translate the domain name into the corresponding IP address.

## HTTP and HTTPS

HTTP is a protocol that is used to transfer data between a client (such as a web browser) and a server (such as website). 

When we visit a website, the browser sends a request to the server, and the server responds with the requested data. This is done using the HTTP protocol.

HTTPS is a secure version of HTTP that is used to transfer data between a client and a server. HTTPS is used to ensure that the data is transferred securely and accurately. Data is encrypted using SSL/TLS before it is sent over the internet.

## TCP/IP

TCP/IP provides a ordered, reliable, and error-checked delivery of a stream of bytes between applications running on hosts communicating via an IP network. 

There are a few key concepts that are important to understand about TCP/IP:
- **Ports**: Ports are used to identify the application that is sending or receiving data on a device/host. 
  - Ports are numbered from 0 to 65535.
  - Ports 0 to 1023 are well-known ports and are reserved for common services.
  - Ports 1024 to 49151 are registered ports and are used for custom applications.
  - Ports 49152 to 65535 are dynamic ports and are used for temporary connections.
  - An application can listen on a specific port and wait for incoming connections or data on that port.
  - Ports are used to send data as well. For example, a sender specified an IP address and a port number, the sender uses one of its own ports (a source port) to send data to the receiver. The receiver is listening on a specific port (a destination port) and receives the data.
  - A web browser sends a request to a web server, Here the source port is a temporary port assigned by the web browser (e.g. 51234) and the destination port is the port number that the web server is listening on (e.g. 80). The web server responds to the web browser, here the source port is the port number that the web server is listening on (e.g. 80) and the destination port is a temporary port assigned by the web browser (e.g. 51234).
- **Sockets**: Sockets are combinations of an IP address and a port number, and they are used to identify the application that is sending or receiving data. 
  - IPC (Inter-Process Communication) sockets, also known as Unix domain sockets, enable communication between processes on the same host.
  - Network sockets enable communication between processes on different hosts.
- **Connection**: A connection is a communication path between two devices/hosts. It is established between two sockets. During the connection establishment, the two devices/hosts exchange information about themselves and the connection parameters.

## SSL/TLS

SSL/TLS is a protocol that is used to secure the communication between a client and a server. Data is encrypted using SSL/TLS before it is sent over the internet.

There are a few key concepts that are important to understand about SSL/TLS:
- **Handshake**: The handshake is the process of establishing a secure connection between a client and a server. The client and server exchange information about themselves and the connection parameters.
- **Encryption**: Encryption is the process of encrypting data with the agreed upon algorithm and key so that it cannot be read by anyone except the intended recipient.
- **Decryption**: Decryption is the process of decrypting data with the agreed upon algorithm and key so that it can be read by the intended recipient.
- **Certificate**: A certificate is a digital document that is used to verify the identity of a server. It is signed by a trusted third party (such as a certificate authority).

When building internet-based applications it is important to understand how SSL/TLS works, so that we can transfer sensitive data like passwords, credit card numbers, etc. securely. We also need to obtain and maintain a valid SSL/TLS certificate for our server. This is all to ensure integrity and confidentiality of the data that is transferred over the internet.

## Hosting

Hosting is the process of storing and serving data to other computers.
There are various types of hosting:
- **Shared Hosting**: Shared hosting is a type of hosting where multiple websites share the same server.
- **Virtual Private Server (VPS) Hosting**: VPS hosting is a type of hosting where a single physical server is divided into multiple virtual servers. Each virtual server is a separate operating system instance with its own IP address, storage, and resources.
- **Dedicated Hosting**: Dedicated hosting is a type of hosting where a single physical server is dedicated to a single website.
- **Cloud Hosting**: Cloud hosting is a type of hosting where a server is hosted on a cloud computing platform.
- **Managed Hosting**: Managed hosting is a type of hosting where a hosting provider manages the server for the client.

### The difference between web page, website and web server

- **Web Page**: A web page is a single document that is served by a web server. Think of it as a single page in a book.
- **Website**: A website is a collection of web pages that are served by a web server. Think of it as an entire book. As website is what a user sees when they visit a domain name.
- **Web Server**: A web server is a computer that is used to serve web pages to clients. Think of it as a library that stores many books and gives the requested book to you when you ask for it.

## Web Servers

The web server can refer to the software that is running on a computer, or the computer itself.

- On the hardware side, a web server is a computer that is used to serve web pages to clients. It stores the web pages and serves them to the clients when they request them.
- On the software side, a web server is the software that is running on a computer that is used to serve web pages to clients. It is responsible for receiving requests from clients, processing them, and returning the appropriate web page. An HTTP server is software that understands URLs and the protocol itself. 

At the most basic level, whenever a browser needs a file that is hosted on a web server, the browser requests the file via HTTP. When the request reaches the correct (hardware) web server, the (software) web server processes the request and returns the appropriate web page.

### Static vs Dynamic web servers:
- Static web servers: Static web servers are servers that serve static web pages. They consist of a computer (hardware) and an HTTP server (software). Static web pages are pages that are not generated dynamically. They are stored on the server and served as they are.
- Dynamic web servers: Dynamic web servers are servers that serve dynamic web pages. They consist of a static web server plus extra software, most commonly an application server and a database. It is called dynamic because the application server updates the hosted files based on the request.

For example, to produce the final webpages you see in the browser, the application server might fill an HTML template with data from a database. Sites like Wikipedia have thousands of webpages. Typically, these kinds of sites are composed of only a few HTML templates and a giant database, rather than thousands of static HTML documents. 

To summarize, to fetch a webpage, your browser sends a request to the web server, which searches for the requested file in its own storage space. Upon finding the file, the server reads it, processes it as needed, and sends it to the browser. Let's look at those steps in more detail.

