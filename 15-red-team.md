# Red Team Basics

These notes cover the fundamentals of Red Team operations.
The focus is on mindset, objectives, and methodology,
not on illegal activity or step-by-step exploitation.

All Red Team activities must be authorized and controlled.

---

## 1. What Is a Red Team

A Red Team simulates a real-world attacker.

Goal:
- test an organization’s detection and response
- identify gaps in security controls
- evaluate people, process, and technology

Red Teaming focuses on **outcomes**, not individual bugs.

---

## 2. Red Team vs Pentesting

Pentesting:
- scoped testing
- vulnerability-focused
- time-limited
- mostly technical

Red Team:
- objective-driven
- stealth-focused
- longer engagements
- simulates advanced attackers

Red Teaming is broader and more realistic.

---

## 3. Objectives in Red Team Operations

Objectives define success.

Examples:
- access sensitive data
- reach a specific system
- bypass detection
- demonstrate impact

Finding vulnerabilities alone is not the goal.

---

## 4. Assumed Breach Mindset

Red Teams often assume:
- perimeter defenses will be bypassed
- credentials may be compromised
- some access already exists

This mindset shifts focus to:
- internal security
- detection
- response capability

---

## 5. Attack Paths (Conceptual)

An attack path is a sequence of actions
leading to an objective.

Attack paths may involve:
- misconfigurations
- weak trust relationships
- excessive permissions
- poor monitoring

Understanding attack paths is critical.

---

## 6. Stealth and Evasion (High-Level)

Red Team operations aim to:
- minimize noise
- avoid detection
- blend with normal activity

This tests:
- logging quality
- alerting effectiveness
- analyst awareness

Stealth is about realism, not trickery.

---

## 7. Command and Control (Conceptual)

Command and Control (C2) refers to how attackers:
- maintain access
- communicate with compromised systems

In Red Teaming:
- C2 is simulated safely
- used to test detection and response

C2 behavior is a major detection signal.

---

## 8. Red Team and Blue Team Interaction

Red Team activity helps Blue Teams:
- improve detection
- refine response playbooks
- identify blind spots

Healthy organizations use Red Teaming
as a learning exercise, not a competition.

---

## 9. Rules of Engagement

Red Team engagements must define:
- scope
- allowed techniques
- data handling rules
- safety limits
- emergency stop conditions

Rules protect both the organization and testers.

---

## 10. Reporting and Debriefing

Red Team reports focus on:
- achieved objectives
- attack paths
- detection gaps
- response effectiveness

Debriefings often include:
- lessons learned
- recommendations
- improvement areas

---

## Key Takeaways

- Red Team simulates real attackers
- objectives matter more than bugs
- stealth tests detection capability
- attack paths show real risk
- rules and authorization are critical
- collaboration improves security maturity
