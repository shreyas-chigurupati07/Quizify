# Quizify
## AI Quiz Generator
### Overview

Quizify is an AI-powered tool designed to generate and manage quizzes based on provided documents. This tool leverages advanced natural language processing techniques to create multiple-choice questions from any text-based content. It is built using Python and Streamlit, making it both powerful and easy to use. The system is modular, allowing for easy integration and extension of various components.

### Features

	•	Document Ingestion: Supports ingestion of PDF documents, allowing the system to parse and process text content for quiz generation.
	•	Embedding Generation: Utilizes Google’s textembedding-gecko model to generate text embeddings that help in understanding the context of the documents.
	•	Quiz Generation: Automatically generates quizzes based on topics extracted from the provided documents.
	•	Quiz Management: Enables users to interact with generated quizzes, including answering questions, navigating through the quiz, and receiving feedback.
	•	Streamlit Integration: Provides a user-friendly interface for generating and taking quizzes, making it accessible to non-technical users.

### Project Structure

The project is divided into several tasks, each encapsulated within its respective module:

	1.	Task 3 - Document Processing
		Module: DocumentProcessor
		Functionality: Handles the ingestion and processing of documents, extracting text content for quiz generation.
  
	2.	Task 4 - Embedding Client
		Module: EmbeddingClient
		Functionality: Generates text embeddings using the textembedding-gecko model, which are crucial for understanding document content.
  
	3.	Task 5 - Chroma Collection Creator
		Module: ChromaCollectionCreator
		Functionality: Creates a Chroma collection from the processed document text and embeddings, storing it for later retrieval during quiz generation.
  
	4.	Task 8 - Quiz Generator
		Module: QuizGenerator
		Functionality: Generates a set of quiz questions based on the provided topic and Chroma collection.
  
	5.	Task 9 - Quiz Manager
		Module: QuizManager
		Functionality: Manages the generated quiz questions, enabling navigation, answer submission, and feedback.
  
	6.	Task 10 - Main Application
		Module: Task_10.py
		Functionality: Integrates all the above modules into a cohesive Streamlit application, allowing users to generate and take quizzes interactively.

### Installation

### Prerequisites

	•	Python 3.8 or higher
	•	pip (Python package manager)
	•	Google Cloud credentials (for the embedding service)
