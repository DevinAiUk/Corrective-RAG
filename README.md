# Corrective-RAG
An Implementation of this paper - https://arxiv.org/pdf/2401.15884 using LangChain and LangGraph

### Requirements
- Large Language Model (Change it in models/LLM. By default it uses phi3 in ollama. You can use any model supported by langchain.)
- Embeddings Model (Change it in models/EM. By default it uses nomic-embed-text in ollama. You can use any model supported by langchain.)
- Python 3.10 (use other versions at your own risk) (skip if using docker)
- Python libraries mentioned in requirements.txt (skip if using docker)

### Setup
- Copy the repository
- Change LLM and EM in models.
- Use indexer.ipynb to create FAISS index of your files.
- Run the app
  - Locally
    ```
    streamlit run streamlit_app.py
    ```
  - Docker
    ```
    docker build -t corrective-rag .
    docker run -p 8501:8501 corrective-rag
    ```
#### Keywords - RAG, Corrective RAG, CRAG, LangChain, LangGraph, FAISS, Streamlit, Ollama, phi3, DuckDuckGo
