# Challenge: Managing Cloud Run with a Specialized Toolset
Use a pre-built Model Context Protocol (MCP) server to manage Cloud Run services.

## Concept
Agents can be equipped with tools to interact with external systems. You can think of [Model Context Protocol](https://modelcontextprotocol.io/introduction) (MCP) as a standardized way to expose tools to agents. MCP can also be used to expose prompts and resources, but tools are an important feature.  

MCP uses a client-server architecture. From the ADK perspective, the agent is the *client*, and you'll typically start a local MCP *server* to expose tools. There are many MCP servers available for you to run. [Here's an exhaustive list of the official servers](https://github.com/modelcontextprotocol/servers).

In ADK you can use `MCPToolset` to connect to an MCP server.

## Task
Your goal is to use the [Cloud Run MCP server](https://github.com/GoogleCloudPlatform/cloud-run-mcp) to interact with Cloud Run in your Google Cloud project. 

## Outcome
If you run your agent using `adk web`, you can ask it to list the Cloud Run services in your project. 

## Question
MCP servers provide useful capabilities. What are the security considerations when exposing MCP servers to your agent? Consider that you don't control the tool implementation and their descriptions. To help you think about this, consider reading ["The lethal trifecta for AI agents: private data, untrusted content, and external communication"](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/) by Simon Willison.
