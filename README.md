<p align="center">
<h1 align="center">RAG Chatbot for Document Analysis
</h1>
</p>

<p align="center">
    <img src="https://img.shields.io/badge/Language-Python-3776AB?logo=python&logoColor=white" alt="Python">
    <img src="https://img.shields.io/badge/Framework-Streamlit-FF4B4B?logo=streamlit&logoColor=white" alt="Streamlit">
    <img src="https://img.shields.io/badge/LLM-OpenAI GPT-412991?logo=openai&logoColor=white" alt="OpenAI GPT">
    <img src="https://img.shields.io/badge/Framework-LangChain-FF6B35?logo=langchain&logoColor=white" alt="LangChain">
    <img src="https://img.shields.io/badge/VectorDB-FAISS-00A98F?logo=faiss&logoColor=white" alt="FAISS">
    <img src="https://img.shields.io/badge/Embeddings-OpenAI-412991?logo=openai&logoColor=white" alt="OpenAI Embeddings">
    <img src="https://img.shields.io/badge/Processing-PyPDF2-FF6B35?logo=pdf&logoColor=white" alt="PyPDF2">
    <img src="https://img.shields.io/badge/Splitters-LangChain-FF6B35?logo=langchain&logoColor=white" alt="LangChain Splitters">
    <img src="https://img.shields.io/badge/Text%20Processing-TikToken-000000?logo=tiktok&logoColor=white" alt="TikToken">
    <img src="https://img.shields.io/badge/Environment-python--dotenv-FFD43B?logo=python&logoColor=black" alt="python-dotenv">
    <img src="https://img.shields.io/badge/Virtual%20Env-venv-3776AB?logo=python&logoColor=white" alt="venv">
</p>


<p align="center">
  <img src="./assets/chat.png" width="800"/><br/>
  <em>Demo: RAG Chatbot </em>
</p>


## RAG Chatbot for Document Analysis

A Retrieval-Augmented Generation (RAG) chatbot that allows users to upload PDF documents and ask questions about their content using AI-powered document analysis. This chatbot is using ChatGPT API for the NLP and Streamlit for the user interface

## What's this model about?

The RAG Chatbot is an AI-powered document analysis system that combines document retrieval with generative AI to answer questions about uploaded PDF files. This model uses:

- **Document Processing**: Extracts and chunks text from PDF documents
- **Vector Embeddings**: Creates semantic embeddings using OpenAI's models
- **Similarity Search**: Retrieves relevant document sections using FAISS
- **AI Generation**: Generponses using GPT models based on retrieved context

The system enables users to quickly query large documents without manually reading through them, making it ideal for research, document analysis, and information retrieval tasks.

## Tech Stack

- **Frontend**: Streamlit
- **Backend**: Python
- **Document Processing**: PyPDF2
- **Text Splitting**: LangChain Text Splitters
- **Embeddings**: OpenAI Embeddings
- **Vector Database**: FAISS
- **AI Models**: OpenAI GPT-3.5/4
- **Framework**: LangChain
- **Environment Management**: Python-dotenv

## Features

- 📁 Upload PDF documents through a web interface
- 🔍 Semantic search across document content
- 🤖 AI-powered question answering based on document context
- ⚡ Real-time processing and response generation
- 🔒 Secure API key management via environment variables
- 📊 Display of source document chunks used for answers

## Installation Guide

### Prerequisites
- Python 3.8 or higher
- OpenAI API key

### Step 1: Create a virtual environment and install dependencies

Using `venv`:
```bash
python3 -m venv .ragvenv
source .ragvenv/bin/activate
pip install -r requirements.txt
```

### Step 2: Run streamlit on localhost

```bash
streamlit run chatbot_RAG.py
```