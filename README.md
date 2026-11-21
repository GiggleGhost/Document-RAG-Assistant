# Document RAG Assistant

A Python-based Retrieval-Augmented Generation (RAG) application that enables users to query and extract accurate, context-aware answers directly from PDF documents using Large Language Models (LLMs) and vector search.

## Features

- **PDF Document Ingestion:** Automatically parses and chunks PDF files stored in the `documents/` directory.
- **Semantic Retrieval:** Converts text chunks into vector embeddings to retrieve the most relevant context for any user query.
- **Context-Grounded Answers:** Generates accurate responses backed by the uploaded documents, minimizing model hallucinations.
- **Sample Knowledge Base:** Includes a pre-loaded sample document (`GenAI_RAG_Sample.pdf`) for immediate testing.

## Project Structure

```text
RAG/
├── app.py                  # Main application entry point and user interface
├── rag.py                  # Core RAG pipeline (document loading, chunking, embedding, retrieval)
├── documents/              # Directory for source PDF files
│   └── GenAI_RAG_Sample.pdf
├── requirements.txt        # Python package dependencies
├── .env.example            # Environment variable template
├── .gitignore              # Git ignore rules
└── README.md               # Project documentation

streamlit
langchain
langchain-community
langchain-google-genai
langchain-text-splitters
faiss-cpu
pypdf
python-dotenv
