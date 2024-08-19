# RAG-based Question Answering System with HybridSearch , Reranking and Compression

This project implements a Retrieval-Augmented Generation (RAG) system for question-answering, combining multiple retrieval techniques with reranking and contextual compression to optimize the relevance and accuracy of responses.

## Overview

In this project, we build a sophisticated question-answering system using the following components:

- **RAG (Retrieval-Augmented Generation)**: This technique combines document retrieval and generation to answer questions. It first retrieves relevant documents and then uses a language model to generate answers based on the retrieved content.
  
- **BM25Retriever**: A sparse retrieval method based on the BM25 algorithm. It is used to retrieve a broad set of relevant documents based on the query.

- **Cohere Reranking**: A deep learning-based model provided by Cohere that reorders the initially retrieved documents, ensuring that the most relevant documents are prioritized.

- **ContextualCompressionRetriever**: This retriever further refines the retrieval process by focusing on the most relevant sections of documents, effectively compressing the information that is passed to the language model.

- **EnsembleRetriever**: Combines the outputs of multiple retrieval methods (e.g., BM25 and vector-based retrieval) to improve the breadth and relevance of the retrieved documents.

- **RetrievalQA Chain**: A hybrid chain that integrates retrieval and language model capabilities to generate high-quality, contextually accurate answers.


