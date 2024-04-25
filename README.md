# RAG-system Implementation for "Leave No Context Behind” Paper

## Introduction
In this project, we implement a Retrieval-Augmented Generation (RAG) system utilizing the LangChain framework and the power of LLM (Large Language Model) like Gemini 1.5 Pro. The goal is to answer questions related to the "Leave No Context Behind" paper published by Google on April 10, 2024.

## Overview
The RAG system comprises two main parts:

### Part 1: Generating and Storing Embeddings of Documents
This section involves preparing the documents and storing their embeddings for future use. It is executed in Google Colab and involves the following steps:

- **Library Installation:** Install necessary libraries such as Pypdf, LangChain, NLTK, and Chroma.
- **Load PDF and Create Object:** Load the PDF of the "Leave No Context Behind" paper and create its object for processing.
- **Text Splitting:** Split the text using NLTKTextSplitter to segment it into manageable portions.
- **Chunking and Embedding:** Create chunks of text and generate embeddings using an embedding model.
- **Storage:** Store the generated embeddings in ChromaDB for persistence and future use.

### Part 2: Integrating with Streamlit Using VS Code
This section involves integrating the RAG system with Streamlit for a user-friendly interface. The steps include:

- **Connection Setup:** Establish a connection with ChromaDB and convert it to a retriever object for efficient data retrieval.
- **Template Creation:** Develop a chat template for user interaction.
- **Model and Parser Creation:** Implement a chat model, output parser, and embedding model similar to those used in Part 1.
- **User Interaction:** Accept user input, perform queries on the database, and respond back to the user interface with relevant information.

## Resources
- **Paper Link:** [Link to the "Leave No Context Behind" paper](https://arxiv.org/pdf/2404.07143.pdf)
- **Demo Video:** [Demonstration of the RAG system in action](https://youtu.be/wkmtGRDXAIw)
- **Google Colab Link:** [Google Colab notebook for Part 1 implementation](https://colab.research.google.com/drive/1pY_DlH8LJ9ugQ02hPeDCDnA-DG3p_RvE#scrollTo=pQUhnKhkrKWV)
- **LinkedIn Profile:** [Ajay Chaudhary](https://www.linkedin.com/in/chaudharyajay/)
