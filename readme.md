# LLaMA 2 RAG Chatbot with Pinecone and OpenAI

This repository contains a Jupyter notebook implementation of a Retrieval-Augmented Generation (RAG) system that integrates LLaMA 2, Pinecone vector database, and OpenAI embeddings.

## Project Overview

This project demonstrates how to build a sophisticated RAG system that enhances Large Language Model responses with context from a specialized dataset. The system:

1. Processes and embeds document chunks using OpenAI's embedding model
2. Stores these embeddings in a Pinecone vector database 
3. Retrieves relevant context based on user queries
4. Generates accurate, context-aware responses using a language model

## Key Components

- **Vector Database**: Pinecone serverless index with 1536-dimensional vectors
- **Embedding Model**: OpenAI's text-embedding-ada-002
- **Language Model**: LLaMA 2 (via API integration)
- **Document Processing**: Efficient batch processing with progress tracking

## Getting Started

### Prerequisites

- Python 3.8+
- OpenAI API key
- Pinecone API key
- Access to LLaMA 2 API

### Installation

```bash
pip install pinecone-client openai pandas tqdm langchain
```

### Usage

1. Set up your API keys in the notebook
2. Run the cells sequentially
3. Use the chatbot interface to interact with the RAG system

## Features

- **Efficient Data Processing**: Batch processing to handle large document collections
- **Semantic Search**: Find relevant content based on meaning, not just keywords
- **Context-Aware Responses**: Generate answers grounded in specific document knowledge
- **Memory Management**: Process large datasets without overwhelming system resources

## Example Use Cases

- Question-answering over specialized document collections
- Creating domain-specific assistants with access to proprietary knowledge
- Building customer support systems with accurate information retrieval

## Credits

This project was created following the [DataCamp course on Building RAG Applications](https://www.datacamp.com/datalab/w/4b77144b-99c9-414f-91a5-e000c780aac1/edit).
