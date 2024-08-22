# Quizify
## AI Quiz Generator
### Overview

Quizify is an AI-powered tool designed to generate and manage quizzes based on provided documents. This tool leverages advanced natural language processing techniques to create multiple-choice questions from any text-based content. It is built using Python and Streamlit, making it both powerful and easy to use. The system is modular, allowing for easy integration and extension of various components.

### Features
-  **Document Ingestion:** Supports ingestion of PDF documents, allowing the system to parse and process text content for quiz generation.
-  **Embedding Generation:** Utilizes Google’s textembedding-gecko model to generate text embeddings that help in understanding the context of the documents.
-  **Quiz Generation:** Automatically generates quizzes based on topics extracted from the provided documents.
-  **Quiz Management:** Enables users to interact with generated quizzes, including answering questions, navigating through the quiz, and receiving feedback.
-  **Streamlit Integration:** Provides a user-friendly interface for generating and taking quizzes, making it accessible to non-technical users.

### Project Structure

The project is divided into several tasks, each encapsulated within its respective module:
-  **Task 3 - Document Processing**\
   Functionality: Handles the ingestion and processing of documents, extracting text content for quiz generation.
-  **Task 4 - Embedding Client**\
   Functionality: Generates text embeddings using the textembedding-gecko model, which are crucial for understanding document content.
-  **Task 5 - Chroma Collection Creator**\
		Functionality: Creates a Chroma collection from the processed document text and embeddings, storing it for later retrieval during quiz generation.
  
-  **Task 8 - Quiz Generator**\
		Functionality: Generates a set of quiz questions based on the provided topic and Chroma collection.
  
-  **Task 9 - Quiz Manager**\
		Functionality: Manages the generated quiz questions, enabling navigation, answer submission, and feedback.
  
-  **Task 10 - Main Application**\
		Functionality: Integrates all the above modules into a cohesive Streamlit application, allowing users to generate and take quizzes interactively.

## Installation

### Prerequisites
-  Python 3.8 or higher
-  pip (Python package manager)
-  Google Cloud credentials (for the embedding service)
### Setup
-  Clone the repo:
```
git clone https://github.com/yourusername/quizify.git
cd quizify

```
-  Install Dependencies: 'pip install -r requirements.txt'
-  Set Up Google Cloud Credentials:
  -  Enure you have a valid Google Cloud project with the textembedding-gecko model enabled.
  -  Set the GOOGLE_APPLICATION_CREDENTIALS environment variable to point to your Google Cloud service account key file.
-  Run the Application:'streamlit run Task_10.py'

## Usage

### Generating a Quiz
-  Upload the PDF documents you want to generate quizzes from.
-  Enter the topic for the quiz.
-  Specify the number of questions you want to generate.
-  Click “Submit” to generate the quiz.

### Taking the Quiz
-  Navigate through the quiz using the “Next Question” and “Previous Question” buttons.
-  Select an answer for each question and receive instant feedback on your selection.
-  View explanations for the correct answers.

## Results
![Screenshot from 2024-08-15 13-52-32](https://github.com/user-attachments/assets/9150306c-8cbc-4121-97d2-9492138c6671)

