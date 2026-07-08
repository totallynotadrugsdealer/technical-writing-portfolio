---
title: Sending Your First GET Request
description: Learn how to send your first HTTP GET request using Postman Echo.
---

# Sending Your First GET Request

In this guide, you will send your first API request using the Postman Echo service. This exercise introduces the basic workflow for sending requests in Postman and prepares you for the following guides, where you'll learn how to read responses and save requests.

---

# Prerequisites

Before beginning, ensure that you have:

- Installed the Postman desktop application.
- Created and signed in to your Postman account.
- Familiarized yourself with the Postman interface.

---

# What is a GET request?

A **GET** request is an HTTP method used to retrieve information from a server.

Unlike some other HTTP methods, a GET request does **not** modify data on the server. Instead, it requests existing information and returns it to the client.

For this exercise, you will use the **Postman Echo API**, a publicly available API designed for learning and testing. It simply returns information about the request you send, making it an ideal environment for practicing with Postman.

---

# The request you'll send

For this guide, you'll send a request to the following endpoint:

```

https://postman-echo.com/get

```

This endpoint belongs to the Postman Echo service. When it receives your request, it responds with information about the request itself.

You don't need to configure authentication, headers, query parameters, or a request body for this example.

---

# Send your first GET request

1. Open the Postman desktop application.

2. Click the **+** button in the Workbench to open a new request tab.

3. Verify that the HTTP method is set to **GET**.

4. In the request URL field, enter:

```

https://postman-echo.com/get

```

5. Click **Send**.

After a few moments, Postman sends the request to the Postman Echo API and displays the server's response in the lower Response pane.

> **Tip**
>
> If you receive an error, verify that the request URL has been entered correctly and that you have an active internet connection.

---

# Example

![A completed GET request ready to be sent](images/07-first-get-request.png) 

*Figure 1. A completed GET request using the Postman Echo endpoint.*

---

# What happens when you click Send?

When you click **Send**, the following process takes place:

1. Postman sends a GET request to the Postman Echo API.
2. The API server receives and processes the request.
3. The server generates a response.
4. Postman displays the response in the Response pane.

This exchange between the client (Postman) and the server forms the foundation of how APIs communicate.

---

# Verification

Verify that you can:

- Create a new request.
- Select the **GET** HTTP method.
- Enter the request URL.
- Send the request successfully.
- Confirm that a response appears in the Response pane.

If you can complete these steps, you've successfully sent your first API request.

---

# Summary

In this guide, you learned how to send your first GET request using the Postman Echo API.

You should now be able to:

- Understand the purpose of a GET request.
- Create a new request in Postman.
- Send a request to an API endpoint.
- Receive a response from the server.

In the next guide, you'll learn how to interpret the response returned by the API.

---

# References

- Postman Docs – *Postman Quick Start*  
  https://learning.postman.com/docs/getting-started/quick-start

- Postman Docs – *Postman Elements*  
  https://learning.postman.com/docs/getting-started/basics/postman-elements
