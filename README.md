## For Recruiters 👋

Thanks for visiting this project via my CV or portfolio!

This chatbot was developed during a mentored apprenticeship program (Women Techmakers) in a 3-member team, under the guidance of a senior data scientist. While I did not implement the entire system, I gained valuable experience and contributed meaningfully in areas aligned with my learning stage.

🛠️ **My Key Contributions**:
- Researched and prototyped LlamaIndex integration for retrieval-augmented query responses using OpenAI embeddings.
- Presented the architecture of asynchronous task handling using Redis and Celery, demonstrating understanding of how it enables real-time LLM responses.
- Contributed to the design of query routing logic between product search and generative replies.
- Participated in testing, debugging, and evaluating the chatbot’s semantic search output.

🎯 The experience significantly expanded my technical foundation and gave me hands-on exposure to a production-grade LLM application.

➡️ Jump to: [Architecture](#-architecture-highlights) | [Demo](#demo)

# E-commerce Customer Service Chatbot

A chatbot prototype built in one month as part of a mentored team project to enhance customer experience on e-commerce platforms. The system allows users to:

- Retrieve detailed product information (price, specs, promotions).
- Compare multiple products and get personalized recommendations.
- Interact naturally through a real-time LLM-powered chat interface using semantic search.

Key features include:

- Crawled and embedded product data from `thegioididong.com`; stored vectors in Qdrant for semantic retrieval.
- Integrated LlamaIndex with OpenAI API to implement a retrieval-augmented generation (RAG) pipeline.
- Designed chat flow combining intent detection, vector-based routing, and streaming responses via OpenAI.
- Implemented asynchronous task handling using Celery and Redis to support scalable, real-time interaction.


## Installation and Setup

See `requirements.txt` and Docker configuration for setup instructions.

## Detailed Overview

🎯 **SUDO CODE 2024 – Third Prize Winner**

🧑‍💻 **Role**: Mentee in a 3-member team mentored by a senior data scientist

📅 **Duration**: Oct 2024 – Dec 2024

👩‍💻 **Program**: Women Techmakers – Data Scientist Apprenticeship

### 🔧 Architecture Highlights
![image](https://github.com/user-attachments/assets/0048f248-6492-4cdb-a62d-5baf0c6b5451)


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

- Gained hands-on experience working on an LLM-powered chatbot within a real-world team setting.
- Developed understanding of how vector search, async task queues (Celery + Redis), and retrieval-augmented generation (RAG) work together.
- Took ownership of specific research and presentation tasks, especially around LlamaIndex and system architecture.
- Learned how to bring NLP systems to a production-ready state with user-centric design, while improving collaboration and communication through hands-on mentorship..


## Demo

[Watch the demo](https://github.com/user-attachments/assets/2a00f359-6878-4928-895a-9e9ff04abe43)


## Acknowledgements

Special thanks to the **Women Techmakers** program and my mentor for guidance and hands-on experience.

