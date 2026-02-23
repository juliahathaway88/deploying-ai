Overview

A conversational AI system with multiple services and a chat interface. The bot is friendly, maintains short-term memory, and can answer questions, provide weather updates, perform semantic search, and tell jokes.

1. Services

Weather Service (API Calls)

Uses OpenWeatherMap API.

Returns natural-language summaries of weather (temperature, humidity, conditions).

2. Semantic Search Service

Uses OpenAI embeddings (text-embedding-3-small) on a SQuAD CSV dataset.

Stores embeddings in ChromaDB and retrieves top relevant passages for queries.

3. Joke Service

Returns a simple, humorous response triggered by keywords like “joke.”

4. Chat Interface

Built with Gradio.

Maintains short-term memory (last 3 exchanges).

Friendly personality with guardrails for restricted topics (cats, dogs, horoscopes, zodiac, Taylor Swift).

5. Notes

Embeddings are generated automatically if not already in chroma_db.

Guardrails prevent responses to restricted topics.

Short-term memory gives conversational context for user queries.