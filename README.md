# 🎓 Mini RAG Scholarship Chatbot

A Retrieval-Augmented Generation (RAG) chatbot that answers questions about scholarship eligibility, application procedures, required documents, and funding.

## Overview

This project combines semantic document retrieval with a generative AI model to provide answers grounded in a small collection of scholarship documents.

## Technologies Used

* Python
* Google Colab
* Sentence Transformers
* NumPy
* Google Gemini API
* Gradio

## How It Works

1. Scholarship documents are stored as a small document collection.
2. Sentence Transformers converts the documents into vector embeddings.
3. A user's question is converted into an embedding.
4. The system retrieves relevant documents using similarity scores and topic-based reranking.
5. Gemini generates an answer based on the retrieved information.
6. Gradio provides an interactive chatbot interface with supporting sources.

## Features

* Semantic document retrieval
* Topic-based document reranking
* AI-generated answers grounded in retrieved documents
* Supporting source display
* Interactive Gradio interface
* Handling of questions whose answers are missing from the available documents

## Project Notebook

Open `Mini_RAG_Chatbot.ipynb` to explore the implementation and run the project in Google Colab.

## Setup

1. Open the notebook in Google Colab.
2. Install the required Python packages.
3. Configure your Gemini API key in Google Colab Secrets using the name `GEMINI_API_KEY`.
4. Run the notebook cells in order.
5. Launch the Gradio interface.

## Dataset

The current implementation uses a small collection of sample scholarship documents. The information is intended for demonstrating the RAG workflow and should not be treated as verified scholarship guidance.

## Future Improvements

* Expand the scholarship document collection.
* Improve retrieval accuracy.
* Add conversation memory.
* Improve the chatbot interface.
* Deploy the application for persistent public access.
