# Pfizer Supply Chain AI-Powered Pharmaceutical Document Processing
<img width="1590" height="870" alt="image" src="https://github.com/user-attachments/assets/2c644500-2d19-4285-9fea-b40e3d1bcd4a" />

## 🧠  Pharmaceutical Document Q&A System
**Intelligent RAG Pipeline for Compliance-Ready Document Analysis**
## 🚀  Project Overview

This project implements an **end-to-end Retrieval-Augmented Generation (RAG) system** that enables users to ask natural language questions over **complex pharmaceutical PDFs and receive** **accurate, source-attributed answers**.

It is specifically designed for **regulated environments** where documents must be:

- Interpreted accurately
- Structured intelligently
- Fully traceable for compliance
## 🖼️ System Architecture

## 💼 Business Impact
- ⏱️ Reduces manual review time for large regulatory documents
- 🎯 Improves accuracy of information retrieval
- 📊 Ensures audit-ready traceability (document + page references)
- 🔍 Automatically handles multi-document PDFs (“blob” files)
- 🔒 Enables local deployment (data privacy friendly)
## 🧠 Key Features
- 📄 LLM-based document classification & boundary detection
- 🎯 Query routing to relevant document types
- 🔍 Semantic search with vector embeddings (FAISS)
- 🧾 Source attribution for compliance
- 💬 Interactive Q&A interface (Gradio UI)
## 🏗️ How It Works
1. Upload PDF (multi-document “blob”)
2. Extract text (PyMuPDF + OCR fallback)
3. Classify document types (LLM)
4. Detect document boundaries
5. Chunk text with overlap
6. Generate embeddings
7. Store in FAISS vector database
8. Route user query to relevant document type
9. Retrieve top-k chunks
10. Generate answer with source attribution
## 📓 Notebook Implementation

👉 Full implementation available in:
Task_Build_the_Full_RAG_UI.ipynb

## What the notebook demonstrates:
- End-to-end RAG pipeline construction
- LLM integration (Mistral via LlamaCPP)
- Chunking + embedding pipeline
- Vector search with FAISS
- Query routing logic
- Gradio UI for interaction

This is not just a prototype—it’s a **working system pipeline**.

## ⚙️ Technical Breakdown
  
  **🔹 LLM (Local Deployment)**
- **Mistral-7B-Instruct (GGUF via LlamaCPP)**
- Used for:
   - Document classification
   - Boundary detection
   - Query routing
   - Answer generation

**🔹 Retrieval-Augmented Generation (RAG)**
- Combines:
  - Semantic retrieval (FAISS)
  - LLM reasoning
- Improves accuracy + explainability

**🔹 Query Routing (Key Differentiator)**
- Routes queries to specific document types
- Reduces noise and improves precision
- Adds scalability vs traditional RAG systems

**🔹 Document Processing**
- PyMuPDF (fitz) → text extraction
- pytesseract → OCR fallback
**🔹 Embeddings & Search**
- Sentence-Transformers (MiniLM)
- FAISS vector database

**🔹 Metadata & Traceability**

Each chunk stores:

- Document type
- Page number
- Source reference

✅ Enables **compliance-ready outputs**

## 🖥️ **Demo (Gradio UI)**

The system includes an interactive UI where users can:

- Upload pharmaceutical PDFs
- Process documents
- Ask natural language questions
- Receive traceable answers
## 🛠️ Tech Stack
- **Python**
- **LlamaIndex**
- **FAISS**
- **Sentence-Transformers**
- **Mistral-7B (LlamaCPP)**
- **PyMuPDF + pytesseract**
- **Gradio**

## 📌 Why This Project Stands Out

This is not a basic RAG implementation. It introduces:

- ✅ **Multi-document understanding within a single PDF**
- ✅ **LLM-driven document intelligence (not just retrieval)**
- ✅ **Query routing for efficiency gains**
- ✅ **Compliance-focused design with traceability**

📈 **Future Improvements**
- Fine-tuned domain-specific embeddings
- Hybrid search (BM25 + vector search)
- Cloud deployment (AWS / Azure)
- Monitoring + evaluation metrics dashboard

👤 **About Me**

**Anish Gupta**

Data & AI Professional specializing in:

- Data Science & Machine Learning
- Public Sector & Regulatory Data
- AI-driven 

🤝 **Let’s Connect**

If you're working on **AI, data science, or document intelligence systems,** feel free to connect or collaborate.
