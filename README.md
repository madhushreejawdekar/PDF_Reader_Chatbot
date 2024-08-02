# PDF_Reader_Chatbot
# README

## Project Overview

This project is a web-based application that allows users to upload a PDF file, extract its content, and ask questions about the content. The application uses Flask for the backend, pdfplumber for extracting text from PDFs, and Gemini AI for generating answers to user queries.

## Features

1. **Upload PDF Files**: Users can upload PDF files to the server.
2. **Extract Text**: The content of the uploaded PDF is extracted and saved as a text file.
3. **Ask Questions**: Users can ask questions about the extracted text, and the application will provide answers using the Gemini AI model.

## Files and Directories

- **`app.py`**: The main Flask application file that handles routing and backend logic.
- **`index.html`**: The landing page where users can upload PDF files.
- **`ask_question.html`**: The page where users can enter their questions after uploading a PDF.
- **`ans.html`**: The page where the answers to the user's questions are displayed.
- **`uploads/`**: Directory where uploaded PDF files and their corresponding extracted text files are stored.

## Setup and Installation

1. **Clone the Repository**
   ```sh
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Dependencies**
   Make sure you have Python installed. Then, install the required packages:
   ```sh
   pip install Flask pdfplumber google-generativeai
   ```

3. **Configure API Key**
   Replace `YOUR_API_KEY` in `app.py` with your Gemini AI API key.

4. **Run the Application**
   Start the Flask development server:
   ```sh
   python app.py
   ```

5. **Access the Application**
   Open your web browser and go to `http://127.0.0.1:5000/`.

## Usage

1. **Upload a PDF File**: Navigate to the upload page and select a PDF file to upload.
2. **Ask a Question**: After the file is processed, you will be redirected to a page where you can enter your question.
3. **View the Answer**: The answer will be displayed on the page after processing.

## Error Handling

- If there are issues with the file upload (e.g., no file selected, invalid file type), appropriate error messages will be displayed.
- If there is an issue extracting text or generating an answer, the error message will be displayed on the screen.

