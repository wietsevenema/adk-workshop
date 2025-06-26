# Challenge: Remembering Things (State)
Use session state for short-term memory in a multi-turn conversation.

## Concept
Agents need memory for multi-turn conversations, and multi-agents use memory to pass information. You will use session state for short-term memory.

## Task
Create a "Guess the Number" agent that uses session state to remember a secret number across multiple turns. The agent thinks of a random number between 1 and 100. The player has 10 chances to guess the number. After each guess, the computer tells the player if it was too high or too low.

## Outcome
An agent that can play "Guess the Number" by remembering the secret number between user guesses.

## Question
One possible solution is to use prompt templates to put the secret number into the agent instructions. Is that a suitable solution for this problem?
