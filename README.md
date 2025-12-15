# QBR Prompt Templates
A  collection of production-ready prompt templates used in an AI-powered Quarterly Business Review (QBR) automation.

## Generation Prompts
Used to generate individual sections of the QBR.

### Model used:
GPT-5.1 

Estimated cost:
~2,000 tokens per full QBR workflow (all sections combined)

## Judge Prompts 
Used for LLM-as-a-Judge evaluation of the generated content.
### Model used:
GPT-4.1-mini 

### Quality Tracking 
Persistent quality tracking in production workflows. In the live automation:
- The generated QBR sections
- The judge score and evaluation feedback
are stored in PostgreSQL (Neon).

### How These Prompts Are Used

- Injected with runtime data 
- Executed as independent LLM calls
- Evaluated via a dedicated judge step
- Iterated using prompt versioning

# AI Agent with Knowledge Base (RAG)

The system includes a tool-enabled AI agent that provides conversational access to data.
The agent combines:
- Structured account data retrieved from PostgreSQL via tools
- An authoritative knowledge base (company policies, metric definitions, and interpretation rules) indexed using Retrieval-Augmented Generation.

## Knowledge Base
A static internal document containing:
- Official definitions of QBR metrics
- Threshold-based interpretation rules
- Customer Success policies and guidelines
### The document is ingested once, chunked, embedded, and queried at runtime using semantic search.




