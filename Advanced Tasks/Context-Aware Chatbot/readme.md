# AI Knowledge Assistant (RAG-based Chatbot)

An AI-powered **Retrieval Augmented Generation (RAG) chatbot** that answers questions using a custom knowledge base. The system retrieves the most relevant documents using vector search and generates contextual responses using a large language model.

This project demonstrates how to build a **lightweight, locally powered RAG system** using open-source tools and free APIs.

---

## Features

- Retrieval Augmented Generation (RAG) pipeline
- Semantic search using embeddings
- Fast vector similarity search
- Conversational memory
- Custom knowledge base support
- Source citation for transparency
- Simple interactive UI

---

## Architecture

The system follows a standard **RAG pipeline**.


User Query
│
▼
Embed Query (Sentence Transformers)
│
▼
FAISS Vector Search
│
▼
Retrieve Top-K Relevant Documents
│
▼
Combine With Conversation Memory
│
▼
Prompt Construction
│
▼
Groq LLM (Llama 3)
│
▼
Generated Answer + Sources


---

## Tech Stack

| Component | Technology |
|----------|------------|
| Orchestration | LangChain |
| Embeddings | sentence-transformers/all-MiniLM-L6-v2 |
| Vector Database | FAISS |
| LLM | Groq API (Llama 3) |
| Memory | ConversationBufferWindowMemory |
| UI | Streamlit |
| Knowledge Base | Custom Documents |

---

## Project Structure


project/
│
├── app.py # Streamlit interface
├── rag_pipeline.py # RAG logic
├── ingest.py # Document ingestion
├── knowledge_base/ # Custom documents
│
├── vector_store/ # FAISS index
│
├── requirements.txt
└── README.md


---

```bash
git clone https://github.com/yourusername/ai-knowledge-assistant.git
cd ai-knowledge-assistant
