# Workshop: Building AI Agents with Google's Agent Development Kit (ADK)

Welcome\! This workshop is designed to take you from the basics of agent development to building and deploying robust, intelligent AI agents on Google Cloud. Here’s what I expect you to do:

* **Choose a buddy**: to do the challenges with (you’re faster together and learn more)   
* **Relax and learn**: Don’t do every challenge. Pick what looks interesting. If you start one and can’t finish it, don’t feel bad — if you like it, you can continue at home. If you finish one, that’s amazing\!   
* **Pick any challenge**: You can skip levels and there’s no requirement to start at the beginning.   
* **Don’t be stuck:** If you struggle for more than 20 seconds, raise your hand and we’ll come help you.

## Do use your tools for finding answers

The challenges are intentionally not step-by-step walkthroughs. Here are some great tools to help you:

* [Google Gemini](https://gemini.google.com/) or [Google Search](https://www.google.com/)  
* [Gemini in Copilot Chat](https://docs.github.com/en/copilot/using-github-copilot/ai-models/using-gemini-in-github-copilot) when writing code (or [aider](https://aider.chat/) if you’re a CLI person)  
* Search the [ADK docs](https://google.github.io/adk-docs/) and explore the [adk-samples](https://github.com/google/adk-samples) repository
* If you have Gemini Pro: Chat with the [adk-python repository](https://github.com/google/adk-python) in [Google Gemini](https://gemini.google.com/) (Hit plus and choose Import Code).  

## You’ll likely need a Google Cloud Project

Most challenges require a Cloud project. In our in-person workshops, you can grab the free $5 credit to use the Google Cloud free tier without a credit card. Be aware that there are some (rate) limits. 

## The Challenges

### [Level 0: AI Studio Fundamentals](levels/level-0/)
Understand the core capabilities of the Gemini model family through direct interaction in AI Studio, without writing any code. This level builds foundational knowledge of what an agent can do before you learn to build one yourself.
*   Explore multi-modal capabilities (text, images, audio).
*   Use speech-to-text and text-to-speech.
*   Combine Google Search with URL context for research.
*   Deploy a prompt as a serverless app from Vertex AI Studio.

### [Level 1: ADK Fundamentals](levels/level-1/)
Go from zero to a running, tool-using agent, and deploy it to the cloud. Some Python experience is recommended.
*   Set up your local environment with `adk create` and `adk web`.
*   Create your first tool for an agent.
*   Deploy your agent to Cloud Run.

### [Level 2: Building Smarter Agents](levels/level-2/)
Move beyond single-function agents to handle conversational memory, connect to external data, and orchestrate complex tasks.
*   Use session state for conversational memory.
*   Save files as artifacts.
*   Connect to external APIs using an OpenAPI spec.
*   Build workflow agents with `SequentialAgent`.
*   Create reasoning agents with `PlanReActPlanner`.
