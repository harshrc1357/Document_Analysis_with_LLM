## Document Analysis with LLM
Overview
This project demonstrates a comprehensive approach to document analysis using Large Language Models (LLMs). It provides a step-by-step workflow for extracting, analyzing, and interacting with text from PDF documents.

Installation
To use this project, you'll need to install the following packages:
1. pdfplumber
2. transformers
3. nltk

Usage
Step 1: Extract Text from PDF
The first step involves extracting text content from PDF documents. The system uses pdfplumber to process each page and compile the text into a single document.

Step 2: Summarize the Document
After extraction, the text is summarized using a transformer-based summarization model (t5-small). This provides a concise overview of the document's key points.

Step 3: Split the Document into Passages
The document is then divided into manageable passages based on sentence boundaries. This segmentation ensures that each passage maintains contextual coherence while being small enough for efficient processing.

Step 4: Generate Questions from Document Content
For each passage, the system automatically generates relevant questions using a text-to-text generation model. This creates a comprehensive set of questions that cover the document's content.

Step 5: Answer Generated Questions
Finally, the system uses a question-answering model to provide accurate answers to the generated questions, creating a complete question-answer set based on the document.

Models Used
1. Text Summarization: t5-small
2. Question Generation: valhalla/t5-base-qg-hl
3. Question Answering: deepset/roberta-base-squad2
