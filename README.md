# 🤖 private-rag-assistant

A fully private, production-ready Retrieval-Augmented Generation (RAG) assistant — built using **LangChain**, **Chroma**, and **local LLMs**. This system lets you query your personal documents (PDFs, reports, contracts) with natural language — entirely **offline**, with **zero cloud dependency**.

> 🔐 Perfect for privacy-first use cases, air-gapped environments, and showcasing practical GenAI engineering.

---

## 🔍 What Is It?

A hands-on, end-to-end RAG pipeline that demonstrates how to:

- Parse and chunk documents (PDFs)
- Generate and store vector embeddings locally
- Retrieve relevant context for any user query
- Generate responses using an LLM — without calling external APIs

Built from scratch using open-source tools, this project is ideal for AI engineers, ML practitioners, and recruiters who want to see GenAI done *the right way*.

---

## ✨ Key Features

- 🧠 **Complete Local RAG Stack** — Fully functional with no internet required  
- ⚙️ **LangChain-Powered Workflows** — Clean integration of embedding, retrieval, and generation logic  
- 📦 **Chroma Vector Store** — Fast, lightweight, and local vector database  
- 📄 **Document-Aware** — Plug in your own PDFs and ask anything  
- 🔁 **Pluggable Models** — Use OpenAI or local Hugging Face models  
- 🧪 **Testable & Modular** — Easily extend and validate with test cases  

---

## 🧠 Architecture Overview
[ PDF Documents ]
↓
[ Text Splitter ] ← Custom chunking
↓
[ Embedding Function ] ← Local or OpenAI
↓
[ Chroma Vector DB ] ← Fast, local storage
↓
[ Retriever + LLM ] ← LangChain pipeline
↓
[ Answer Generation ]


---

## 🛠️ Tech Stack

| Purpose             | Tool / Library                    |
|---------------------|-----------------------------------|
| LLM Interface        | [LangChain](https://www.langchain.com/)        |
| Embeddings           | OpenAI / HuggingFace Transformers |
| Vector Storage       | [ChromaDB](https://www.trychroma.com/)         |
| Document Parsing     | PyMuPDF / LangChain Loaders       |
| CLI + Scripting      | Python 3.10+                      |
| Testing              | `unittest` + custom assertions   |

---

## 🚀 Quickstart

### 1. Clone the Repo
git clone https://github.com/pixegami/rag-tutorial-v2.git
cd rag-tutorial-v2
pip install -r requirements.txt

### 2. Add Your PDFs
Place your documents into the data/ folder.

### 3. Populate the Vector Database
python populate_database.py

### 4. Ask Natural Language Questions
python query_data.py "What is this document about?"

### 5. Run Tests
python test_rag.py


## 🧩 File Structure
'''
├── data/                      # Input documents (PDFs)
├── get_embedding_function.py  # Embedding model loader
├── populate_database.py       # Document chunking + vectorization
├── query_data.py              # Retrieval + generation logic
├── test_rag.py                # Tests for the RAG pipeline
├── requirements.txt           # Dependencies
└── README.md                  # This file ✨
'''
🌐 Use Case Examples

📝 Research Assistant — Upload academic papers and ask for summaries
⚖️ Legal AI — Analyze contracts and extract clauses
📚 Knowledge Base — Query internal docs, FAQs, handbooks, etc.

👔 Why This Project Stands Out
✅ Real-World Relevance — Mirrors how RAG systems are deployed in production
✅ Offline-First — Ideal for privacy-sensitive industries
✅ Recruiter-Ready — Demonstrates full-stack AI/ML capability: ingestion → embedding → retrieval → generation

🤝 About the Author
Built with ❤️ by Atharva Godbole — an AI/ML Engineer passionate about open-source GenAI, document intelligence, and privacy-first AI.

📫 Email: avsgod21@gmail.com
💼 LinkedIn: linkedin.com/in/atharvagodbole98
