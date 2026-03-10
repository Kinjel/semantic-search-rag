# Semantic Search & Retrieval-Augmented Generation (RAG) System

## Overview

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline that retrieves relevant information from documents using **semantic search** and generates context-aware responses using a **Large Language Model (LLM)**.

The system converts documents into **vector embeddings**, stores them in a **FAISS vector database**, retrieves relevant content based on user queries, and generates responses using an LLM.

---

## Technologies Used

* Python
* FAISS (Vector Database)
* Google Gemini Embeddings
* Groq API (LLaMA 3.3 Model)
* PocketFlow
* NumPy

---

## Workflow

1. Documents are divided into smaller chunks.
2. Each chunk is converted into vector embeddings.
3. Embeddings are stored in a FAISS vector index.
4. User queries are converted into embeddings.
5. Vector similarity search retrieves the most relevant document chunks.
6. Retrieved context is provided to the LLM to generate the final answer.

---

## Example Query

```
What is Semantic Search?
```

### Retrieved Context

Semantic search systems convert documents and queries into embeddings and compare them using vector similarity.

### Generated Response

The system retrieves relevant document chunks using FAISS and generates an answer using the LLaMA model.

---

## How to Run

1. Install required libraries

```
pip install faiss-cpu
pip install google-genai
pip install pocketflow
pip install groq
```

2. Add API keys for:

* Google Gemini
* Groq

3. Run the notebook:

```
rag_semantic_search.ipynb
```
