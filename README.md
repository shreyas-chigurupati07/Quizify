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
1. A numbered list
              1. A nested numbered list
              2. Which is numbered
          2. Which is numbered

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

## Installation

### Prerequisites

	•	Python 3.8 or higher
	•	pip (Python package manager)
	•	Google Cloud credentials (for the embedding service)

## Usage

### Generating a Quiz

	1.	Upload the PDF documents you want to generate quizzes from.
	2.	Enter the topic for the quiz.
	3.	Specify the number of questions you want to generate.
	4.	Click “Submit” to generate the quiz.

### Taking the Quiz

	•	Navigate through the quiz using the “Next Question” and “Previous Question” buttons.
	•	Select an answer for each question and receive instant feedback on your selection.
	•	View explanations for the correct answers.

## Project Development

### Task Breakdown

Each task in the project is a building block that contributes to the overall functionality of the Quizify application. Below is a brief description of each task:

	1.	Task 3: Document ingestion and text processing.
	2.	Task 4: Embedding generation using a pre-trained model.
	3.	Task 5: Creation and management of Chroma collections for storing processed data.
	4.	Task 8: Automated quiz question generation based on the processed text.
	5.	Task 9: Management of quiz questions and user interaction.
	6.	Task 10: Integration of all components into a Streamlit application for end-to-end quiz generation and management.
