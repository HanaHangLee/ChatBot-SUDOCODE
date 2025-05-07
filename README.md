# E-commerce Customer Service Chatbot

Developed a chatbot for an e-commerce website to:

- Provide all product information.
- Compare products and generate recommendations based on user input.
- Streamline customer interaction using LLM and semantic search.

## Installation and Setup

See `requirements.txt` and Docker configuration for setup instructions.

## Detailed Overview

🎯 **SUDO CODE 2024 – Third Prize Winner**

🧑‍💻 **Role**: Mentee in a 3-member team mentored by a senior data scientist

📅 **Duration**: Oct 2024 – Dec 2024

👩‍💻 **Program**: Women Techmakers – Data Scientist Apprenticeship

### 🔧 Architecture Highlights

- **Data Ingestion & Embedding**:
    
    Crawled product data (price/specs/promo) → stored in MariaDB → embedded using OpenAI/SentenceTransformer → stored in Qdrant for semantic search.
    
- **Chat Runtime**:
    
    User queries embedded → intent classified → routed to either product info retrieval or LLM (OpenAI).
    
    Redis used for context caching; Celery handles async tasks like vector search and OpenAI API calls.
    
- **Streaming Response**:
    
    Prompts sent to OpenAI → responses streamed to simulate real-time chat.
    
    Redis stores chat history for continuity.
    
- **System Components**:
    
    
    | Component | Technology Used |
    | --- | --- |
    | Vector DB | Qdrant |
    | Embedding | OpenAI API / SentenceTransformers |
    | Async Task Queue | Celery + Redis |
    | Backend API | Django REST Framework |
    | Chat UI | Streamlit |
    | RAG Integration | LlamaIndex + OpenAI GPT |

### 🧠 What I Learned

- Designed end-to-end LLM-powered chatbot using modular architecture.
- Integrated vector search, async task processing, Redis caching, and streaming responses.
- Worked with tools like Celery, Qdrant, LlamaIndex, and OpenAI API.
- Understood production-ready deployment of NLP systems with user-centric UI.

## Demo

[Watch the demo](https://github.com/user-attachments/assets/2a00f359-6878-4928-895a-9e9ff04abe43)


## Acknowledgements

Special thanks to the **Women Techmakers** program and my mentor for guidance and hands-on experience.

