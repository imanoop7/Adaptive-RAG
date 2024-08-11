# Adaptive RAG

This repository contains the implementation of an Adaptive Retrieval-Augmented Generation (RAG) system using a combination of LangChain and Streamlit, specifically leveraging the PHI3 model for text generation and the Tavily API for web search. The goal is to create a multi-PDF chatbot that can intelligently route user questions to either a vector store or web search, based on the content of the question.

## Overview

The `Adaptive RAG` project demonstrates how to implement an adaptive RAG system using LangChain components and the Streamlit library. This project allows users to upload multiple PDF files, which are processed and split into text chunks. The system then uses these chunks to create a vector store and employs the PHI3 model to generate relevant answers to user queries. Additionally, the project integrates a web search tool to handle queries that are not well-suited for vector store retrieval.

## Requirements

To run this project, you need the following dependencies:

- Python 3.8+
- LangChain
- Streamlit
- Tavily API Key
- HuggingFaceBgeEmbeddings
- Chroma VectorStore
- PyPDFLoader

## Installation

- Clone the repository and install the required packages:
    - cd Adaptive-RAG
    - pip install -r requirements.txt

## Usage
1. Set up Environment Variables: Create a .env file in the project directory and add your Tavily API key.
    `TAVILY_API_KEY=your_tavily_api_key`

2. Run the Streamlit Application:
    ```bash
    streamlit run adaptive-RAG.py

3. Upload PDF Files: Use the Streamlit interface to upload one or more PDF files.

4. Ask Questions: Enter your questions in the provided input field to receive answers based on the uploaded PDFs or web search results.

## Project Structure
`adaptive-RAG.py`:  The main Streamlit application script..
`requirements.txt`: File listing all the dependencies for the project.
`.env`: create a environment variables file containing the Tavily API key.


## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements, bug fixes, or suggestions.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---
Happy coding! If you have any questions or need further assistance, feel free to open an issue.
---