# Corrective-RAG
An Implementation of this paper - https://arxiv.org/pdf/2401.15884 using LangChain and LangGraph

### Requirements
- Large Language Model (Change it in models/LLM. By default it used phi3 in ollama)
- Embeddings Model (Change it in models/EM. By default it uses nomic-embed-text in ollama)
- Python 3.10 (use other versions at your own risk) (skip if using docker)
- Python libraries mentioned in requirements.txt (skip if using docker)

### Setup
- Copy the repository
- Use indexer.ipynb to crete FAISS index of your files.
- Paste index.faiss and index.pkl files to index folder.
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
