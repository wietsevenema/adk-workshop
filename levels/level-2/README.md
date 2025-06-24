## Level 2: Building Smarter Agents

**Goal:** Move beyond single-function agents to handle conversational memory, connect to external data, and orchestrate complex tasks.

---
### Challenge: Remembering Things (State)

**Concept:** Agents need memory for multi-turn conversations, and multi-agents use memory to pass information. You will use session state for short-term memory.

**Task:** Create a "Guess the Number" agent that uses session state to remember a secret number across multiple turns. The agent thinks of a random number between 1 and 100. The player has 10 chances to guess the number. After each guess, the computer tells the player if it was too high or too low.

**Outcome:** An agent that can play "Guess the Number" by remembering the secret number between user guesses.

**Question:** One possible solution is to use prompt templates to put the secret number into the agent instructions. Is that a suitable solution for this problem? 

---
### Challenge: Saving Files (Artifacts)

**Concept:** Agents can create and save files, called artifacts. This is useful for generating reports, logs, or other data that needs to persist beyond a single conversation.

**Task:** Modify your "Guess the Number" agent. After the game is won, store a log of all the guesses, and the outcome of the game, to an artifact.

**Outcome:** After winning the game, a `game_log.txt` file appears in the "Artifacts" section of the web UI.

**Question:** What is the key difference between storing data in session state versus saving it as an artifact? When would you choose one over the other?

---
### Challenge: Connecting to the World (External APIs)

**Concept:** Agents become truly powerful when they can interact with external services. You use an OpenAPI specification to interact with an external API.

**Task:** Create a Hacker News agent using the `OpenAPIToolset` to automatically generate tools from an OpenAPI spec. Refer to [the API documentation](https://github.com/HackerNews/API) to get started

**Outcome:** An agent that can answer "What are the top 5 stories on Hacker News right now?" by using the automatically generated tools.

**Question:** What is the main advantage of an `OpenAPIToolset` instead of writing individual functions for every single API endpoint? What are the disadvantages?

---
### Challenge: Workflow Agents

**Concept:** Some problems are best solved as a sequence of steps. You will use a `SequentialAgent` to create a "team" of specialized agents that work together to solve a complex problem.

**Task:** Build a **deep research agent** using a `SequentialAgent`. The first agent in the sequence will use `google_search` and `url_context` tools to gather information on a topic. The second agent will take the collected information and produce a concise summary.

**Outcome:** A workflow agent that can answer a research question by first finding relevant web pages and then summarizing their content.

**Question:** The sequential agent is a *workflow agent*. Does the conversation web UI work well for this type of agent? 

---
### Challenge: Reasoning Planner

**Concept:** For problems that require dynamic planning, you can instruct the agent to write down a plan first, and then execute it, using  `PlanReActPlanner`.

**Task:** Create a deep research agent that uses `google_search` and `url_context` tools. Add the `PlanReActPlanner` to this agent to see how it plans its research steps.

**Outcome:** When you ask your agent a research question, you will see a `/*PLANNING*/` section in the debug logs outlining its strategy *before* it calls any tools.

**Question:** When would a `SequentialAgent` be a better choice than a `PlanReActPlanner`, and vice-versa?
