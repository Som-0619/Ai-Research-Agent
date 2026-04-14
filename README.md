# Ai-Research-Agent (Offline)

An intelligent, fully offline research assistant that enables semantic search, paper recommendation, and summarization over scientific literature using natural language queries.

# Overview

This project builds a lightweight AI-powered research assistant that helps users explore academic papers without relying on external APIs or paid services.

Using natural language input, the system retrieves the most relevant research papers, ranks them by similarity, and provides concise summaries.

# Features
 Semantic Search Engine
Query research papers using natural language
 TF-IDF + Cosine Similarity
Efficient document ranking without deep learning
 Paper Recommendation System
Suggests similar papers based on content
 Extractive Summarization
Generates short summaries from abstracts
 Fully Offline System
No API keys, no billing, no external dependencies
 Lightweight & Efficient
Handles large datasets using sampling and preprocessing

# Dataset

This project uses the arXiv research papers dataset from Kaggle.

Format: JSON / JSONL

To optimize performance, only a subset of the dataset is used during runtime.

# Tech Stack
Python
Pandas – data handling
Scikit-learn – TF-IDF + similarity
NLTK – text preprocessing & summarization

# How It Works
Data Loading
JSON dataset is loaded and cleaned
Relevant fields (title, abstract) are extracted
Preprocessing
Lowercasing, stopword removal, noise cleaning
Vectorization
Text is converted into TF-IDF vectors
Search
User query is vectorized
Cosine similarity finds the most relevant papers
Recommendation
Similarity between documents suggests related papers
Summarization
Extracts key sentences from abstracts

# Installation
```
git clone https://github.com/your-username/ai-research-agent.git
cd ai-research-agent
pip install -r requirements.txt
```
# Usage

Run the notebook or execute the script:

python main.py

Then enter your query:

deep learning for image classification

# Example Output
Result 1:
Title: Deep Learning for Image Recognition
Score: 0.87
Abstract: ...

# Future Improvements
 Replace TF-IDF with semantic embeddings (Sentence Transformers)
 Build a Streamlit web interface
 Add PDF upload + document chat
 Implement hybrid search (keyword + semantic)
 Optimize performance using indexing (FAISS)
 
# Limitations
Uses TF-IDF (not deep semantic understanding)
Performance depends on dataset size
Summarization is extractive (not generative)

# Motivation

Most research tools rely on paid APIs or heavy infrastructure.
This project proves that useful AI systems can be built locally, efficiently, and cost-free.

# Author

Soumyajit (CSE - Data Science)
Passionate about AI systems, ML engineering, and building real-world projects.

# License

This project is open-source and available under the MIT License.

# Reality Check (Straight Talk)

This README is:

clean ✅
professional ✅
recruiter-friendly ✅
