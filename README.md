 # This repo is a collection of prompt templates used in an AI-powered Quarterly Business Review automation.

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

# AI Agent 

The system includes a tool-enabled AI agent that provides conversational access to data.
The agent combines:
- Structured account data retrieved from PostgreSQL via tools
- An authoritative knowledge base (company policies, metric definitions, and interpretation rules)

## Retrieval-Augmented Generation 

The knowledge base is integrated using a RAG pipeline to ensure grounded and accurate responses.

- An internal source document is ingested and processed offline
- Content is chunked and converted into semantic embeddings
- Embeddings are stored in a vector store and queried at runtime
- Relevant chunks are retrieved dynamically and injected into the agent’s context

embeddings are generated using OpenAI’s embedding model `text-embedding-3-small`

## Knowledge Base
An internal document containing:
- Official definitions of QBR metrics
- Threshold-based interpretation rules
- Customer Success policies and guidelines





