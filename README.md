# ChatWithPDFs
A Langchain based LLM application built to chat with multiple PDFs at the same time.

## Introduction
Langchain based LLM application to chat with multiple PDFs at the same time. Currently chatting with documents, especially with multiple documents is present only in the Paid versions of the AI tools available, like ChatGPT. While some other LLM applications like ChatPDF also provide a similar service to chat with PDF, it can only answer questions from a single PDF at a time. Moreover on the free tier of this application, you can only upload and chat with a maximum of two PDFs in a day. This application is developed to overcome this challenge and make this feature available to everyone who wants to read/reference from multiple PDFs at the same time at zero cost! Very useful to students who are looking to cramp their study materials at the last minute and score good grades. This application can handle any number of files (tested with a maximum of 20 PDFs) each of maximum size 200MB. This is a pretty good number to start with for an LLM PDF chat app.

The application is hosted on the Streamlit app community to be accessible to everyone online.

## TechStack
This application uses the following techstack to achieve the desired results:
Langchain - LLM orchestration framework
FAISS (Facebook AI Similarity Search) - Open Source Vector Database
Google Gemini Pro - Pre trained General Large Language Model for 
PyPDF2 - Open Source pure-python library for working with PDFs
Streamlit - Open Source python library to host the application as a Web App

## How does the app work:
Go to the app website, upload your files and submit for it to process
Now, in the chat pane, ask your desired questions. You can write any prompts to the app!

What happens in the app:


## How to run it locally:

For this application to work on your end, clone the repo, run the command,
cp env.sample .env

After that go to https://aistudio.google.com/library and generate a Google API key and paste it in the file.

Run the app
streamlit run app.py
