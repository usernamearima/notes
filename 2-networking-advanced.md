# Networking Advanced

These notes cover more advanced networking concepts
that build on basic networking fundamentals.
They focus on understanding how traffic flows,
how networks are segmented, and how access is controlled.

---

## 1. Network Layers (High-Level View)

Networking is often described using layers.
Each layer has a specific role.

Simplified view:
- Application layer – HTTP, DNS, FTP
- Transport layer – TCP, UDP
- Network layer – IP
- Link layer – Ethernet, Wi-Fi

Each layer solves a different problem.
This separation helps with troubleshooting and design.

---

## 2. TCP Flags and Connections

TCP communication uses flags to manage connections.

Common TCP flags:
- SYN – start connection
- ACK – acknowledge data
- FIN – close connection
- RST – reset connection

These flags are used to:
- establish connections
- transfer data
- close connections
- handle errors

Understanding TCP flags helps explain:
- connection failures
- resets
- unusual network behavior

---

## 3. Stateful vs Stateless Communication

### Stateless
Each request is independent.
The server does not remember previous requests.

Examples:
- basic HTTP requests
- DNS queries

### Stateful
The server keeps track of client state.

Examples:
- TCP connections
- authenticated sessions

Security relevance:
- state handling errors can cause vulnerabilities
- improper session handling can expose data

---

## 4. NAT – Network Address Translation

NAT translates private IP addresses to a public IP address.

Why NAT exists:
- IPv4 address shortage
- hiding internal network structure

Example:
- internal IP: 192.168.1.10
- public IP: one shared internet address

NAT is commonly used in:
- home networks
- corporate networks
- cloud environments

---

## 5. Private vs Public IP Addresses

### Private IP Ranges
- 10.0.0.0 – 10.255.255.255
- 172.16.0.0 – 172.31.255.255
- 192.168.0.0 – 192.168.255.255

Private IPs:
- are not routable on the internet
- are used inside internal networks

Public IPs:
- are reachable from the internet
- identify networks externally

---

## 6. Routing Basics

Routing decides how packets move between networks.

A router:
- receives a packet
- checks the destination IP
- forwards the packet to the next hop

Packets may pass through:
- multiple routers
- different networks
before reaching the destination.

Traceroute visualizes this process.

---

## 7. Firewalls (Conceptual)

A firewall controls network traffic based on rules.

Firewalls can:
- allow traffic
- block traffic
- log traffic

Rules are often based on:
- IP address
- port
- protocol
- direction (inbound / outbound)

Firewalls are a key security control point.

---

## 8. Network Segmentation

Network segmentation divides a network into smaller parts.

Why segmentation is used:
- limit access
- reduce attack surface
- contain damage

Examples:
- separating user network from servers
- isolating admin systems
- separating development and production

Segmentation improves security and visibility.

---

## 9. East-West vs North-South Traffic

### North-South Traffic
Traffic entering or leaving a network.
Example:
- user → internet
- internet → server

### East-West Traffic
Traffic inside the same network.
Example:
- server → server
- application → database

Security monitoring must consider both types.

---

## 10. Network Visibility and Logging

To secure a network, you need visibility.

Visibility includes:
- knowing which systems communicate
- knowing which ports are used
- knowing normal vs abnormal traffic

Logs may come from:
- firewalls
- routers
- servers

Without visibility, detection is ineffective.

---

## Key Takeaways

- Networking is layered
- TCP manages reliable communication
- NAT hides internal networks
- routing defines traffic paths
- firewalls enforce rules
- segmentation limits damage
- visibility enables security
