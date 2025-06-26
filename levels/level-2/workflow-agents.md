# Challenge: Workflow Agents
Use a `SequentialAgent` to create a team of specialized agents that work together.

## Concept
Some problems are best solved as a sequence of steps. You will use a `SequentialAgent` to create a team of specialized agents that work together to solve a problem.

## Task
Build a **research agent** using a `SequentialAgent`. The first agent in the sequence will use the `google_search` tool to gather information on a topic. The second agent will take the collected search results and produce a concise summary. Ask it for example to "Research I/O Connect".

## Outcome
A workflow agent that can answer a research question by first finding relevant web pages and then summarizing the search result snippets.

## Question
The sequential agent is a *workflow agent*. Does the conversation web UI work well for this type of agent?
