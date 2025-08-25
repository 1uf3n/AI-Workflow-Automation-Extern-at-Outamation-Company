# AI Workflow Automation for Mortgage Document Processing

## Overview  
This project was developed during my **AI Workflow Automation Externship at Outamation (May – Jul. 2025)**.  
It focuses on building an AI-driven pipeline that automates classification, retrieval, and question answering (QA) for mortgage-related documents. The system integrates **OCR, LlamaIndex, Mistral-7B, and SentenceTransformers** to handle unstructured, multi-page PDFs while ensuring **data privacy, efficiency, and accuracy**.  

## Features  
- **ML Engineering**: Developed a local **RAG (Retrieval-Augmented Generation)** pipeline with **LlamaIndex + Mistral-7B** for offline mortgage document analysis.  
- **OCR Integration**: Automated **document-type detection** using OCR and prompt-based classification.  
- **Semantic Information Retrieval**: Created **vector indexes per document type** with SentenceTransformers, boosting relevance in multi-page PDFs.  
- **System Optimization**: Reduced latency by >30% via GPU layer tuning, token length adjustments, and chunk overlap optimization.  

## Repository Structure  
- `bank_loan.csv`: Raw dataset of loan records  
- `bank_loan_cleaned.csv`: Cleaned dataset after preprocessing  
- `cleaned_image.jpg`: Example scanned image for OCR pipeline  
- `cleaned_text_sample.txt`: OCR-extracted text sample  
- `extracted_loan_data.json`: Structured JSON output from pipeline  

### Code/
- `Advanced PDF Retr...ipynb`: Advanced retrieval with LlamaIndex  
- `Analyze a Scanned PDF.ipynb`: OCR + text extraction workflow  
- `Cleaning Loan Data.ipynb`: Data cleaning and preprocessing  
- `Dataset clean.ipynb`: CSV data cleaning steps  
- `Defining Functions in Python`: Utility functions used across notebooks  
- `Denoise image.ipynb`: Image preprocessing for OCR accuracy  
- `Document Classification Before Retrieval.ipynb`: Document-type classifier  
- `Embeddings and C...Gemini.ipynb`: Embedding generation + Gemini test  
- `Experimenting with L...Performance.ipynb`: Latency and efficiency experiments 

## Tech Stack  
- **Programming**: Python (NumPy, Pandas, PyTorch)  
- **LLM & Retrieval**: LlamaIndex, Mistral-7B, SentenceTransformers  
- **OCR**: Tesseract, PyMuPDF  
- **Visualization**: Matplotlib, Seaborn  
- **Data Storage**: JSON, CSV  

## Workflow  

1. **OCR & Image Preprocessing**  
   - Denoise scanned mortgage documents (`Denoise image.ipynb`)  
   - Extract raw text into `.txt` (`Analyze a Scanned PDF.ipynb`)  

2. **Data Cleaning & Structuring**  
   - Process raw loan dataset (`Cleaning Loan Data.ipynb`, `Dataset clean.ipynb`)  
   - Output structured JSON (`extracted_loan_data.json`)  

3. **Document Classification**  
   - Use OCR metadata + embeddings to classify document type  
   - Notebook: `Document Classification Before Retrieval.ipynb`  

4. **Information Retrieval (RAG Pipeline)**  
   - Build document-specific indexes with SentenceTransformers  
   - Use **LlamaIndex + Mistral-7B** for QA over PDFs  

5. **Optimization & Performance Tuning**  
   - Experiment with token length, overlap, GPU offloading (`Experimenting with L...Performance.ipynb`)  
   - Achieved >30% latency reduction without loss of context quality  

## Results  
- Reduced LLM **response latency by 30%+** through optimized pipeline tuning  
- Improved **retrieval relevance** across 1,000+ multi-page mortgage PDFs  
- Built a **scalable offline RAG system** that protects data privacy while enabling semantic QA  

## Future Work  
- Extend to support **multi-lingual mortgage documents**  
- Integrate with **real-time API** for enterprise deployment  
- Explore **hybrid embedding models** for better semantic coverage  

## Author  
**Rebecca (Lufan Wang)**  
AI Workflow Automation Extern @ Outamation  
- LinkedIn: [(https://www.linkedin.com/in/lufanw )]  
- Email: [1uf3nnn@gmail.com]  
