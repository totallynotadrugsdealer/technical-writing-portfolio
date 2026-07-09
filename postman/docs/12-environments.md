# Environments

| Field | Value |
|--------|-------|
| Audience | Beginners with little or no experience working with APIs |
| Document Type | Concept |
| Estimated Reading Time | 5–7 minutes |
| Prerequisites | Workspaces |

---

# Purpose

This guide introduces **Postman Environments** and explains how they help you work with different API configurations. By the end of this guide, you will understand what environments are, why they are useful, and how to switch between them.

---

# What is an Environment?

An **Environment** is a named set of variables that Postman uses when sending requests.

Instead of manually changing values such as a server URL, API key, or token every time you work with a different API, you can store those values in an environment and switch between environments whenever needed.

For example, you might have:

- A development environment
- A testing environment
- A production environment

Each environment can contain different values for the same variables.

---

# Why use Environments?

Environments make it easier to work with APIs that have multiple versions or deployments.

Instead of editing every request individually, you simply change the active environment.

For example, you might use:

| Environment | Purpose |
|-------------|---------|
| Development | Testing new features during development |
| Testing | Verifying changes before release |
| Production | Accessing the live API used by end users |

Using environments reduces repetitive work and helps prevent mistakes caused by manually changing request values.

---

# Switching between Environments

The active environment is displayed near the top-right corner of the Postman window.

To switch environments:

1. Click the **Environment** selector.
2. Select the environment you want to use.

Postman immediately begins using the variables stored in the selected environment for any requests that reference them.

![Selecting an environment](../images/environment-selector.png)

*Figure 1. Selecting the active environment.*

> **Image Credit**
>
> Adapted from the Postman Learning Center documentation. Original image © Postman, Inc. Used for educational purposes. :contentReference[oaicite:0]{index=0}

---

# Setting an Environment as Active

You can also activate an environment from the **Environments** section in the sidebar.

1. Open **Environments**.
2. Locate the environment you want to use.
3. Select **Set active**.

![Setting an environment as active](../images/environment-set-active.png)

*Figure 2. Setting an environment as the active environment.*

> **Image Credit**
>
> Adapted from the Postman Learning Center documentation. Original image © Postman, Inc. Used for educational purposes. :contentReference[oaicite:1]{index=1}

---

# When should you use Environments?

Although they are optional, environments become especially useful when:

- Working with multiple servers.
- Switching between development, testing, and production APIs.
- Reusing values across many requests.
- Collaborating with other team members.

For simple learning exercises, such as the Postman Echo API used in previous guides, you typically do not need an environment.

---

# Verification

After reading this guide, you should be able to:

- Explain what a Postman environment is.
- Describe why environments are useful.
- Identify common environment types.
- Switch between environments in Postman.
- Set an environment as the active environment.

---

# Summary

In this guide, you learned that environments allow Postman to use different sets of values for different situations without requiring you to edit every request.

You should now understand that environments:

- Store reusable values.
- Simplify working with multiple APIs or servers.
- Can be switched at any time.
- Help organize API development across different stages such as development, testing, and production.

In the next guide, you will learn how to troubleshoot common problems when working with APIs in Postman.

---

# Related documentation

- Previous guide: **Workspaces**
- Next guide: **Common Errors**
