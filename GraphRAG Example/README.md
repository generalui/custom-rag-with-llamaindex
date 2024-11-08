# GraphRAG vs. Baseline RAG: Solving Multi-Hop Reasoning in LLMs

This repository contains the source code for the article ["GraphRAG vs. Baseline RAG: Solving Multi-Hop Reasoning in LLMs"](https://www.genui.com/resources/graphrag-vs.-traditional-rag-solving-multi-hop-reasoning-in-llms).

## Prerequisites

- Python 3.11+
- An OpenAI API key

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

4. Edit `.env` file and add your API key:
- `OPENAI_API_KEY`: Your OpenAI API key

## Running the Demo

1. Open `main.ipynb`

2. Run all cells to see the demo in action

The notebook demonstrates:
- Initial setup and utility functions for response handling
- Loading and parsing a corpus of articles
- Construction of a GraphRAG index using LlamaIndex
- Construction of a traditional Vector RAG index for comparison
- Visualization of the knowledge graph (viewable in `knowledge_graph.html`)
- Comparison of both approaches through multiple test questions
- Performance analysis showing GraphRAG's superior accuracy in multi-hop reasoning tasks
 