# Challenge: Managing Cloud Run with a Specialized Toolset
Use a pre-built, complex toolset to manage Google Cloud Run services.

## Concept
Agents can be equipped with sophisticated, domain-specific toolsets that encapsulate complex logic for interacting with external systems. The `MCPToolset` (Multi-Capability-Provisioner Toolset) is an example of such a toolset, providing a high-level interface for managing Google Cloud resources like Cloud Run. This allows you to build powerful, specialized agents without having to implement every low-level API call yourself.

## Task
Your goal is to use the pre-built `cloud-run-mcp-server` agent to interact with your Google Cloud project. Navigate to the `tmp/cloud-run-mcp-server` directory, run the agent using `adk web`, and ask it to list the Cloud Run services in your project.

## Outcome
The agent uses the `MCPToolset` to communicate with the Google Cloud API and returns a list of your active Cloud Run services, demonstrating its ability to manage cloud resources.

## Question
The `MCPToolset` provides powerful capabilities. What are the security considerations when exposing such tools to an LLM, and how might you mitigate them?
