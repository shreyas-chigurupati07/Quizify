# Quizify
## AI Quiz Generator

### Overview

This project is designed to create an AI-powered tool that dynamically generates quizzes from user-provided documents. The tool aims to enhance the learning experience by offering instant feedback and detailed explanations, helping students reinforce their understanding of various topics.

### Features

	Document Ingestion & Processing: Upload and process PDFs, converting them into a format suitable for generating quizzes.
	Embedding Creation: Transform processed text into vector embeddings using advanced AI models.
	Chroma Collection: Organize embeddings into collections for efficient quiz generation.
	Dynamic Quiz Generation: Generate quizzes tailored to specific topics with a customizable number of questions.
	User-Friendly Interface: Streamlit-based interface for easy interaction, quiz navigation, and feedback.
	Instant Feedback: Immediate insights into answers with explanations to reinforce learning.

### Tech Stack

	Programming Language: Python
	Frontend Framework: Streamlit
	AI Model: TextEmbedding-gecko@003
	Embedding Management: LangChain
	Data Storage: Chroma Vector Store

### Project Workflow

	1.	Document Ingestion & Processing:
 		Use the DocumentProcessor class to ingest and process PDFs.
   		Extract text from documents for embedding.
	2.	Embedding Creation:
 		Configure the EmbeddingClient with the AI model to convert text into vector embeddings.
   		These embeddings represent the semantic meaning of the text.
	3.	Chroma Collection Creation:
 		Use the ChromaCollectionCreator to group embeddings into collections.
   		These collections serve as the knowledge base for quiz generation.
	4.	Quiz Generation:
 		Generate quiz questions based on the topic and number of questions specified by the user.
   		Store generated questions in a question bank.
	5.	Session State Management:
 		Initialize session state variables to manage quiz progress and user interaction.
	6.	Quiz Display & User Interaction:
 		Display quiz questions and allow users to select answers via the interface.
   		Provide immediate feedback and explanations.

### Installation
