# AEC Agent Skills

Specialized AI agent skills for Architecture, Engineering, and Construction (AEC) professionals. This project explores the development of a modular AI workforce, translating domain-specific tasks into executable agent actions to enhance productivity and decision-making in the construction engineering lifecycle.

## Key Features
*   **Domain-Specific Skills:** Implements agents capable of parsing construction documents, performing basic quantity takeoffs, and analyzing design constraints.
*   **Modular Architecture:** Skills are designed as independent, composable modules for flexible agent assembly.
*   **Tool Integration:** Connects AI reasoning with external data sources and calculation engines relevant to AEC workflows.

## Tech Stack
*   Python
*   LangChain / LlamaIndex
*   FastAPI
*   OpenAI / Anthropic APIs

## Getting Started
1.  Clone the repo: `git clone https://github.com/zoreanuj/AEC_Agent_Skills.git`
2.  Install dependencies: `pip install -r requirements.txt`
3.  Set your API keys in a `.env` file.
4.  Run the example agent: `python examples/basic_agent.py`