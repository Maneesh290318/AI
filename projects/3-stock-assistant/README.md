# Market Data AI Assistant

A conversational prototype that combines market-data retrieval with LLM-generated explanations, demonstrating how structured external data can be transformed into a natural-language user experience.

## Workflow

```text
User Question → Ticker / Intent → Market Data Retrieval → Structured Metrics → LLM Explanation → Response
```

## Key Capabilities

- Retrieves market information for common ticker symbols
- Processes structured financial metrics
- Generates plain-language explanations
- Supports basic comparisons across securities
- Demonstrates read-only tool-assisted AI

## Tech Stack

Python · OpenAI API · Yahoo Finance data · python-dotenv

## Run Locally

```bash
pip install -r requirements.txt
python stock_assistant.py
```

Configure `OPENAI_API_KEY` securely at runtime.

## Engineering Focus

This project demonstrates a common applied-AI architecture: use deterministic tools or APIs to obtain factual structured data, then use an LLM as the explanation layer rather than the source of the underlying market data.

## Roadmap

- Add charts and historical trends
- Add explicit source timestamps
- Add technical indicators
- Add news/sentiment enrichment
- Add response evaluation and caching
- Expose functionality through an API

## Disclaimer

This project is for educational and portfolio purposes only and does not provide investment advice. Market data can be delayed or incomplete and should be independently verified.
