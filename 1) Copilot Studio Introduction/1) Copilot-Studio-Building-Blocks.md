# Four Building Blocks of a Copilot Chatbot

## Overview

A Copilot chatbot is built around four core elements:

1. Topics
2. Triggers
3. Knowledge
4. Responses

These elements work together to understand a user's question, identify the correct conversation path, find relevant information, and provide an answer.

---

## 1. Topics

A **topic** is a container of conversation logic that handles a specific type of request.

It is similar to the subject of a normal conversation. Each topic focuses on a particular context or business scenario.

### Examples of Topics

- Password reset
- Vacation policies
- Office behaviour
- Remote work
- General enquiries

### Example

**User question:**

> How many vacation days do I have?

This question should be handled by the **Vacation Policies** topic.

**User question:**

> What is my password?

This question should be handled by the **Password Reset** topic.

### Key Point

Topics organize chatbot conversations into separate logical areas.

---

## 2. Triggers

A **trigger** identifies what the user is asking and decides which topic should handle the conversation.

Triggers can include specific phrases, questions, or similar natural-language expressions.

### Vacation Policy Trigger Examples

- How many vacation days do I have?
- What is the vacation policy?
- How much time off do I get?
- Can I take next week off?

These questions can activate the **Vacation Policies** topic.

### Password Reset Trigger Examples

- Reset password
- What is my password?
- I forgot my password
- Help me change my password

These questions can activate the **Password Reset** topic.

### Key Point

Triggers detect the user's intent and route the conversation to the correct topic.

---

## 3. Knowledge

**Knowledge** contains the information that Copilot uses to answer user questions.

The chatbot does not automatically know an organization's internal policies. Relevant knowledge sources must be added or connected.

### Example Knowledge Sources

For the Banana Tech Solutions chatbot, the knowledge sources include:

- Employee Benefits Policy
- Employee Conduct Policy
- IT Support Guidelines
- Remote Work Policy

### Example

A question about vacation entitlement may use information from the **Employee Benefits Policy**.

A password-related question may use information from the **IT Support Guidelines**.

### Key Point

Knowledge provides the information required to generate accurate and relevant answers.

---

## 4. Responses

A **response** is the answer delivered by Copilot to the user.

Responses are usually generated within a topic and may use information retrieved from connected knowledge sources.

### Example 1

**User question:**

> How many vacation days do I have?

**Response:**

> Full-time employees receive 17.5 vacation days per year.

### Example 2

**User question:**

> I forgot my password. What should I do?

**Response:**

> Go to the IT portal and submit a password reset request.

### Key Point

Responses communicate the final answer or guidance to the user.

---

## How the Four Building Blocks Work Together

The typical conversation flow is:

```text
User Question
     ↓
Trigger identifies the user's intent
     ↓
The correct Topic is activated
     ↓
The Topic uses the available Knowledge
     ↓
A Response is delivered to the user
