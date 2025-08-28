# multimodal-rag-fashion: Multimodal RAG for Fashion Analysis

**Interactive Web App | Multimodal Retrieval-Augmented Generation (RAG) | Llama 3.2 Vision Instruct**

---

## Overview

**multimodal-rag-fashion** is an interactive web application that combines **computer vision, vector similarity search, and large language models (LLM)** to perform detailed, catalog-style fashion analysis from images. Users can upload any fashion photo and receive **AI-generated insights** about clothing items, style elements, and similar items at different price points.  

This project showcases a **complete multimodal RAG pipeline**, integrating visual inputs with structured fashion datasets to provide actionable insights in real time. The dataset is inspired by **Taylor Swift's iconic outfits**, demonstrating how to connect visual inputs with structured metadata for precise identification of garments, accessories, and styling elements.

---

## Features

- **Multimodal RAG pipeline:** Combines images with LLMs for context-augmented responses  
- **Vector similarity search:** Finds visually similar items using precomputed embeddings (`swift-style-embeddings.pkl`)  
- **Interactive Web Interface:** Built with **Gradio** for real-time user interaction  
- **Modular architecture:** Clean separation of models (`models/`), utilities (`utils/`), and example images (`examples/`)  
- **Scalable & Extensible:** Easy to update with new datasets or LLM models  

---
## Installation

Clone the repo
```bash
git clone https://github.com/Azihadadi/multimodal-rag-fashion.git
cd multimodal-rag-fashion
pip install -r requirements.txt
```

Run the Gradio app:
```bash
python app.py
```
Open the link provided by Gradio in your browser to start using the app.

## Project Structure
```
multimodal-rag-fashion/
│
├── app.py                     # Main Gradio app
├── config.py                  # Configuration file
├── requirements.txt           # Dependencies
├── swift-style-embeddings.pkl # Precomputed embeddings
│
├── models/
│   ├── image_processor.py     # Image encoding & feature extraction
│   ├── llm_service.py         # LLM interaction logic
│
├── utils/
│   ├── helpers.py             # Utility functions (preprocessing, logging)
│
├── examples/                  # Sample images
│
└── README.md                  # Project documentation
```
## Tech Stack

- **Languages:** Python 3.10+  
- **AI/ML Frameworks:** PyTorch, Hugging Face Transformers  
- **LLM:** Llama 3.2 Vision Instruct  
- **Retrieval & RAG:** FAISS / Vector DB, LangChain, Retrieval-Augmented Generation  
- **Web Interface:** Gradio  
- **Utilities:** NumPy, Pandas, Matplotlib, Seaborn  
- **Environment:** Linux, VSCode/Jupyter

## Future Improvements

- Add **multi-user support** for the web app  
- Integrate with **e-commerce APIs** for live product recommendations  
- Extend dataset to include **more fashion styles and categories**  
- Optimize LLM responses for **faster inference and scalability**  
- Add **automated testing and CI/CD pipelines** for reproducibility  
- Enhance the UI/UX with **advanced Gradio components**  

