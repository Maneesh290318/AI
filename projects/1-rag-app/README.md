# RAG Document Assistant

A lightweight retrieval-augmented generation (RAG) application that answers questions using local text documents rather than relying only on a model's general knowledge.

## Architecture

```text
Documents → Chunking → Embeddings → Similarity Retrieval → Context → OpenAI Model → Grounded Answer
```

## Key Capabilities

- Loads local text documents for private knowledge-grounding experiments
- Splits source content into retrievable chunks
- Creates vector representations for semantic matching
- Retrieves relevant context for each user question
- Uses retrieved context to generate document-aware responses

## Tech Stack

Python · OpenAI API · python-dotenv

## Run Locally

```bash
pip install -r requirements.txt
```

Create a local `.env` file:

```text
OPENAI_API_KEY=your_key_here
```

Add source documents to `documents/`, then run:

```bash
python rag_app.py
```

## Engineering Focus

This project demonstrates the core RAG pattern: separating knowledge retrieval from response generation. That architecture can be extended with production vector databases, metadata filtering, citations, evaluation, observability, and access controls.

## Roadmap

- Add source citations to generated answers
- Add persistent vector storage
- Add retrieval-quality evaluation
- Support PDF and structured document ingestion
- Add API and web interfaces
- Add automated tests and containerized deployment

## Security

API credentials are loaded at runtime and should never be committed to source control.
