# Question-Answering-with-Structured-Data

## Overview

This project demonstrates various approaches for building a question-answering system using structured data. The system integrates SQL-based models, Retrieval-Augmented Generation (RAG) with CSV data, and TAPAS model fine-tuning for different types of question-answering tasks.

## Ideas Implemented

### Idea-1: SQL-based Model
- **Objective:** Develop a Text-to-SQL generation system using Google Gemini Pro LLM.
- **Dependencies:** `langchain`, `google-generativeai`, `langchain-google-genai`
- **Functionality:** Converts natural language questions into SQL queries and executes them on an SQLite database containing movie and director information.

### Idea-2: RAG-Based Model with CSV Data
- **Objective:** Build a chatbot using Retrieval-Augmented Generation (RAG) with Open Source Mistral LLM and LangChain framework.
- **Dependencies:** `transformers`, `sentence-transformers`, `faiss-gpu`, `langchain`
- **Functionality:** Uses a pre-trained Mistral model to answer questions based on a CSV dataset containing movie information.

### Idea-3: TAPAS Model
- **Objective:** Pre-train TAPAS model on custom data for table-based question answering.
- **Dependencies:** `transformers`, `pandas`
- **Functionality:** Uses TAPAS for answering questions about movie data stored in a CSV file.

## Setup

### Dependencies
Install required Python packages using pip:

```bash
pip install -q -U langchain==0.1.2 google-generativeai==0.5.2 langchain-google-genai==1.0.3 transformers==4.40.2 accelerate==0.30.1 bitsandbytes==0.43.1 huggingface_hub==0.23.0 pypdf==4.2.0 sentence-transformers==2.7.0 faiss-gpu==1.7.2
