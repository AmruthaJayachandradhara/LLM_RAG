# LLM_RAG - Application for Interacting with Our Documents via Chat.

# Overview

This project demonstrates a document retrieval and question-answering system using ChromaDB for vector storage and OpenAI's embedding and chat models for processing and answering queries.

# Features

Loads and processes text documents from a directory

Splits documents into smaller chunks for better retrieval

Generates embeddings using OpenAI's text-embedding-3-small model

Stores embeddings in a persistent ChromaDB instance

Queries the database for relevant document chunks

Uses OpenAI's GPT model to generate responses based on retrieved context

# Setup and Installation : Prerequisites

1.Python 3.x

2.An OpenAI API key

3.Required Python libraries (install using requirements.txt)

# How It Works

1. Load Documents : Documents are read from a specified directory (./news_articles). The script loads .txt files and prepares them for processing.

2. Split Documents into Chunks : To ensure efficient retrieval, documents are split into smaller overlapping chunks of 1000 characters.

3. Generate Embeddings : Each chunk is transformed into an embedding vector using OpenAI’s text-embedding-3-small model.

4. Store in ChromaDB : The embeddings are stored in a persistent ChromaDB instance for efficient similarity search.

5. Querying Documents : When a user asks a question, the system retrieves relevant document chunks from ChromaDB based on semantic similarity.

6. Generate a Response : Using retrieved chunks as context, OpenAI’s GPT model generates a concise response.


