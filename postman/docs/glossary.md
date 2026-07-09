# Glossary

| Field | Value |
|--------|-------|
| Audience | Beginners with little or no experience working with APIs |
| Document Type | Reference |
| Estimated Reading Time | 8–10 minutes |
| Prerequisites | None |

---

# Purpose

This glossary provides definitions for common API and Postman terminology used throughout this guide.

Use it as a quick reference whenever you encounter an unfamiliar term.

---

# API

**Application Programming Interface (API)**

A set of rules that allows different software applications to communicate with one another.

An API enables one application to request information or services from another application.

---

# API Endpoint

A specific URL where an API accepts requests.

Example:

```
https://postman-echo.com/get
```

---

# Authorization

The process of verifying whether a client has permission to access a resource.

Many APIs require an API key, OAuth token, or other credentials before responding.

---

# Body

The main content of an HTTP request or response.

For example, a response body may contain JSON data returned by an API.

---

# Collection

A group of related API requests saved together in Postman.

Collections help organize requests into reusable workflows.

---

# Endpoint

See **API Endpoint**.

---

# Environment

A named set of variables used to switch between different API configurations, such as development, testing, or production.

---

# GET

An HTTP method used to retrieve information from a server.

A GET request does not modify data.

---

# Header

A key-value pair sent with an HTTP request or response that provides additional information.

Examples include:

- `Content-Type`
- `Authorization`
- `Accept`

---

# HTTP

**Hypertext Transfer Protocol**

The standard protocol used for communication between clients and web servers.

APIs commonly use HTTP to exchange requests and responses.

---

# HTTP Method

The action a client wants the server to perform.

Common HTTP methods include:

- GET
- POST
- PUT
- PATCH
- DELETE

---

# JSON

**JavaScript Object Notation**

A lightweight format used to exchange structured data between applications.

Most modern APIs send responses in JSON format.

Example:

```json
{
  "name": "Alice",
  "city": "Delhi"
}
```

---

# Parameter

Additional information sent with a request.

Parameters help specify exactly what data an API should return.

---

# Path Parameter

A parameter included as part of the URL path.

Example:

```
/users/123
```

where `123` identifies a specific user.

---

# Query Parameter

A parameter appended to the end of a URL after a question mark (`?`).

Example:

```
https://example.com/users?page=2
```

Here, `page=2` is a query parameter.

---

# Request

A message sent from a client to a server asking it to perform an action.

Every request includes an HTTP method and a URL.

---

# Response

The message returned by a server after processing a request.

A response usually includes:

- Status code
- Headers
- Response body

---

# Response Body

The data returned by the server.

It commonly contains JSON representing the requested information.

---

# Status Code

A three-digit HTTP number indicating the outcome of a request.

Examples include:

- 200 OK
- 201 Created
- 400 Bad Request
- 401 Unauthorized
- 404 Not Found
- 500 Internal Server Error

---

# URL

**Uniform Resource Locator**

The web address used to identify an API endpoint.

Example:

```
https://postman-echo.com/get
```

---

# Variable

A named value that can be reused throughout Postman requests.

Variables make it easier to switch between environments without editing every request.

---

# Workspace

A collaborative area in Postman where collections, environments, APIs, and other resources are organized.

Workspaces can be personal or shared with a team.

---

# Related documentation

- Previous guide: **Network Errors**
- Next guide: **Keyboard Shortcuts**
