# Legal-Document-Chatbot-Using-Gemini_Pro

## Overview
This project presents a Legal Document Analysis Chatbot designed to automate the process of analyzing legal documents. By leveraging modern Natural Language Processing (NLP) techniques, the solution aims to provide real-time insights from legal texts such as bail eligibility and penalties, thus facilitating faster and more accurate decision-making for legal professionals.

The chatbot utilizes Google Generative AI embeddings for text understanding, combined with FAISS (Facebook AI Similarity Search) for efficient retrieval of relevant information. The primary goal is to minimize the manual effort spent on document review, reducing errors and processing time while maximizing the accuracy of legal decision support.

## Key Features
1) PDF Text Extraction: The application supports multiple PDF uploads, extracts text from each document, and prepares it for further analysis.
2) Text Chunking: The text is split into manageable chunks using the RecursiveCharacterTextSplitter to ensure efficient processing and retrieval.
3) Text Embeddings: Each chunk of text is converted into vector embeddings using Google Generative AI Embeddings. These embeddings are used for semantic search and analysis.
4) FAISS Vector Store: The project uses FAISS, an open-source vector search library by Facebook, to store and index the text embeddings. This allows for fast and scalable similarity search on legal texts.
5) Conversational Interface: The chatbot can answer legal questions by retrieving relevant document sections, providing users with clear and accurate responses based on the context of the documents.

## How It Works
Users upload PDF files through the Streamlit interface.
The system extracts the text from the PDFs, chunks the text into sections, and generates vector embeddings for each chunk using Google Generative AI.
These embeddings are stored in FAISS, enabling fast similarity search.
The user can ask legal questions, and the chatbot will search for the most relevant sections of the documents, providing answers using a custom PromptTemplate.

## Technology Stack
1) Python: Core language used for development.
2) Streamlit: Provides the web interface for user interaction, file uploads, and question-answering.
3) PyPDF2: Library used for PDF text extraction.
4) Langchain: A framework to handle document chunking, chain management, and prompt creation.
5) FAISS: An open-source library for efficient similarity search and clustering of dense vectors.
6) Google Generative AI Embeddings: Used for generating vector embeddings from text.
7) dotenv: For environment variable management (e.g., API keys).

## Business Use Case
The primary business problem this solution addresses is the time-consuming and error-prone process of manually reviewing large volumes of legal documents to assess penalties and bail eligibility. By automating this task, legal professionals can focus on strategic decisions, improving operational efficiency, minimizing compliance risks, and maximizing legal decision support.


