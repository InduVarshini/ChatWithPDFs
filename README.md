# ChatWithPDFs

A LangChain-based LLM application designed to chat with multiple PDFs simultaneously.

You can access the app on 
[https://chatwithmorepdfs.streamlit.app/](https://chatwithmorepdfs.streamlit.app/)

## Introduction

**ChatWithPDFs** is a LangChain-powered application that enables interactive conversations with multiple PDFs at the same time. While existing AI tools, like ChatGPT, offer similar functionality for document interaction, these features are often restricted to paid versions. Tools like ChatPDF allow interactions with PDFs, but typically limit users to one document at a time, and impose strict usage caps on free tiers (e.g., only two PDFs per day).

This application addresses those limitations by providing a free, open-access solution for chatting with multiple PDFs simultaneously. Whether you're a student preparing for exams or someone referencing multiple documents for research, **ChatWithPDFs** makes it easy to handle up to 20 PDFs (each up to 200MB) at once, ensuring a robust experience for diverse use cases.

The app is hosted online via the Streamlit community platform, making it accessible to everyone.

## Features

- **Multi-PDF Interaction**: Chat with multiple PDFs simultaneously, overcoming the restrictions of most free-tier AI tools.
- **High Capacity**: Supports up to 20 PDFs at once, each with a maximum file size of 200MB.
- **Cost-Free Access**: Available at zero cost, making it ideal for students and researchers.
- **Simple Interface**: Upload your files, ask questions, and get answers with ease.

## Tech Stack

This application is built using the following technologies:

- **LangChain**: Framework for orchestrating large language models (LLMs).
- **FAISS (Facebook AI Similarity Search)**: Open-source vector database for efficient document indexing and retrieval.
- **Google Gemini Pro**: Pre-trained general-purpose LLM.
- **PyPDF2**: Python library for extracting and processing PDF content.
- **Streamlit**: Python-based library for building interactive web applications.

## How It Works

### Using the App Online:

1. Visit the app at [https://chatwithmorepdfs.streamlit.app/](https://chatwithmorepdfs.streamlit.app/) 
2. Upload your desired PDF files and submit them for processing.
3. Use the chat pane to ask questions or write prompts related to the uploaded documents.

### Behind the Scenes:

1. Uploaded PDFs are processed to extract and index content using PyPDF2 and FAISS.
2. User prompts are handled by the LLM (Google Gemini Pro), which queries the indexed content for relevant answers.
3. Results are returned in real time, enabling seamless interaction with your documents.

## Running the Application Locally

To run the application on your machine:

1. Clone the repository:
   ```bash
   git clone https://github.com/InduVarshini/ChatWithPDFs.git
   ```
2. Set up environment variables:
   ```bash
   cp env.sample .env
   ```
3. Obtain a Google API key:
   - Visit [Google AI Studio](https://aistudio.google.com/library).
   - Generate an API key and paste it into the `.env` file.

4. Start the application:
   ```bash
   streamlit run app.py
   ```