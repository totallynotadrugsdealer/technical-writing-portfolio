# Reading the Response

| Field | Value |
|--------|-------|
| Audience | Beginners with little or no experience working with APIs |
| Document Type | Concept |
| Estimated Reading Time | 4–6 minutes |
| Prerequisites | Sending Your First GET Request |

---

# Purpose

This guide explains how to read and understand the information returned after sending an API request in Postman. By the end of this guide, you will be able to identify the different parts of the response viewer and understand what each section tells you about your request.

---

# Prerequisites

Before you begin, ensure that you have:

- Installed the Postman desktop application.
- Created and signed in to your Postman account.
- Successfully sent your first GET request using the Postman Echo API.

---

# Understanding the Response Viewer

After you click **Send**, Postman displays the server's response in the **Response Viewer**, located in the lower half of the request tab.

The Response Viewer helps you determine whether your request was successful and allows you to inspect the data returned by the server.

![Response Viewer](../images/response-viewer-overview.png)

*Figure 1. The Postman Response Viewer showing the response body, status code, response time, response size, and response tabs.*

> **Image Credit**
>
> Adapted from the Postman Learning Center documentation. Original image © Postman, Inc. Used for educational purposes.

---

# Understanding the Response Body

The **Body** tab contains the data returned by the API.

For the Postman Echo endpoint, the response is returned in **JSON (JavaScript Object Notation)** format. Postman automatically formats the response with indentation and syntax highlighting, making it easier to read.

A typical response looks similar to the following:

```json
{
  "args": {},
  "headers": {
    "host": "postman-echo.com"
  },
  "url": "https://postman-echo.com/get"
}
```

Every API returns different information, but the response body is where you'll usually find the data requested from the server.

---

# Understanding the Status Code

Above the response body, Postman displays the **HTTP status code**.

For a successful request, you should see:

```
200 OK
```

The status code indicates whether the request was processed successfully.

Some common HTTP status codes are shown below.

| Status Code | Meaning |
|-------------|---------|
| **200 OK** | The request completed successfully. |
| **400 Bad Request** | The request was invalid or incorrectly formatted. |
| **401 Unauthorized** | Authentication is required or has failed. |
| **403 Forbidden** | You do not have permission to access the requested resource. |
| **404 Not Found** | The requested resource could not be found. |
| **500 Internal Server Error** | The server encountered an unexpected error while processing the request. |

Checking the status code should always be your first step when troubleshooting an API request.

---

# Understanding Response Time

Next to the status code, Postman displays the **response time**.

Example:

```
208 ms
```

Response time indicates how long the server took to process your request and return a response.

Although faster responses generally indicate better performance, acceptable response times depend on the API and the operation being performed.

---

# Understanding Response Size

Postman also displays the **response size**.

Example:

```
1.26 KB
```

This indicates how much data was returned by the server.

Larger responses usually contain more information and therefore require more data to be transferred between the server and your computer.

---

# Understanding the Response Tabs

The Response Viewer includes several tabs that organise different parts of the server's response.

| Tab | Description |
|------|-------------|
| **Body** | Displays the data returned by the API. |
| **Headers** | Displays metadata returned by the server as key-value pairs. |
| **Cookies** | Displays any cookies returned by the server. |

For now, you'll spend most of your time working with the **Body** tab.

As you begin working with authenticated APIs and more complex requests, the **Headers** and **Cookies** tabs will become increasingly useful.

> **Tip**
>
> When an API request doesn't behave as expected, begin by checking the **status code** and the **response body**. Together, they usually provide enough information to understand what happened.

---

# Verification

Verify that you can successfully:

- Locate the Response Viewer after sending a request.
- Identify the response body.
- Find the HTTP status code.
- Locate the response time.
- Locate the response size.
- Switch between the **Body**, **Headers**, and **Cookies** tabs.

If you can complete these steps, you can confidently read the basic information returned by an API request in Postman.

---

# Summary

In this guide, you learned how to interpret the information displayed in Postman's Response Viewer.

You should now be able to:

- Identify the response body.
- Interpret common HTTP status codes.
- Understand response time and response size.
- Recognise the purpose of the Body, Headers, and Cookies tabs.

In the next guide, you will learn how to save requests so that you can organise and reuse them in future sessions.

---

# Related documentation

- Previous guide: **Sending Your First GET Request**
- Next guide: **Saving a Request**
