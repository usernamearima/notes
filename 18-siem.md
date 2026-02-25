# SIEM Basics

These notes cover the fundamentals of Security Information
and Event Management (SIEM).
They focus on how SIEM systems collect, analyze,
and correlate security data.

All content is for learning and legal environments only.

---

## 1. What Is a SIEM

SIEM stands for Security Information and Event Management.

A SIEM system:
- collects logs from many sources
- normalizes data
- correlates events
- generates alerts
- supports investigations

SIEM provides centralized visibility.

---

## 2. Why SIEM Is Used

SIEM is used to:
- detect security incidents
- centralize logs
- correlate events across systems
- support incident response
- meet compliance requirements

Without SIEM, visibility is fragmented.

---

## 3. Log Collection

SIEM collects logs from multiple sources, such as:
- operating systems
- authentication services
- applications
- network devices
- security tools

Logs are usually sent via:
- agents
- syslog
- APIs

---

## 4. Log Normalization

Different systems produce logs in different formats.

Normalization:
- converts logs into a common format
- enables searching and correlation
- improves analysis consistency

Without normalization, correlation is difficult.

---

## 5. Correlation Rules

Correlation rules define suspicious patterns.

Examples:
- multiple failed logins followed by success
- admin login from unusual location
- endpoint alert followed by network activity

Correlation increases detection accuracy.

---

## 6. Alerts in SIEM

Alerts are generated when:
- correlation rules match
- thresholds are exceeded
- anomalies are detected

Good alerts are:
- high-confidence
- actionable
- prioritized

Too many alerts reduce effectiveness.

---

## 7. Dashboards and Visualization

SIEM dashboards provide:
- high-level security overview
- real-time visibility
- trend analysis

Dashboards help analysts:
- monitor activity
- identify anomalies quickly

---

## 8. SIEM and Incident Response

SIEM supports incident response by:
- providing timelines
- linking related events
- storing evidence
- enabling investigations

SIEM is often the starting point
for security investigations.

---

## 9. SIEM Limitations

SIEM is not a silver bullet.

Common limitations:
- high noise levels
- false positives
- complex tuning
- performance costs

SIEM effectiveness depends on configuration.

---

## 10. SIEM Tuning and Maintenance

SIEM requires continuous tuning:
- improving correlation rules
- reducing noise
- updating log sources
- adapting to new threats

A poorly tuned SIEM loses value quickly.

---

## 11. SIEM in Security Operations

SIEM is a core tool for:
- SOC teams
- Blue Teams
- incident responders
- threat hunters

SIEM connects detection, response,
and monitoring workflows.

---

## Key Takeaways

- SIEM centralizes security logs
- log collection and normalization are critical
- correlation improves detection
- alerts must be actionable
- dashboards improve visibility
- SIEM supports incident response
- tuning is continuous and necessary
