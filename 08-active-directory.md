# Active Directory Basics

These notes cover the fundamentals of Active Directory (AD).
The focus is on understanding structure, roles, and security concepts.
All content is for learning and legal environments only.

---

## 1. What Is Active Directory

Active Directory (AD) is a directory service used by Windows environments.

It is mainly used to:
- manage users
- manage computers
- manage permissions
- manage authentication and authorization

Active Directory is commonly used in corporate and enterprise networks.

---

## 2. Why Active Directory Exists

Without Active Directory:
- each computer would manage users separately
- permissions would be hard to control
- administration would not scale

Active Directory centralizes:
- identity
- access control
- policy enforcement

---

## 3. Domain

A **domain** is the main boundary in Active Directory.

Examples:
- company.local
- corp.example.com

A domain contains:
- users
- computers
- groups
- policies

All domain objects are managed centrally.

---

## 4. Domain Controller (DC)

A Domain Controller is a server that runs Active Directory services.

Responsibilities of a DC:
- authenticating users
- authorizing access
- storing the AD database
- enforcing security policies

If the Domain Controller is compromised,
the entire domain is at risk.

---

## 5. Users and Computers

### Users
Users represent people or services.

User accounts are used to:
- log in to computers
- access resources
- authenticate to services

### Computers
Computer objects represent machines joined to the domain.

When a computer joins a domain:
- it becomes an AD object
- it trusts the Domain Controller

---

## 6. Groups

Groups are used to manage permissions efficiently.

Instead of assigning permissions to users:
- users are added to groups
- permissions are assigned to groups

Common group types:
- Security groups
- Distribution groups

Groups simplify access control.

---

## 7. Organizational Units (OUs)

Organizational Units are containers inside a domain.

OUs are used to:
- organize users and computers
- apply policies
- delegate administration

Example:
- Users OU
- Computers OU
- Admins OU

OUs do NOT create security boundaries,
but they help with management.

---

## 8. Group Policy (GPO)

Group Policy controls configuration and security settings.

GPOs can:
- enforce password policies
- control software installation
- restrict system behavior
- apply security settings

GPOs are applied to:
- users
- computers
- OUs

---

## 9. Authentication in Active Directory

Active Directory uses centralized authentication.

When a user logs in:
- credentials are sent to the Domain Controller
- the DC verifies identity
- access is granted or denied

Common authentication protocols:
- Kerberos
- NTLM (legacy)

---

## 10. Authorization in Active Directory

Authorization defines what a user can access.

After authentication:
- group memberships are evaluated
- permissions are checked
- access is granted or denied

Authentication = who you are  
Authorization = what you can do

---

## 11. Trust Relationships (High-Level)

Domains can trust each other.

Trusts allow:
- users from one domain to access resources in another
- larger enterprise structures

Trusts increase complexity and attack surface.

---

## 12. Why Active Directory Is a Security Target

Active Directory is critical because:
- it controls identity
- it controls access
- it controls policy

If AD is compromised:
- attackers gain broad access
- detection becomes difficult
- recovery is complex

Protecting AD is a top security priority.

---

## Key Takeaways

- Active Directory centralizes identity and access
- the domain is the core security boundary
- Domain Controllers are critical assets
- groups simplify permission management
- GPOs enforce security policies
- authentication and authorization are separate
- AD compromise affects the entire organization
