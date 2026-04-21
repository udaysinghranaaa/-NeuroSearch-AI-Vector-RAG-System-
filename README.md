# 🧠 NeuroSearch AI (Vector + RAG System)

A high-performance **Vector Database built from scratch in C++**, integrated with a **Retrieval-Augmented Generation (RAG)** pipeline using a local LLM via Ollama.

This project demonstrates how modern AI systems like Pinecone, Weaviate, and Chroma work internally — including **HNSW indexing, semantic search, and LLM-based answer generation**.

---

## 🚀 Features

* 🔍 **3 Search Algorithms**

  * HNSW (production-grade)
  * KD-Tree
  * Brute Force

* 📏 **3 Distance Metrics**

  * Cosine Similarity
  * Euclidean Distance
  * Manhattan Distance

* 🧠 **Semantic Search**

  * Converts text → vector embeddings
  * Finds nearest neighbors in vector space

* 📄 **Document Embedding**

  * Uses Ollama (`nomic-embed-text`)
  * Splits long text into chunks automatically

* 🤖 **RAG Pipeline**

  * Retrieves relevant chunks using HNSW
  * Generates answers using LLM (`llama3.2`)

* 📊 **Visualization**

  * PCA-based 2D scatter plot
  * Shows semantic clustering of vectors

---

## 🛠 Tech Stack

* **C++** (Core backend + algorithms)
* **HTML, CSS, JavaScript** (Frontend UI)
* **Ollama** (Local LLM + embeddings)
* **REST API** (Communication layer)

---

## ⚙️ How It Works

User Query
⬇
Embedding (Ollama)
⬇
Vector Search (HNSW)
⬇
Top Matching Context
⬇
LLM (llama3.2)
⬇
Final Answer

---

## ▶️ Run Locally

### 1. Start Ollama

```
ollama serve
```

### 2. Run Project

```
./db
```

### 3. Open in Browser

```
http://localhost:8080
```

---

## 📁 Project Structure

```
├── main.cpp        # C++ backend (Vector DB + RAG)
├── httplib.h       # HTTP server library
├── index.html      # Frontend UI
└── README.md
```

---

## 💡 Key Concepts

* **HNSW (Hierarchical Navigable Small World)**

  * Fast approximate nearest neighbor search (O(log N))

* **Vector Embeddings**

  * Converts text into numerical vectors

* **RAG (Retrieval-Augmented Generation)**

  * Combines search + LLM for accurate answers

---

## ⚠️ Requirements

* MSYS2 (for g++)
* Git
* Ollama

---

## 👨‍💻 Author

**Uday Singh Rana**

---

## ⭐ Note

This is a **local AI system** — no external API required.
Runs fully on your machine using Ollama.
