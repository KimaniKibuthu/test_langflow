# Test Langflow
In this repo, we instantiate langflow and play with it.

For this usecase, we build a RAG that reads our pdf document.
## General Workflow
```diagram
Start
 ↓
Ingest PDF Document
 ↓
Split Document
 ↓
Embed Text Chunks (Create Vectors)
 ↓
Store Embeddings in Vector Database
 ↓
Create Retriever
 ↓
End
```

## Usage
To use, first clone the repo, then:

1. Ensure you have python 3.10

    ```bash
    pyenv install 3.10.11
    pyenv global 3.10.11
    ```	

2. Install the requirements:

    ```bash
    pip install poetry 
    poetry config virtualenvs.in-project true
    poetry install --no-root
    poetry shell
    ```	

3. Run langflow:

    ```bash
    langflow run
    ```	