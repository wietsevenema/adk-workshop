## Level 1: ADK Fundamentals

This level covers the basics of building an AI agent. You will learn how to create an agent that can use tools to interact with its environment, and deploy it to an HTTPS endpoint. 

---
### Challenge: Local Setup & "Hello, Agent\!"

**Concept:** The first step is to set up your local development environment and run the basic, pre-generated agent to understand the core workflow.

**Task:** Use `adk create` to generate agent source code and `adk web` to launch the local web UI.

**Outcome:** You have the ADK web UI running on your machine, allowing you to chat with your first, simple agent.

**Question:** The `adk web` command starts a server. Explore the UI and find out what all the tabs do. 

---
### Challenge: Your First Tool

**Concept:** The core power of an agent lies in its ability to use tools (Python functions) to perform actions and interact with the world. You will define a tool using a standard Python function and register it with your agent.

**Task:** Create a simple Python function that accepts a number of sides, `roll_dice(sides: int)`, and add it to the `tools` list of your `Agent`. Test it in the web UI.

**Outcome:** The agent will call your Python function and reply with its result. You will see the function call and response in the debug logs.

**Question:** The description of a tool is very important for getting good results. Can you explain why? 

---
### Challenge: Your First Cloud Deployment

**Concept:** Make your agent accessible to the world by deploying it as a web app on Cloud Run.

**Task:** Use the `adk deploy cloud_run` command to deploy the tool-using agent from the previous challenge.

**Outcome:** You will have a public URL that serves the same ADK web UI and agent you just built.

**Question:** Does it make sense to deploy the ADK web UI to a production endpoint? How would you integrate ADK into your application? 
