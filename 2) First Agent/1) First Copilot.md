# Create Your First Copilot Chat Agent

## Overview

In this lesson, we create a basic agent in Microsoft Copilot Studio.

The objective is to create a minimum working agent and understand the main components available inside it:

- Topics
- Triggers
- Knowledge
- Responses
- Testing options

---

## Open Microsoft Copilot Studio

Open Microsoft Copilot Studio using the following URL:

```text
https://copilotstudio.microsoft.com
```

Before creating the agent, select the correct Power Platform environment.

Make sure the environment has the required license, such as:

- Microsoft Copilot Studio trial license
- Azure-based Copilot Studio licensing

The correct license ensures that the required Copilot Studio features are available.

---

## Agents and Workflows

Copilot Studio provides options to create:

- Agents
- Workflows

The focus of this lesson is on creating an **agent**.

Workflows will be covered separately.

---

## Create a New Agent

To create an agent:

1. Open Microsoft Copilot Studio.
2. Select the correct environment.
3. Select **Create an agent**.
4. Optionally describe what the agent should do.
5. Create the agent.

The description does not automatically create the complete agent.

Instead, Copilot Studio uses the natural-language description as part of the agent's instructions and logic.

These instructions remain available inside the agent and can be edited later.

For a minimum working agent, the description can be left blank.

---

## Agent Creation Process

Copilot Studio may take some time to create the agent.

Even when no instructions are provided, the platform checks whether there is any information that needs to be analysed and applied.

After the agent is created, Copilot Studio immediately provides an option to test it.

---

## Rename the Agent

The default name of the agent can be changed.

In this example, the agent is created for BananaTech and renamed:

```text
BananaAssist
```

### Steps

1. Select **Edit**.
2. Change the agent name.
3. Optionally add a description.
4. Select **Save**.

---

## Change the Agent Icon

The agent icon can also be changed.

### Icon Requirements

- File format: PNG
- Recommended file size: Less than 72 KB

If the image is larger, Copilot Studio may automatically resize it.

### Steps

1. Select **Edit**.
2. Select **Change icon**.
3. Upload the PNG file.
4. Select **Save**.
5. Refresh the page.

Refreshing the page ensures that the latest agent name, icon, and interface changes are displayed.

---

## Initial Welcome Message

After renaming and refreshing the agent, the default welcome message is updated.

Example:

```text
Hello, I'm BananaAssist. How can I help?
```

The welcome message uses the current name of the agent.

---

## Agent Overview

The agent overview contains several important sections.

### Knowledge

The **Knowledge** section contains the information sources used by the agent.

Knowledge sources can include:

- Files
- Websites
- URLs
- SharePoint content
- Other supported data sources

At this stage, the Knowledge section is empty.

Without organization-specific knowledge, the agent cannot provide accurate company-specific answers.

---

## Tools

Tools allow an agent to perform actions or communicate with external systems.

Tools are not configured in this lesson and will be covered separately.

---

## Connected Agents

An agent can call other agents as part of its logic.

For example, the main `BananaAssist` agent could call another specialized agent to complete a particular task.

At this stage, no additional agents are connected.

---

## Default Topics

A newly created agent already contains several built-in topics.

Examples include:

- Goodbye
- Greetings
- Start over
- Thank you

These topics provide basic conversational behaviour before any custom topics are created.

Additional topics can later be created for scenarios such as:

- Password reset
- Vacation policies
- Office behaviour
- Remote work policies
- Unidentified user requests

---

## Topics, Triggers, and Responses

When a topic is opened, its conversation logic can be viewed.

### Trigger

A trigger determines when a topic should start.

For example, the **Greetings** topic may be activated when the user enters:

```text
Hello
```

The trigger identifies the user's message and activates the appropriate topic.

### Response

The messages displayed inside the topic are the responses sent to the user.

Example:

```text
Hello, I'm BananaAssist. How can I help?
```

A topic can also contain additional actions, such as:

- Asking a question
- Redirecting to another topic
- Calling an action
- Ending the current topic
- Ending the conversation

---

## Configure the Test Panel

Before testing the agent, open the test panel settings using the three-dot menu.

Enable the following options:

```text
Show activity map when testing
Track between topics
```

These options help identify:

- Which topic was activated
- Which trigger was matched
- Which response was displayed
- How the conversation moved between topics

These settings should remain enabled while developing and testing the agent.

---

## Test the Agent

Select **Test** to open the testing panel.

### Test 1: Greeting

Enter:

```text
Hello
```

The activity map shows that:

1. The **Greetings** topic was activated.
2. The greeting trigger was matched.
3. A greeting response was displayed.
4. The topic ended.

This demonstrates the basic conversation flow:

```text
User message
     ↓
Trigger
     ↓
Topic
     ↓
Response
```

---

## Test a General Question

Enter:

```text
How are you doing?
```

The agent may provide a general AI-generated response, such as:

```text
I'm doing great. Thank you for asking. I'm here and ready to assist.
```

This response may not come from a custom topic or an organization-specific knowledge source.

---

## Test the Goodbye Topic

Enter:

```text
Goodbye
```

The agent activates the **Goodbye** topic.

It may ask:

```text
Would you like to end your conversation?
```

The user can confirm the action or choose to continue the conversation.

This demonstrates how built-in topics support basic conversation management.

---

## Test a Knowledge-Based Question

Enter:

```text
How many vacation days do I have?
```

Because no company policy document has been added to the Knowledge section, the agent cannot provide an accurate BananaTech-specific response.

The agent may provide a general answer, but the response will not be based on the organization's actual vacation policy.

This demonstrates why knowledge sources are important.

---

## Existing Capabilities of a New Agent

Even a newly created agent already contains:

- Built-in topics
- Triggers
- Responses
- Basic conversation logic
- General AI capabilities
- A testing interface
- Topic tracking options

Custom knowledge, instructions, tools, and topics can be added later.

---

## Agent Creation Process

```text
Open Copilot Studio
        ↓
Select the correct environment
        ↓
Create a new agent
        ↓
Rename the agent
        ↓
Change the icon
        ↓
Review the built-in topics
        ↓
Enable test tracking options
        ↓
Test the agent
```

---

## Relationship Between Core Components

```text
User asks a question
        ↓
A trigger identifies the intent
        ↓
The appropriate topic is activated
        ↓
The topic runs its conversation logic
        ↓
Knowledge may be used to find information
        ↓
A response is delivered to the user
```

---

## Important Testing Settings

```text
Show activity map when testing: Enabled
Track between topics: Enabled
```

These settings make it easier to follow and understand the agent's conversation logic.

---

## Key Takeaways

- Microsoft Copilot Studio is available at `copilotstudio.microsoft.com`.
- The correct environment and license should be selected before creating an agent.
- Natural-language instructions become part of the agent's editable logic.
- A newly created agent already contains built-in topics.
- Each topic can contain triggers, responses, and conversation actions.
- The activity map shows how the conversation moves through topics.
- Knowledge sources are required for organization-specific answers.
- A basic agent can respond to greetings and general questions.
- Testing should begin early to understand the agent's behaviour.

---
