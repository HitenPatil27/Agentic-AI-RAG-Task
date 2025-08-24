# PDF Question Answering with RAG
### This project implements a Retrieval-Augmented Generation (RAG) system for answering questions based on the content of uploaded PDF documents. It uses a Flask backend with a modern, animated HTML front-end to provide a user-friendly interface for uploading PDFs and querying their content. The system leverages the sentence-transformers library for text embeddings, PyPDF2 for PDF text extraction, and the Groq API for generating responses.
# Features
### PDF Upload: Users can upload PDF files via a web interface.
Query Processing: Ask questions about the PDF content, and the system retrieves relevant text chunks and generates answers.
Aesthetic Design: A responsive, modern UI with animations (fade-in, slide-in, and loading spinners) using Tailwind CSS.
Robust File Handling: Handles temporary files with retry logic to prevent file access errors (e.g., WinError 32 on Windows).
Retrieved Chunks: Displays the top retrieved text chunks with similarity scores for transparency.
Error Handling: User-friendly error messages for invalid inputs or processing failures.

# Usage

Run the Flask Server:
python app.py

The server will start at http://localhost:5000.

Access the Web Interface:

Open a browser and navigate to http://localhost:5000.
Upload a PDF file using the file input.
Enter a question about the PDF content (e.g., "What is the conclusion of this document?").
Click "Submit" to view the generated response and optionally view retrieved text chunks.


# Example Workflow:

Upload a PDF (e.g., a research paper).
Ask a question like "What are the key findings?".
The system processes the PDF, retrieves relevant chunks using cosine similarity, and generates a response via the Groq API.

# ScreenShots
### 1. Upload a PDF.
<img width="1918" height="1011" alt="1" src="https://github.com/user-attachments/assets/6be1500e-ec7c-4b2f-b44e-40740e16e537" />
<img width="1918" height="1007" alt="2" src="https://github.com/user-attachments/assets/33f4582f-b4fe-4b67-a2dc-2315a102717b" />

### 2. Ask a question
<img width="1918" height="1007" alt="3" src="https://github.com/user-attachments/assets/3d9726ed-c5df-4014-b8c0-3c6763f7f44f" />

### 3. Get Result
<img width="1917" height="1012" alt="4" src="https://github.com/user-attachments/assets/4e45a55a-0386-4d3e-bef8-a8e394cc71fe" />




