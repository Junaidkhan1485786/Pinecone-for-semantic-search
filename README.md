# Pinecone-for-semantic-search
perform a simple semantic search using pincone 



# Pinecone Semantic Search

This project demonstrates semantic search using Pinecone and Hugging Face's sentence-transformers library.

## Features

- **Semantic Search**: Find relevant information based on the meaning of queries.
- **Pinecone Integration**: Efficiently store and query embeddings with Pinecone.

## Setup

1. **Clone the Repository**

    ```bash
    git clone https://github.com/your-username/pinecone-semantic-search.git
    cd pinecone-semantic-search
    ```

2. **Create a Virtual Environment**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

4. **Configure the Project**

    Update `config.py` with your Pinecone API key and environment:

    ```python
    # config.py
    PINECONE_API_KEY = 'your-pinecone-api-key'
    PINECONE_ENVIRONMENT = 'your-pinecone-environment'
    INDEX_NAME = 'semantic-search'
    MODEL_NAME = 'sentence-transformers/all-MiniLM-L6-v2'
    ```

5. **Run the Script**

    Execute the `semantic_search.py` script:

    ```bash
    python semantic_search.py
    ```

## How It Works

1. **Initialize Pinecone**: Connect using API key and environment.
2. **Create/Connect Index**: Set up or use an existing Pinecone index.
3. **Load Model**: Use `sentence-transformers` to load the model.
4. **Upsert Data**: Load and insert data into Pinecone.
5. **Query and Retrieve**: Perform search queries and display results.
