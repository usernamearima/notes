# Security Tools Overview

These notes provide a high-level overview of common tools
used across cybersecurity domains.
The focus is on purpose and use cases, not exploitation.

All tools are referenced for learning and legal labs only.

---

## 1. Tool Categories

Security tools can be grouped by purpose:
- networking and diagnostics
- web and API testing
- system administration
- monitoring and detection
- incident response

Understanding categories helps choose the right tool.

---

## 2. Networking Tools

### ping
Used to test connectivity between systems.

Typical use:
- check if a host is reachable
- test basic network access

---

### traceroute
Used to view the path traffic takes across networks.

Typical use:
- diagnose routing issues
- identify where connectivity fails

---

### ip / ipconfig
Used to inspect network configuration.

Typical use:
- check IP addresses
- inspect network interfaces

---

## 3. Web and API Tools

### curl
Used to send HTTP requests from the command line.

Typical use:
- test HTTP responses
- inspect headers
- interact with APIs

---

### wget
Used to download files from the internet.

Typical use:
- retrieve files
- automate downloads
- fetch resources for labs

---

### Browser Developer Tools
Built into modern browsers.

Typical use:
- inspect requests and responses
- analyze headers
- debug frontend behavior

---

## 4. Intercepting Proxies

### Burp Suite (Conceptual)
Used to observe and modify HTTP traffic.

Typical use:
- understand request/response flow
- analyze authentication logic
- test application behavior (legal scope only)

---

## 5. System Administration Tools

### nano / vim
Text editors for terminal environments.

Typical use:
- edit configuration files
- write scripts
- manage notes

---

### ps / top / htop
Used to inspect running processes.

Typical use:
- monitor resource usage
- identify abnormal processes

---

## 6. Package Management Tools

### apt
Used to install and manage software on Linux systems.

Typical use:
- install tools
- update systems
- manage dependencies

---

## 7. Logging and Monitoring Tools

### Event Viewers / Log Files
Used to review system activity.

Typical use:
- investigate incidents
- troubleshoot errors
- analyze security events

---

### SIEM Platforms (High-Level)
Centralize logs and alerts.

Typical use:
- correlate events
- generate alerts
- support investigations

---

## 8. Incident Response Tools (Conceptual)

Common IR tooling includes:
- log analysis tools
- forensic imaging tools
- timeline analysis tools

Purpose:
- preserve evidence
- understand incident scope
- support recovery

---

## 9. Tool Selection Principles

Good tool usage requires:
- understanding the problem
- choosing the right category
- avoiding unnecessary complexity

Tools support skills.
They do not replace understanding.

---

## Key Takeaways

- tools serve specific purposes
- categories help with selection
- networking tools diagnose connectivity
- web tools analyze HTTP behavior
- system tools manage and inspect systems
- logging tools provide visibility
- tools support, not replace, expertise
