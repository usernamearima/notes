# Security Basics

These notes cover fundamental security concepts
that apply across networking, web, systems, cloud,
and enterprise environments.

They focus on understanding security principles,
not exploitation.

---

## 1. What Is Cybersecurity

Cybersecurity is the practice of protecting:
- systems
- networks
- applications
- data

The goal is to prevent:
- unauthorized access
- data breaches
- system abuse
- service disruption

---

## 2. Assets

An asset is anything that has value.

Examples of assets:
- user data
- credentials
- servers
- applications
- source code
- logs

Security exists to protect assets.

---

## 3. Threats

A threat is something that can cause harm.

Examples:
- attackers
- malware
- misconfiguration
- insider misuse
- automation abuse

A threat does not need to be intentional
to cause damage.

---

## 4. Vulnerabilities

A vulnerability is a weakness.

Examples:
- software bugs
- logic flaws
- weak passwords
- missing access controls
- exposed services

Vulnerabilities make threats possible.

---

## 5. Risk

Risk is the combination of:
- asset value
- threat likelihood
- vulnerability impact

High risk exists when:
- valuable assets
- are exposed
- through serious vulnerabilities

Security is about reducing risk,
not eliminating it completely.

---

## 6. Confidentiality, Integrity, Availability (CIA)

### Confidentiality
Data is only accessible to authorized users.

Examples:
- access control
- encryption

---

### Integrity
Data is accurate and not modified improperly.

Examples:
- checksums
- access restrictions

---

### Availability
Systems and data are accessible when needed.

Examples:
- redundancy
- backups
- protection against outages

---

## 7. Defense in Depth

Defense in depth means using multiple security layers.

Examples:
- firewalls
- authentication
- authorization
- logging
- monitoring

If one layer fails,
others still provide protection.

---

## 8. Least Privilege

Least privilege means:
users and systems get only the access they need.

Benefits:
- limits damage
- reduces attack surface
- improves control

Excessive privileges increase risk.

---

## 9. Authentication vs Authorization

### Authentication
Answers:
Who are you?

Examples:
- passwords
- tokens
- certificates

---

### Authorization
Answers:
What are you allowed to do?

Examples:
- role-based access
- permission checks

A user can be authenticated
but not authorized.

---

## 10. Attack Surface

Attack surface is everything that can be attacked.

Examples:
- open ports
- exposed APIs
- login pages
- admin panels

Reducing attack surface improves security.

---

## 11. Logging and Monitoring

Logs record system activity.

Examples:
- login events
- access attempts
- configuration changes

Monitoring analyzes logs to detect:
- anomalies
- attacks
- misuse

Without logs, detection is difficult.

---

## 12. Human Factor

People are part of security.

Common issues:
- weak passwords
- phishing
- mistakes
- misconfiguration

Security is both technical and human.

---

## Key Takeaways

- security protects valuable assets
- threats exploit vulnerabilities
- risk combines impact and likelihood
- CIA defines security goals
- defense in depth reduces failure impact
- least privilege limits damage
- authentication and authorization differ
- logging enables detection
