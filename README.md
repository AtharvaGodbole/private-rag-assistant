# private-rag-assistant
A private, production-ready Retrieval-Augmented Generation (RAG) assistant using LangChain, Chroma, and local LLMs — answer questions from your own documents with zero cloud dependency.
# 🔍 Retrieval-Augmented Generation (RAG) with Local LLMs

A hands-on, production-ready Retrieval-Augmented Generation (RAG) system powered by **LangChain**, **ChromaDB**, and **local LLMs**. This project demonstrates how to build an intelligent Q&A system over custom documents — *completely offline* — using open-source tools.

> 🚀 Designed for AI Engineers, ML Practitioners, and Recruiters who want to see practical GenAI in action.

---

## 📌 Features

- **Fully Local RAG Pipeline** — No cloud APIs required
- **LangChain-Powered Workflows** — Clean integration of embedding, retrieval, and generation
- **Chroma Vector DB** — Efficient and lightweight vector storage
- **Custom Document Parsing** — Load and chunk your own PDFs
- **Embeddings + LLMs** — Swap between local or OpenAI models
- **Modular Codebase** — Easy to extend or productionize
- **Test Suite** — Verify performance and accuracy with test cases

---

## 🧠 Architecture Overview

[ PDF Documents ]
↓
[ Text Splitter ] ← customizable chunking
↓
[ Embedding Function ] ← OpenAI or local
↓
[ Chroma Vector DB ] ← stores vectors locally
↓
[ Retriever + LLM ] ← powered by LangChain
↓
[ Generated Answer ]


---

## 🛠️ Tech Stack

| Component         | Tool/Library      |
|------------------|-------------------|
| LLM Interface     | [LangChain](https://www.langchain.com/)     |
| Embeddings        | OpenAI / HuggingFace Transformers |
| Vector Database   | [ChromaDB](https://www.trychroma.com/)     |
| Document Parsing  | PyMuPDF / LangChain Document Loaders |
| Local Serving     | Python CLI        |
| Testing           | `unittest` / Custom test suite |

---

## 🚀 Getting Started

1. Clone & Install
git clone https://github.com/pixegami/rag-tutorial-v2.git
cd rag-tutorial-v2
pip install -r requirements.txt

2. Add PDFs
Drop your PDFs into the data/ folder.

3. Populate Vector DB
python populate_database.py

4. Ask Questions
python query_data.py "What is this document about?"

🧪 Run Tests
python test_rag.py


🧩 File Structure
├── data/                     # Input documents (PDFs)
├── get_embedding_function.py # Embedding model loader
├── populate_database.py      # Chunks + embeds + stores
├── query_data.py             # Retrieves and generates answers
├── test_rag.py               # Test cases
├── requirements.txt          # Python dependencies
└── README.md

🌐 Demo Use Case
📄 Upload: Research papers, legal contracts, or manuals
💬 Ask: “What are the key findings?” or “What clauses relate to liability?”
🧠 Get: Accurate, contextual responses using your documents

👔 Why This Project Matters
✅ Production-Ready Patterns — Shows how RAG pipelines are structured in real-world applications
✅ Offline GenAI — Perfect for privacy-sensitive or air-gapped environments
✅ Recruiter Showcase — Demonstrates full-stack AI/ML development: data ingestion → embedding → retrieval → generation

🤝 Connect
Built by [Atharva Godbole] — AI/ML Engineer passionate about open-source GenAI and real-world deployment.

📫 Reach me at: [avsgod21@gmail.com]
💼 [https://www.linkedin.com/in/atharvagodbole98/] 

