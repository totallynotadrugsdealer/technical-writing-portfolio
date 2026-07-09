# Network Errors

| Field | Value |
|--------|-------|
| Audience | Beginners with little or no experience working with APIs |
| Document Type | Troubleshooting |
| Estimated Reading Time | 8–10 minutes |
| Prerequisites | Sending Requests |

---

# Purpose

A network error occurs when Postman cannot successfully communicate with the API server.

Unlike HTTP status codes, network errors usually mean the request never reached the server or the connection failed before a response was received.

This guide explains the most common network errors and how to resolve them.

---

# What Causes Network Errors?

Network errors can occur because of:

- A server that is offline
- An incorrect URL or port
- Firewall or proxy restrictions
- Network connectivity problems
- Slow or unavailable servers
- DNS resolution failures

Most network errors occur before the server returns an HTTP response.

---

# ECONNREFUSED

## Meaning

Postman attempted to connect to a server, but the connection was refused.

This usually means there is no application listening at the specified address.

## Common causes

- Server is not running
- Wrong port number
- Incorrect URL
- Firewall blocking the connection

## How to fix it

Check that:

- the server is running
- the URL is correct
- the port number is correct
- your firewall allows the connection

If you're connecting to **localhost**, ensure the Postman Desktop Agent is running.

---

# ECONNRESET

## Meaning

The server accepted the connection but closed it before completing the request.

## Common causes

- Server restarted
- Server crashed
- Temporary network interruption
- Server overload

## How to fix it

Try the following:

- Wait a few moments and send the request again.
- Verify your network connection.
- Check whether the server is restarting or overloaded.

---

# ETIMEDOUT

## Meaning

The request took too long and timed out before receiving a response.

## Common causes

- Slow server
- Poor network connection
- Proxy delays
- Firewall delays

## How to fix it

Check that:

- your internet connection is stable
- the server is responding normally
- proxy and firewall settings are not delaying requests

---

# DNS Errors

One common DNS-related error is:

```
getaddrinfo ENOTFOUND
```

## Meaning

Postman could not resolve the server's hostname into an IP address.

## Common causes

- Incorrect hostname
- DNS configuration issues
- Proxy configuration problems

## How to fix it

Verify:

- the server address is spelled correctly
- your DNS and proxy configuration
- Postman is updated to the latest version

---

# CORS Errors

CORS (Cross-Origin Resource Sharing) errors occur when a browser blocks a request because the server does not allow requests from that origin.

## How to fix it

If you're using the Postman web app:

- Use the **Postman Desktop Agent**, which is not subject to browser CORS restrictions.

If you manage the API:

- Configure the appropriate `Access-Control-Allow-Origin` headers on the server.

---

# Using the Postman Console

If a network error is unclear, open the **Postman Console**.

The console can help you inspect:

- request details
- connection attempts
- redirects
- request headers
- error messages

The additional information often helps identify where the request failed.

---

# General Troubleshooting Checklist

Before investigating a specific network error, try the following:

- Confirm your internet connection is working.
- Verify the request URL.
- Check that the API server is running.
- Update Postman to the latest version.
- Restart Postman.
- Review your proxy and firewall settings.
- Check the Postman Status page for service interruptions.

---

# Verification

After reading this guide, you should be able to:

- Recognize common Postman network errors.
- Understand what each error indicates.
- Perform basic network troubleshooting.
- Determine whether the issue is with your request, your network, or the server.

---

# Summary

Network errors occur when Postman cannot successfully communicate with the server.

Most issues are caused by unavailable servers, incorrect URLs, DNS failures, firewall restrictions, or network timeouts. Verifying your connection, checking the server status, and reviewing your request configuration will resolve most network problems.

---

# Related documentation

- Previous guide: **Authentication Problems**
- Next guide: **Variables**
