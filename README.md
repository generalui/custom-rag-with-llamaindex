# Building a custom RAG pipeline with LlamaIndex and Llama3.2

This repository contains the source code for the article ["Building a custom RAG pipeline with LlamaIndex and Llama3.2"](https://www.genui.com/resources/building-a-custom-rag-pipeline-with-llamaindex-and-llama3.2).

## Prerequisites

- Python 3.11+
- A Groq API key
- A LlamaIndex Cloud API key
- A Hugging Face token

## Setup Instructions

1. Create and activate a Python virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate  # On Windows, use: .venv\Scripts\activate
```

2. Install the required packages:

```bash
pip install -r requirements.txt
```

3. Set up environment variables:

```bash
cp .env.example .env
```

4. Edit `.env` file and add your API keys:
- `GROQ_API_KEY`: Your Groq API key
- `LLAMA_CLOUD_API_KEY`: Your LlamaIndex Cloud API key
- `HF_TOKEN`: Your Hugging Face token

## Running the Demo

1. Open `main.ipynb`

3. Run all cells to see the demo in action

The notebook demonstrates:
- Loading and parsing PDF documents
- Creating vector embeddings using Hugging Face models
- Using Groq's LLM for question answering
- Persisting the vector store for future use

## Note

Make sure you have all the required API keys before running the notebook. The demo uses a sample PDF file, but you can modify the code to work with your own documents.