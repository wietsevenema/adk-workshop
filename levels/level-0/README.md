## Level 0: AI Studio Fundamentals (Introductory)

**Goal:** Understand the core capabilities of the Gemini model family, without writing any code. This section builds the foundational knowledge of what an agent can do before you learn to build one yourself. In their essence, every agent is one (or more) prompts with some orchestration glue code around it. 

**Prerequisites:** All you need is a web browser to access [AI Studio](https://aistudio.google.com/). Only the final challenge requires a Google Cloud project.

---
### Challenge: Multi-Modal Understanding
     
**Concept:** Gemini is "multi-modal," meaning it can understand information from different formats like text, images, and audio simultaneously. This is a powerful capability that allows you to build applications that can "see" and interpret the world, not just process text.

**Task:** Your goal is to verify Gemini's ability to understand an image. In AI Studio, provide an image to the model and ask it to describe the image, extract text from it, or to identify objects in the image.

**Outcome:** The model will return a text-based answer to your question, demonstrating that it understood the contents of the image.

**Question:** What ar other types of files you can upload to test Gemini's multi-modal capabilities?

---
### Challenge: Speech-to-Text
     
**Concept:** Gemini can understand spoken language from audio and video files. This is useful for transcribing meetings, analyzing customer calls, or making video content searchable.

**Task:** Your goal is to get a written transcript from a video. In AI Studio, provide a YouTube Video (through the plus icon) to the model and ask it to transcribe the audio with speaker identification.

**Outcome:** The model will return a written transcript of the spoken content from the video.

**Question:** How could you use this transcription capability to quickly find specific information within a long video lecture?

---
### Challenge: Text-to-Speech
     
**Concept:** Gemini can generate high-quality, natural-sounding human speech from text. This allows agents to communicate with users through voice, creating more interactive and accessible experiences.

**Task:** Your goal is to have Gemini read a piece of text aloud. In AI Studio, write a sentence or paragraph and ask the model to generate audio from it.

**Outcome:** You will be able to play a high-quality audio file of Gemini speaking the text you provided.

**Question:** What languages are supported? Can you mix different languages in one sentence? 

---
### Challenge: Building your own 'Gemini Deep Research'
     
**Concept:** A model's knowledge is limited to its training data. To perform research, it needs to access external information. The Google Search tool allows it to discover current sources, while the URL Context tool allows it to perform a deep analysis of specific web pages. 

**Task:** Your goal is to combine search and URL context. Enable both the tools and ask a question you want to research. See how the answer changes when you disable the tools.

**Outcome:** The model provides a synthesized answer based on one or more searches, demonstrating its ability to find information, reason about, make follow up queries, and read the result pages. 

**Question:** What are the risks of relying on data you find on the internet? 

---
### Challenge: From Prompt to Deployed App
     
**Concept:** A well-crafted prompt can be a complete application. [Vertex AI Studio](https://console.cloud.google.com/vertex-ai/generative/language) (the enterprise-grade version of AI Studio) can instantly deploy a prompt as a serverless web app with a web UI and its own endpoint. 

**Task:** Your goal is to create a simple translation service. In Vertex AI Studio, create a prompt that translates English text to German. Use a *prompt variable* for the text component. Use the "Build with code" > "Deploy as app" button to create a callable API endpoint for your translator.

**Outcome:** You will have a live, public API endpoint that takes English text and returns its German translation.

**Question:** How would you modify the prompt to ensure the translation uses a certain style? 
