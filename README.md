# PDF Chat Agent

A highly intuitive and interactive PDF Chat Agent designed to assist users in querying and extracting information from PDFs in real time. This project leverages natural language processing and advanced search capabilities to deliver accurate and context-aware responses from uploaded documents.


## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Project Architecture](#project-architecture)
5. [Setup and Installation](#setup-and-installation)
6. [Usage](#usage)
7. [Contributing](#contributing)



## Overview

The **PDF Chat Agent** allows users to upload PDF files and interact with them using natural language queries. The application processes the document, extracts meaningful content, and provides relevant answers, making document analysis and navigation seamless.



## Features

- **Interactive Chat**: Query PDFs using natural language.
- **Efficient Parsing**: Processes complex documents with ease.
- **Context-Aware Responses**: Provides answers based on the document's content.
- **Multi-File Support**: Handles multiple PDFs in one session.
- **User-Friendly Interface**: Simple and intuitive design.



## Technologies Used

- **Python**: Backend logic and natural language processing.
- **Flask**: Lightweight framework for building the web application.
- **PyPDF2 / PDFplumber**: PDF parsing and text extraction.
- **OpenAI API**: Natural language processing for query understanding.
- **JavaScript**: Enhancing frontend interactivity.
- **HTML/CSS**: User interface and styling.



## Project Architecture

The following illustrates the architecture of the PDF Chat Agent:

```plaintext
Client (Browser)
  |
  |---> Frontend (HTML, CSS, JavaScript)
        |---> File Upload
        |---> Query Interface
        |---> Results Display
  |
  |---> Backend (Flask API)
        |---> File Handling
        |---> Query Processing
              |---> PDF Parser (PyPDF2/PDFplumber)
              |---> OpenAI API Integration
              |---> Response Generation
        |---> Session Management
  |
  |---> Storage
        |---> Uploaded PDF Files
        |---> Temporary Processed Data
```



## Setup and Installation

### Prerequisites

Ensure the following software is installed on your system:
- Python 3.8 or later
- pip (Python package manager)

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/BhawnaMehbubani/PDF-Chat-Agent.git
   cd PDF-Chat-Agent
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables for the OpenAI API key:
   ```bash
   export OPENAI_API_KEY='your_api_key_here'
   ```

5. Run the application:
   ```bash
   python app.py
   ```

6. Open your browser and navigate to `http://127.0.0.1:5000`.



## Usage

1. **Upload PDF**: Drag and drop or upload your PDF file via the interface.
2. **Ask Questions**: Type queries related to the uploaded document.
3. **Get Responses**: View context-aware answers from the PDF content.



## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit changes: `git commit -m "Add new feature"`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.

