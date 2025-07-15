# Retrieval-Augmented Generation (RAG) Pipeline 

This project implements a lightweight Retrieval-Augmented Generation (RAG) pipeline that leverages semantic search and Together AI's LLMs to answer natural language questions based on a custom corpus of documents.

---

## Setup

install dependancies via 
```pip install -r requirements.txt```

---

##  Features

-  **Context-aware Question Answering** using LLMs
-  Supports embedding and retrieval from a custom document set
-  Uses **Together AI** API for inference (e.g. Llama-3-70B)
-  FAISS-based vector search
-  Simple CLI or script interface
-  Secrets handled securely via `.env`

---

##  Architecture

```text
User Query
   ↓
Retrieve relevant context chunks from FAISS
   ↓
Format prompt with context + query
   ↓
Send prompt to Together AI LLM via API
   ↓
Receive and return answer
```
