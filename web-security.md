# Web Security Basics

These notes focus on common web security concepts and logic flaws.
The goal is to understand how and why security issues happen,
not how to exploit them.

All examples are for theory and legal labs only.

---

## 1. Authentication vs Authorization

### Authentication
Authentication answers the question:
**Who are you?**

Examples:
- login with username and password
- login with token
- login with session cookie

If authentication fails:
- the user should not be logged in

---

### Authorization
Authorization answers the question:
**What are you allowed to do?**

Examples:
- can you view this page?
- can you edit this resource?
- can you access admin functionality?

A user can be authenticated but NOT authorized.

---

## 2. Broken Access Control

Broken Access Control happens when
a user can perform actions they should not be allowed to perform.

---

### Simple Example

- user is logged in as a normal user
- URL is changed:
  `/user/123` → `/user/124`
- another user's data is visible

This means access control is broken.

---

### Other Common Examples

- accessing `/admin` as a normal user
- deleting other users' posts
- changing another user's password
- frontend blocks action, backend does not

---

### Important Rule

This is NOT a frontend or UI bug.
This is a **server-side logic bug**.

The backend must enforce permissions.

---

## 3. Why Frontend Security Is Not Enough

The frontend:
- controls what buttons are visible
- may block actions in the UI

But:
- frontend code runs on the user's device
- users can modify requests
- tools can bypass UI restrictions

Only the backend can enforce security.

---

## 4. How Proper Access Control Should Work

For every sensitive request, the server should check:
- who the user is
- what role the user has
- what the user is allowed to do

The server should NOT rely only on:
- the user being logged in

---

## 5. ID-Based Access Issues

Many applications use IDs in URLs or requests.

Example:
```text
/user/123
/order/456

If the server does not verify ownership:
users may access other users' data

This is a common source of access control issues.

---

## 6. Testing Access Control (Conceptual, Legal)

Access control testing focuses on logic, not exploitation.

Typical ideas:
change IDs in requests
access restricted endpoints
repeat requests as different users
observe server responses

If the server responds successfully
when it should block access,
there is a logic flaw.

---

## 7. Security Responsibility

Security responsibilities:
frontend → user experience
backend → security enforcement
All authorization decisions must happen on the server.

Key Takeaways
authentication = who you are
authorization = what you can do
being logged in is not enough
frontend controls are not security
broken access control is a server-side logic issue
