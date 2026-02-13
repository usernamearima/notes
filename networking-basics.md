# Networking Basics

These notes cover fundamental networking concepts used in cybersecurity.
They focus on understanding how systems communicate on a network.

---

## 1. Client and Server Model

Network communication is based on the client–server model.

Client → request → server  
Server → response → client  

The **client** initiates communication.
The **server** waits for requests and responds.

Examples of clients:
- web browsers
- command-line tools
- applications

Examples of servers:
- web servers
- API servers
- file servers
- email servers

---

## 2. What Is a Server

A server is a computer that listens for incoming requests.

A server can provide:
- websites
- APIs
- files
- email services
- device communication

Important concept:
A server does not ask first.
It waits until a client sends a request.

---

## 3. IP Address

An IP address identifies a computer on a network.

Examples:
- 192.168.1.1 (local network)
- 8.8.8.8 (public address)

The IP address tells the network:
**where the data should be sent**.

Without an IP address, a computer cannot communicate over a network.

---

## 4. Ports

A port identifies a specific program running on a computer.

Think of it as:
- IP address → the computer
- Port → the application on that computer

Common ports:
- 80 – HTTP
- 443 – HTTPS
- 22 – SSH
- 21 – FTP

IP + port = exact service on a specific machine.

---

## 5. HTTP – Requests and Responses (Networking View)

HTTP is a protocol used by clients and servers to communicate.

Basic flow:
Client → HTTP request → Server  
Server → HTTP response → Client  

An HTTP request asks for a resource or action.
An HTTP response contains the result.

Common HTTP status codes:
- 200 – OK (request successful)
- 404 – Not Found (resource does not exist)
- 500 – Internal Server Error (server-side issue)

---

## 6. TCP and UDP

### TCP – Transmission Control Protocol

TCP is a reliable, connection-based protocol.

Before data is sent, TCP uses a **three-way handshake**:
1. SYN – client requests a connection
2. SYN/ACK – server accepts the request
3. ACK – client confirms the connection

TCP ensures:
- data delivery
- correct order
- error handling

Used by:
- HTTP / HTTPS
- SSH
- FTP

---

### UDP – User Datagram Protocol

UDP is connectionless and faster than TCP.

Characteristics:
- no handshake
- no guarantee of delivery
- lower latency

UDP is used when speed is more important than reliability
(e.g. DNS, streaming).

---

## 7. Network Interfaces and IP Configuration

A computer must have an IP address to use a network.

Command:
```bash
ip a

This command shows:
network interfaces
assigned IP addresses
interface state (UP / DOWN)

Common interfaces:
lo – localhost (127.0.0.1)
eth0 – wired connection
wlan0 – wireless connection

Used for:
checking network configuration
troubleshooting connectivity
```
---

## 8. Ping

Ping checks connectivity between two computers.

Usage:
ping 8.8.8.8
ping google.com

If responses are received:
the connection works

If no response:
network issue
wrong address
destination is unreachable

Stop ping:
Ctrl + C

Ping is used to:
test internet access
test DNS resolution
check if a host is alive

---

## 9. Traceroute

Traceroute shows the path packets take to reach a destination.

Usage:
traceroute google.com

Each line represents one hop (router).

* * * means no response from that hop (normal behavior).

Used to:
identify where a connection fails
analyze routing paths
debug network issues

---

## 10. DNS – Domain Name System

DNS translates domain names into IP addresses.

Computers do not understand names like google.com.
They communicate using IP addresses.

Flow:
Domain name → DNS → IP address → connection

---

## 11. DNS Tools

nslookup
Basic DNS lookup tool.
nslookup google.com


Shows:
domain name
resolved IP address

dig
Advanced DNS inspection tool.

dig google.com

Important part:
ANSWER SECTION

DNS tools are used to:
troubleshoot network issues
verify domain resolution
debug connectivity problems
