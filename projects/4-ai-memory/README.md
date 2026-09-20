# Conversational AI with Persistent Memory

A conversational AI prototype that maintains context across interactions and persists conversation history between sessions.

## Architecture

```text
User Message → Load Conversation State → Build Context → OpenAI Model → Response → Persist Updated State
```

## Key Capabilities

- Maintains short-term conversational context
- Persists history across application sessions
- Uses prior context when generating responses
- Supports inspecting and clearing stored memory
- Demonstrates stateful AI application design

## Tech Stack

Python · OpenAI API · JSON persistence · python-dotenv

## Run Locally

```bash
pip install -r requirements.txt
python memory_ai.py
```

Configure `OPENAI_API_KEY` through a secure runtime environment.

## Engineering Focus

Stateless model APIs do not automatically provide application-level memory. This project demonstrates how an application can explicitly manage state, reconstruct relevant context, and persist conversations.

For production systems, the same pattern can be extended with database-backed memory, semantic retrieval, summarization, retention policies, encryption, and user-level isolation.

## Roadmap

- Replace flat-file persistence with a database
- Add semantic memory retrieval
- Add conversation summarization
- Add user/session isolation
- Add configurable retention controls
- Add automated tests

## Privacy

Conversation history is stored by the application. Real deployments should define retention, access, encryption, and deletion policies appropriate to the data being processed.
