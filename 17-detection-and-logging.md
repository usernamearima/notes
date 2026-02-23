# Detection and Logging Basics

These notes cover the fundamentals of detection and logging.
They explain how security teams gain visibility into systems
and identify suspicious or malicious activity.

All content is for learning and legal environments only.

---

## 1. What Is Detection

Detection is the process of identifying suspicious
or malicious activity in systems and networks.

Detection answers the question:
**How do we know something bad is happening?**

Detection relies on visibility and data.

---

## 2. What Is Logging

Logging is the process of recording events.

Logs capture:
- user actions
- system events
- errors
- security-relevant activity

Without logs, detection is not possible.

---

## 3. Why Logging Is Critical for Security

Logs are used to:
- detect attacks
- investigate incidents
- understand attacker behavior
- support compliance

If activity is not logged,
it cannot be analyzed later.

---

## 4. Common Log Sources

Typical sources of logs include:
- operating systems (Windows, Linux)
- authentication systems
- applications
- web servers
- databases
- network devices
- security tools

Each source provides a different view of activity.

---

## 5. Authentication and Authorization Logs

Important security events include:
- successful logins
- failed logins
- privilege changes
- access to sensitive resources

These logs help detect:
- brute-force attempts
- credential abuse
- unauthorized access

---

## 6. Network Logs

Network logs provide visibility into traffic.

Examples:
- firewall logs
- proxy logs
- DNS logs
- VPN logs

Network logs help identify:
- unusual connections
- data exfiltration
- command-and-control traffic

---

## 7. Endpoint Logs

Endpoints include:
- workstations
- servers

Endpoint logs may include:
- process creation
- file changes
- registry changes
- service activity

Endpoint visibility is critical
for detecting post-compromise activity.

---

## 8. Detection Methods (High-Level)

### Signature-Based Detection
- looks for known patterns
- effective for known threats
- weak against new attacks

---

### Behavior-Based Detection
- looks for unusual behavior
- can detect unknown threats
- may produce false positives

Effective detection often combines both.

---

## 9. Alerts

Alerts are generated when:
- a detection rule matches
- behavior exceeds a threshold
- anomalies are identified

Alerts must be:
- actionable
- prioritized
- understandable

Too many alerts lead to alert fatigue.

---

## 10. False Positives and False Negatives

### False Positive
- alert triggers for benign activity

### False Negative
- malicious activity is missed

Detection tuning aims to:
- reduce false positives
- minimize false negatives

Perfect detection does not exist.

---

## 11. Correlation

Correlation links multiple events together.

Examples:
- login failure followed by success
- process execution after email open
- network connection after privilege escalation

Correlation improves detection accuracy.

---

## 12. Detection Gaps

Detection gaps occur when:
- activity is not logged
- logs are not collected
- rules do not exist
- alerts are ignored

Identifying gaps is critical for improvement.

---

## 13. Detection in the Security Lifecycle

Detection supports:
- incident response
- threat hunting
- continuous improvement

Detection is not a one-time setup.
It evolves with threats.

---

## Key Takeaways

- detection identifies malicious activity
- logging provides visibility
- multiple log sources are required
- authentication and network logs are critical
- alerts must be actionable
- false positives and negatives are unavoidable
- correlation improves detection
- detection is a continuous process
