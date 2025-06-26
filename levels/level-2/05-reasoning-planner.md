# Challenge: Reasoning Planner
Use a `PlanReActPlanner` to make an agent that writes down a plan before executing it.

## Concept
For problems that require dynamic planning, you can instruct the agent to write down a plan first, and then execute it, using `PlanReActPlanner`.

## Task
Create a (single, not sequential) research agent that uses the `google_search` tool. Add the `PlanReActPlanner` to this agent to see how it plans its research steps.

## Outcome
When you ask your agent a research question, you will see it outlining its strategy *before* it calls any tools, if the question is sufficiently complex.

## Question
When would a `SequentialAgent` be a better choice than a `PlanReActPlanner`, and vice-versa?
