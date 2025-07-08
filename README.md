## 📖 About

This repository contains all the code and notebooks used to build a Retrieval-Augmented Generation (RAG) system from scratch, as described in the Medium article [Building Retrieval-Augmented Generation (RAG) from Scratch](https://medium.com/red-buffer/building-retrieval-augmented-generation-rag-from-scratch-74c1cd7ae2c0).  
You’ll find:

- **`rag_from_scratch.py`** – a pure-Python implementation of:
  - Document chunking (with customizable token limits)
  - Embedding computation (via BAAI’s BGE and/or OpenAI)
  - Cosine-similarity retrieval of top-k chunks
  - Chaining retrieved context into an LLM prompt
- **`RAG_From_Scratch.ipynb`** – a Colab notebook walkthrough  
- Instructions on how to wire everything up with your own API keys

## 🔧 Prerequisites

- Python 3.8+
- PyTorch
- `transformers`, `langchain-openai`
- An OpenAI API key (if you want to use GPT-3.5/4 as the LLM)

## 🚀 Getting Started

```bash
git clone https://github.com/YourGitHubUsername/your-rag-repo.git
cd your-rag-repo
pip install -r requirements.txt
# populate `documents/` with your text files...
python rag_from_scratch.py
