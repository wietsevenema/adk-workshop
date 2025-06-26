# Challenge: From Prompt to Deployed App
Deploy a prompt as a serverless web app with its own endpoint.

## Concept
A well-crafted prompt can be a complete application. [Vertex AI Studio](https://console.cloud.google.com/vertex-ai/generative/language) (the enterprise-grade version of AI Studio) can instantly deploy a prompt as a serverless web app with a web UI and its own endpoint.

## Task
Your goal is to create a simple translation service. In Vertex AI Studio, create a prompt that translates English text to German. Use a *prompt variable* for the text component. Use the "Build with code" > "Deploy as app" button to create a callable API endpoint for your translator.

## Outcome
You will have a live, public API endpoint that takes English text and returns its German translation.

## Question
How would you modify the prompt to ensure the translation uses a certain style?
