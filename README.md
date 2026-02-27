# Agentic YouTube Intelligence  

*A playful yet structured experiment in building a tool-using AI agent that thinks before it acts — and occasionally acts before it thinks.*

---

## About This Project  

This project serves as a minimal but intentional MVP for exploring agent-style AI systems that I plan to evolve into real-world, production-grade applications. Its current objective is straightforward: given a YouTube query, the system searches for relevant videos, extracts transcripts, summarizes the content, and generates a structured PDF output.

However, the true purpose of the project is not the summary itself. The focus is on the architecture — designing a system where an LLM controls tools, maintains state, and makes iterative decisions instead of following a rigid, hardcoded workflow. While the present version may not yet solve a large-scale real-world problem, it acts as a controlled sandbox for experimenting with agent reasoning, tool orchestration, and autonomy.

The long-term vision is to extend this architecture into a more robust, real-world system capable of handling complex research tasks, multimedia knowledge extraction, and autonomous information synthesis. The current implementation is the foundation.

In short, this is not just a content summarizer. It is an architectural playground for building real AI agents.

---

## How It Works  

The system operates around a reasoning loop inspired by ReAct-style agents:
User Goal
→ LLM evaluates current state
→ LLM decides next action
→ Appropriate tool is invoked
→ Result is observed and added to state
→ LLM reassesses
→ Continue or stop


Instead of enforcing a fixed pipeline, the LLM acts as the controller. The tools act as specialists.
