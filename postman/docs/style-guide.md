# Style Guide

## Purpose

This style guide defines the writing standards used throughout the Postman documentation project.

The objective is to create documentation that is clear, accurate, consistent, and easy for beginners to follow. These standards help ensure that every document provides a predictable and user-focused experience.

---

# Audience

This documentation is intended for users with little or no prior experience working with APIs or Postman.

Assume the reader:

- Can comfortably use a computer.
- Has never worked with API development tools.
- Is unfamiliar with technical terminology unless explained.

---

# Writing Principles

Follow these principles throughout the documentation.

- Put the user's task before technical detail.
- Explain unfamiliar concepts before using them.
- Write one topic per document.
- Keep instructions concise.
- Prioritize clarity over completeness.
- Test every documented procedure before publishing.

---

# Voice and Tone

## Voice

Professional, approachable, and instructional.

## Tone

Friendly and encouraging without being conversational.

Avoid:

- jokes
- slang
- unnecessary marketing language
- unnecessary technical jargon

---

# Point of View

Write from the second-person point of view.

✔ You can create a new collection.

✘ The user can create a new collection.

---

# Tense

Use present tense whenever possible.

✔ Postman stores requests in Collections.

✘ Postman will store requests in Collections.

---

# Headings

Use sentence case for all headings.

Headings should clearly describe the task or concept.

Good

- Install Postman
- Send your first request
- Understanding Collections

Avoid generic headings such as:

- Tutorial
- Guide
- Information

---

# Procedures

Write procedures as numbered steps.

Begin each step with an imperative verb.

Each step should describe only one action.

Good

1. Open Postman.
2. Select **New**.
3. Choose **HTTP Request**.

Poor

1. Open Postman and create a request before checking the response and saving it.

Whenever appropriate, include the following sections:

- Prerequisites
- Procedure
- Verification
- Troubleshooting
- Next steps

---

# Lists

Use numbered lists for sequential tasks.

Use bulleted lists for related information that does not require a specific order.

Keep list items concise.

---

# User interface conventions

Use bold formatting for interface elements.

Examples

Select **Send**.

Open **Collections**.

Choose **Create Workspace**.

Use the exact product terminology that appears in the Postman interface.

---

# Screenshots

Use screenshots only when they improve understanding.

Screenshots should:

- show only the relevant interface
- avoid unnecessary browser tabs or desktop elements
- remain consistent in size whenever possible
- be updated whenever the interface changes

Whenever possible, crop screenshots to focus attention on the relevant action.

---

# Code samples

Keep code samples short.

Include only the code necessary to demonstrate the concept.

Whenever possible:

- explain what the code does
- identify placeholders
- specify the programming language

Example

```bash
curl https://api.example.com/users
```

---

# Terminology

Use official Postman terminology consistently throughout the documentation.

Examples include:

- Postman
- Collection
- Workspace
- Environment
- Request
- Response
- API
- Endpoint
- HTTP Method

Avoid inventing alternative names for existing product features.

Explain technical terms the first time they appear.

---

# Word Choice

Prefer plain language.

Use familiar words whenever possible.

Write:

- for example

Instead of:

- e.g.

Write:

- that is

Instead of:

- i.e.

Avoid unnecessary abbreviations unless they are commonly understood by the intended audience.

---

# Cross-references

Where appropriate, link readers to related documentation instead of repeating information.

For example:

See **Understanding Collections** before creating your first collection.

---

# Review Checklist

Before publishing documentation, confirm that:

- The documented procedure has been tested.
- Every step is accurate.
- Product terminology is used consistently.
- Technical terms are explained when first introduced.
- Screenshots match the current interface.
- Headings are descriptive.
- Grammar and spelling have been reviewed.
- The document follows this style guide.

---

# Document Metadata

Every documentation page should include:

- Title
- Purpose
- Intended audience (when necessary)
- Prerequisites (for procedural topics)
- Related documentation (when applicable)
- Last updated date (optional for this portfolio)
✔ Postman stores requests in Collections.

✘ Postman will store requests in Collections.

---

## Headings

Use sentence case for all headings.

Headings should describe the action or concept rather than being overly general.

✔ Create your first request

✔ Understanding Collections

✘ Tutorial

✘ Guide

✘ Examples

---

## Procedures

Write instructions as numbered steps.

Begin each step with an imperative verb.

Each step should describe one action only.

✔ 1. Select **Send**.

✔ 2. Review the response body.

✘ Click Send and then look at the response while making sure everything works.

---

# User Interface Elements

Use bold formatting for buttons, menu items, and interface labels.

Example:

Select **Send**.

Open **Collections**.

---

# Notes

Use blockquotes.

> Note:
> You must be connected to the internet to sign in.

---

# Screenshots

Include screenshots only when they clarify an action or interface.

Avoid screenshots that contain unnecessary UI elements.

---

# Code

Use fenced code blocks.

Specify the language whenever possible.

---

# Terminology

Use terms consistently.

Always capitalize:

- Postman
- Collection
- Workspace
- Environment

Avoid abbreviations unless previously explained.
