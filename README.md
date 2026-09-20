# Applied AI Engineering Projects

A collection of hands-on AI applications exploring retrieval-augmented generation (RAG), agent workflows, conversational memory, real-time data assistants, and AI-powered data quality.

## Portfolio Projects

### 1. RAG Document Assistant
Builds a retrieval-augmented generation workflow that processes documents, creates embeddings, retrieves relevant context, and uses an LLM to answer grounded questions.

**Focus:** document processing, chunking, embeddings, vector retrieval, grounded generation

### 2. Social Media AI Agent with Human Approval
Explores an AI-assisted content workflow in which generated content is reviewed before publication.

**Focus:** agent workflows, human-in-the-loop design, content generation, approval controls

### 3. Stock Data AI Assistant
Combines market-data retrieval with AI-generated explanations to make structured financial information easier to interpret.

**Focus:** external APIs, data processing, LLM explanations, tool-assisted workflows

### 4. Conversational AI with Memory
Demonstrates persistent conversational context across interactions and sessions.

**Focus:** memory management, session persistence, context handling, personalized responses

### 5. Data Quality Copilot
Analyzes tabular data and surfaces data-quality issues to support faster validation and investigation.

**Focus:** CSV analysis, data-quality checks, automated findings, AI-assisted analytics

## Repository Structure

```text
projects/
├── 1-rag-app/
├── 2-social-media-agent/
├── 3-stock-assistant/
├── 4-ai-memory/
└── 5-data-quality-copilot/
```

Each project contains its own implementation and supporting documentation.

## Engineering Themes

- Retrieval-Augmented Generation (RAG)
- AI agents and tool-assisted workflows
- Human-in-the-loop AI
- Conversational memory
- API integration
- Data quality and analytics
- Secure configuration through environment variables

## Getting Started

```bash
git clone https://github.com/Maneesh290318/AI.git
cd AI
```

Choose a project and follow the README within its directory.

For Python projects, dependencies can typically be installed with:

```bash
pip install -r requirements.txt
```

Create a local `.env` file only when a project requires runtime credentials. Never commit secrets or API keys.

## Portfolio Direction

These projects are designed to evolve from focused prototypes into production-oriented AI systems with stronger evaluation, observability, testing, deployment, and cloud integration.

Planned improvements include architecture diagrams, automated tests, Docker packaging, CI/CD, model evaluation, tracing, and deployable demos.

## Disclaimer

The projects are educational and portfolio implementations. AI-generated outputs should be reviewed before being used in consequential workflows.
