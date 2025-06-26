# Challenge: Your First Tool
Define a tool and register it with your agent.

## Concept
As powerful as they are, LLMs used in *isolation* have some key limitations. For example, their knowledge is frozen at the time they were trained - and they cannot interact directly with the outside world.

A key development that enables a more dynamic approach is 'tool calling'. Here's how it works:

*   With each prompt, you provide the LLM with a list of available tools and their descriptions.
*   The LLM uses these descriptions to decide which tool (if any) can help fulfill the prompt.
*   Instead of running the tool itself, the LLM generates a structured output that specifies which tool it wants to use and what information to pass to it.
*   Your application code receives this output, executes the actual tool, and sends the result back to the LLM.
*   The LLM then uses the tool's output to generate its final response to you.

## Task
Create a simple Python function that accepts a number of sides, `roll_dice(sides: int)`, and add it to the `tools` list of your `Agent`. Test it in the web UI.

## Outcome
The agent will call your Python function and reply with its result. You will see the function call and response in the web UI.

## Question
The description of a tool is very important for getting good results. Can you explain why? What are common failure modes with tool descriptions?
