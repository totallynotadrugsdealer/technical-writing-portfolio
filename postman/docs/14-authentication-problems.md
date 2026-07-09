# Authentication Problems

| Field | Value |
|--------|-------|
| Audience | Beginners with little or no experience working with APIs |
| Document Type | Troubleshooting |
| Estimated Reading Time | 8–10 minutes |
| Prerequisites | Requests, Responses, Environments |

---

# Purpose

Authentication is one of the most common reasons an API request fails.

This guide explains how to identify authentication-related errors and the steps you can take to resolve them in Postman.

---

# What Is Authentication?

Authentication is the process of proving your identity to an API.

Many APIs require credentials before allowing access to protected resources.

Common authentication methods include:

- API Keys
- Bearer Tokens
- Basic Authentication
- OAuth 2.0

If authentication is missing or incorrect, the API usually returns an error instead of the requested data.

---

# Common Authentication Errors

## 401 Unauthorized

### Meaning

Your request was received, but the server could not verify your identity.

### Common causes

- Missing API key
- Invalid API key
- Expired access token
- Incorrect username or password
- Wrong authentication type

### How to fix it

Check that:

- the request URL is correct
- the selected authorization type matches the API documentation
- the API key or token is valid
- credentials have been entered correctly

---

## 403 Forbidden

### Meaning

The server recognizes who you are but refuses to grant access.

### Common causes

- Your account lacks permission.
- The API key doesn't have sufficient privileges.
- The requested resource isn't accessible to your account.

### How to fix it

Verify that:

- your account has permission to access the resource
- your API key includes the required scopes or permissions
- you're using the correct credentials

---

# Verify Your Authorization Settings

When troubleshooting authentication:

1. Open the **Authorization** tab.
2. Confirm the correct authentication type is selected.
3. Verify that all required credentials are present.
4. Save the changes.
5. Send the request again.

Even a small mistake—such as an extra space or an expired token—can cause authentication to fail.

---

# Check Environment Variables

Many collections store credentials in environment variables.

For example:

```
{{apiKey}}
```

or

```
{{accessToken}}
```

If the variable has no value, Postman sends an empty credential.

### Verify that

- the correct environment is selected
- required variables contain values
- variable names match those used in the request

---

# Using the Postman Console

The Postman Console helps you inspect what was actually sent.

It can show:

- request headers
- resolved variable values
- redirects
- request details

If authentication appears correct but the request still fails, checking the console can help identify missing or incorrect credentials.

---

# Authentication Troubleshooting Checklist

If a request returns **401 Unauthorized** or **403 Forbidden**, check the following:

- Is the request URL correct?
- Is the correct authorization type selected?
- Is the API key or access token valid?
- Has the token expired?
- Is the correct environment selected?
- Are all required variables populated?
- Does your account have permission to access the resource?

---

# Security Best Practices

When working with credentials:

- Never share API keys or access tokens.
- Store sensitive values in environments instead of directly in requests.
- Use HTTPS whenever possible to protect credentials during transmission.
- Remove expired or unused credentials.

---

# Verification

After reading this guide, you should be able to:

- Understand common authentication errors.
- Distinguish between **401 Unauthorized** and **403 Forbidden**.
- Verify authentication settings in Postman.
- Troubleshoot missing or invalid credentials.

---

# Summary

Authentication errors usually occur because credentials are missing, invalid, expired, or incorrectly configured.

When a request fails, verify the authentication type, confirm your credentials, check your environment variables, and inspect the request in the Postman Console. Following these steps resolves most authentication problems quickly.

---

# Related documentation

- Previous guide: **Common Errors**
- Next guide: **Variables**
