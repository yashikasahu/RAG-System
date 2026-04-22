# 🧠 RAG System — Retrieval-Augmented Generation Pipeline

A production-style **Retrieval-Augmented Generation (RAG)** system that answers questions from custom documents using embeddings, vector search, and LLMs with **grounded responses and citations**.

---

## 🚀 Overview

This project implements a full RAG pipeline:

```
User Query → Embedding → Vector Search → Context Retrieval → LLM → Answer (+ Citations)
```

Instead of relying on the LLM’s memory, the system retrieves relevant information from a document corpus (PDFs, text files) and generates **accurate, context-based answers**.

---

## ✨ Features

* 📄 Document ingestion (PDF + text files)
* ✂️ Smart chunking with overlap
* 🔢 Embedding generation using Sentence Transformers
* 🗂️ Vector storage using ChromaDB
* 🔍 Custom retriever with similarity filtering
* 🧠 Context-aware answer generation
* 🔗 Inline citations from source documents
* 📝 Answer summarization
* 🕘 Query history tracking

---

## 🧱 Project Architecture

* **EmbeddingModel** → Generates vector embeddings
* **VectorStore** → Stores and manages embeddings
* **RAGRetriever** → Retrieves relevant chunks
* **AdvancedRAGPipeline** → End-to-end system

---

## ⚙️ Tech Stack

* Python
* Sentence Transformers (`all-MiniLM-L6-v2`)
* ChromaDB (vector database)
* LangChain utilities
* Groq LLM (Llama 3)

---

## 📂 Project Structure

```
RAG/
│
├── data/
│   ├── PDF/
│   ├── text_files/
│
├── notebook/
│   └── document.ipynb
│
├── main.py
├── requirements.txt
├── README.md
├── .gitignore
```

---

## ▶️ How to Run

```bash
# install dependencies
pip install -r requirements.txt

# run the project
python main.py
```

---

## 🧪 Example Query

```
Query: Explain attention mechanism in transformers
```

**Output:**

* Context-based answer
* Inline citations ([1], [2], etc.)
* Optional summary

---

## 📈 Current Status

* Functional RAG pipeline
* Citation-based answers
* Intermediate-level system design

---

## 🔮 Future Improvements

* Hybrid retrieval (BM25 + vector search)
* Cross-encoder re-ranking
* Evaluation metrics (RAGAS)
* FastAPI deployment
* Frontend UI

---

## 💡 Key Insight

> The quality of a RAG system depends more on **retrieval quality** than the LLM itself.

---

## 📌 Author

Yashika Sahu
Data Analyst / AI-ML Enthusiast
