# Web Basics – How the Web Works

These notes explain how web applications work at a technical level.
The focus is on understanding communication, not exploiting it.

---

## 1. What Is a Web Application

A web application is software accessed through a web browser.

It usually consists of:
- a client (browser)
- a server (backend)
- communication over HTTP or HTTPS

The browser sends requests.
The server processes them and sends responses.

---

## 2. Client and Server in the Web Context

### Client
The client is usually a web browser.

The client:
- sends HTTP requests
- renders HTML
- executes JavaScript
- displays responses to the user

### Server
The server:
- receives HTTP requests
- processes logic
- accesses databases
- returns responses

The server decides what the client is allowed to see or do.

---

## 3. URL Structure

A URL defines where a request is sent.

Example:
https://example.com/login

Components:
- protocol: `https`
- domain: `example.com`
- path: `/login`

The path usually maps to a specific function or resource on the server.

---

## 4. HTTP Methods

HTTP methods describe the **action** the client wants to perform.

Common methods:
- **GET** – retrieve data
- **POST** – send data (e.g. login form)
- **PUT** – update data
- **DELETE** – remove data

Example meaning:
- GET `/profile` → get profile data
- POST `/login` → send login credentials

---

## 5. HTTP Requests

An HTTP request contains:
- method (GET, POST, etc.)
- path (e.g. /login)
- headers
- optional body

### Request Body
The body often contains user input:
- username
- password
- form data
- JSON data

The server must never trust request data blindly.

---

## 6. HTTP Responses

An HTTP response contains:
- status code
- headers
- response body

The response body may contain:
- HTML
- JSON
- error messages

The browser decides how to display the response.

---

## 7. HTTP Status Codes (Web Perspective)

Common status codes:
- **200** – request successful
- **301 / 302** – redirect
- **401** – unauthorized
- **403** – forbidden
- **404** – resource not found
- **500** – server error

Status codes help debug application behavior.

---

## 8. Headers

Headers are metadata sent with requests and responses.

Examples of request headers:
- User-Agent
- Content-Type
- Cookie

Examples of response headers:
- Set-Cookie
- Content-Type
- Cache-Control

Headers strongly influence application behavior.

---

## 9. Cookies

Cookies are small pieces of data stored in the browser.

Cookies are used for:
- authentication
- session management
- user preferences

A cookie is usually sent:
- from server to client
- then back to the server with each request

Cookies are a core part of web authentication.

---

## 10. Sessions (High-Level)

A session links multiple requests to the same user.

Typical flow:
- user logs in
- server creates a session
- session ID is stored in a cookie
- browser sends the cookie with each request

The server uses the session to recognize the user.

---

## 11. Forms and User Input

Forms allow users to send data to the server.

Common examples:
- login forms
- registration forms
- search fields

Form data is sent via:
- GET (visible in URL)
- POST (sent in request body)

All user input must be validated on the server.

---

## 12. Web Application Logic

The frontend:
- displays content
- may block actions visually

The backend:
- enforces rules
- controls access
- validates permissions

Security must always be enforced on the server side.

---

## Key Takeaways

- the browser sends requests
- the server makes decisions
- HTTP defines communication
- methods describe actions
- headers control behavior
- cookies and sessions identify users
- backend logic is critical for security
