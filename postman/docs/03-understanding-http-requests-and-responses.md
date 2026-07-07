# Understanding HTTP Requests and Responses

| Field | Value |
|--------|-------|
| Audience | Beginners with little or no experience working with APIs |
| Document Type | Concept |
| Estimated Reading Time | 6–8 minutes |
| Prerequisites | What is an API? |

---

# Purpose

This guide introduces HTTP requests and responses, the fundamental mechanism through which applications communicate over the web. After reading this guide, you should understand the components of a request, the information contained in a response, and how these concepts relate to using Postman.

---

# What is HTTP?

**Hypertext Transfer Protocol (HTTP)** is a communication protocol that allows clients and servers to exchange information over the internet.

Whenever you open a website, log in to an application, or retrieve information from an online service, HTTP is often the protocol used to send and receive data.

Postman uses HTTP to send requests to APIs and display the responses returned by those APIs.

---

# What is an HTTP request?

An HTTP request is a message sent from a client to a server asking it to perform an action.

Every request contains several pieces of information that tell the server what action should be performed and what data should be returned.

A request typically includes:

- An HTTP method
- A URL (endpoint)
- Headers
- An optional request body

---

# Components of an HTTP request

## HTTP method

The HTTP method specifies the action the client wants to perform.

Some common HTTP methods are:

| Method | Purpose |
|---------|---------|
| GET | Retrieve information |
| POST | Create new information |
| PUT | Replace existing information |
| PATCH | Update part of existing information |
| DELETE | Remove information |

You will use the **GET** method in your first Postman request later in this documentation.

---

## URL (Endpoint)

The URL identifies the location of the API resource.

For example:

```text
https://api.example.com/users
```

In this example:

- `https://` specifies the protocol.
- `api.example.com` identifies the server.
- `/users` identifies the resource being requested.

---

## Headers

Headers provide additional information about the request.

Examples include:

- Authentication credentials
- Content type
- Accepted response format

Many APIs require specific headers before they will process a request.

---

## Request body

Some requests include additional data called the **request body**.

For example, when creating a new user account through an API, the request body might contain:

```json
{
  "name": "Jane Smith",
  "email": "jane@example.com"
}
```

Requests using the **GET** method typically do not include a request body.

---

# What is an HTTP response?

After processing a request, the server returns an HTTP response.

The response tells the client whether the request succeeded and may include additional data.

A response typically contains:

- A status code
- Response headers
- A response body

---

# Status codes

Status codes indicate the outcome of a request.

Some common status codes include:

| Status Code | Meaning |
|-------------|---------|
| 200 OK | The request was successful. |
| 201 Created | A new resource was created successfully. |
| 400 Bad Request | The request was invalid. |
| 401 Unauthorized | Authentication is required or failed. |
| 404 Not Found | The requested resource could not be found. |
| 500 Internal Server Error | The server encountered an unexpected error. |

A more detailed explanation of status codes is provided in the **HTTP Status Codes** reference guide.

---

# Response body

The response body contains the data returned by the server.

Many APIs return information in **JSON (JavaScript Object Notation)** format because it is lightweight and easy for applications to process.

For example:

```json
{
  "id": 42,
  "name": "Jane Smith",
  "email": "jane@example.com"
}
```

When you send requests using Postman, the response body is displayed in the response panel.

---

# The request–response cycle

The interaction between a client and an API follows a predictable sequence.

```text
Client (Postman)
        │
        │ HTTP Request
        ▼
       API
        │
 Processes Request
        │
        ▼
   HTTP Response
        │
        ▼
Client (Postman)
```

As a Postman user, most of your work involves creating requests and examining the responses returned by APIs.

---

# Why this matters in Postman

Every request you create in Postman requires you to specify:

- An HTTP method.
- A URL.
- Optional headers.
- Optional request body.

After sending the request, Postman displays:

- The response status code.
- Response headers.
- Response body.
- Response time.
- Response size.

Understanding these components makes it easier to interpret API behaviour and troubleshoot issues.

---

# Summary

HTTP enables communication between clients and servers.

Every interaction consists of a request sent by the client and a response returned by the server.

Postman provides a graphical interface that allows you to build requests, send them to an API, and inspect every part of the response.

Understanding these concepts will prepare you to send your first API request in the next guide.

---

# Related documentation

- Previous guide: **What is an API?**
- Next guide: **Installing Postman**
