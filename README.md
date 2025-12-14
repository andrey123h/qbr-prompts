# QBR Prompt Templates
A  collection of production-ready prompt templates used in an AI-powered Quarterly Business Review (QBR) automation.

## Generation Prompts (GPT-5.1)
Used to generate individual sections of the QBR.

### Model used:
GPT-5.1 
Estimated cost:
~2,000 tokens per full QBR workflow (all sections combined)

## Judge Prompts 
Used for LLM-as-a-Judge evaluation of the generated content.
### Model used:
GPT-4.1-mini 

### Prompts Tracking 
Persistent quality tracking in production workflows. In the live automation:
- The generated QBR sections
- The judge score and evaluation feedback
are stored in PostgreSQL (Neon).

### How These Prompts Are Used

- Loaded dynamically into an n8n workflow
- Injected with runtime data (metrics, notes, feedback)
- Executed as independent LLM calls
- Evaluated via a dedicated judge step
- Iterated safely using prompt versioning


