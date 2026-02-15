# API Security Basics

These notes explain how APIs work and what security concepts
are critical when protecting APIs.
The focus is on understanding logic and design,
not exploitation.

All content is for learning and legal labs only.

---

## 1. What Is an API

An API (Application Programming Interface) allows applications
to communicate with each other.

Instead of a browser talking to a server,
another program talks to the server.

Examples of API clients:
- web frontend (JavaScript)
- mobile applications
- other servers
- automation scripts

APIs usually communicate using HTTP or HTTPS.

---

## 2. API Requests and Responses

API communication is based on requests and responses,
just like normal web traffic.

A typical API request contains:
- HTTP method (GET, POST, PUT, DELETE)
- endpoint (e.g. /api/users)
- headers
- optional body (often JSON)

A typical API response contains:
- status code
- headers
- response body (usually JSON)

APIs are often designed to return data, not HTML.

---

## 3. REST APIs (High-Level)

Most modern APIs are REST-based.

REST APIs typically use:
- GET → retrieve data
- POST → create data
- PUT / PATCH → update data
- DELETE → remove data

Example:
- GET /api/users
- POST /api/login
- DELETE /api/orders/123

The HTTP method describes the action.

---

## 4. Authentication in APIs

APIs must identify who is making the request.

Common API authentication methods:
- API keys
- tokens (e.g. Bearer tokens)
- session cookies

Authentication answers:
**Who is the client?**

If authentication fails:
- the API should reject the request

---

## 5. Authorization in APIs

Authorization defines what an authenticated client is allowed to do.

Examples:
- can this user access this endpoint?
- can this user modify this resource?
- can this user access admin APIs?

An API can authenticate a user
but still fail at authorization.

---

## 6. Broken Object Level Authorization (BOLA)

BOLA is a common API security issue.

It happens when:
- API uses object IDs (e.g. userId, orderId)
- API does not verify ownership
- users can access other users' data

Example:
```text
GET /api/users/123
GET /api/users/124

If access is not properly checked,
data leakage occurs.
```
---

## 7. Excessive Data Exposure

APIs often return more data than needed.

Examples:
internal IDs
email addresses
role information
debug fields
Even if the user is authorized,
exposing unnecessary data increases risk.

APIs should return only what the client needs.

---

## 8. Missing Rate Limiting

APIs should limit how often clients can send requests.

Without rate limiting:
brute-force attempts are easier
abuse is harder to detect
resources can be exhausted
Rate limiting is a basic API protection mechanism.

---

## 9. Trust Boundaries in APIs

APIs must not trust:
client-side validation
frontend restrictions
request structure

Any client can:
modify requests
replay requests
automate requests

All security checks must be enforced by the API backend.

---

## 10. Error Handling in APIs

API error messages should be clear but not verbose.

Bad practice:
exposing stack traces
exposing internal logic
exposing database details

Good practice:
generic error messages
proper HTTP status codes

---

Key Takeaways
APIs are used by programs, not humans
API security relies on backend logic
authentication and authorization are separate
object-level authorization is critical
APIs should expose minimal data
trust boundaries must be enforced server-side
