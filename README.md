📘 AI Research Idea Generator & Novelty Validator










An advanced multi-agent system to generate novel research ideas, evaluate originality using scientific literature, and produce full research blueprints.
🚀 Overview

Researchers, students, and innovators often struggle with the same question:

“Is my research idea truly original?”

This project solves that by using autonomous AI agents that:

Generate high-quality, domain-specific research ideas

Search scientific literature (ArXiv / Semantic Scholar)

Compare ideas to published work using embeddings

Score novelty (0–100) with explanation

Produce a complete research blueprint for the best idea

Built as part of the Google AI Agents Intensive Course, this project showcases multi-agent reasoning, retrieval pipelines, and tool-augmented LLM workflows.

🧠 Key Features
🔍 1. AI-Generated Research Ideas

The LLM Agent produces 3–5 original research directions tailored to the user’s prompt.

📚 2. Scientific Literature Search (ArXiv + Semantic Scholar)

A Search Agent retrieves abstracts, metadata, and keywords from major scientific repositories.

🧮 3. Embedding & Similarity Analysis

Using Sentence-Transformers:

Converts abstracts into vectors

Measures idea similarity

Detects overlap with existing literature

🧪 4. Novelty Evaluation Engine

Each research idea is scored based on:

Factor	Description
Similarity	Cosine similarity to closest papers
Saturation	Number of papers in the domain
Innovation	Uniqueness of problem framing
Feasibility	Technical practicality
Research Value	Impact + contribution potential

Output example:

Novelty Score: 82/100
Why: “Low similarity to current works; unexplored approach in existing literature…”

📘 5. Research Blueprint Generator

Produces a full research plan containing:

Problem statement

Motivation

Methodology

Datasets to use

Evaluation metrics

Implementation outline

Expected challenges

Perfect for academic submissions, thesis beginnings, or research proposals.

🧱 Architecture
User Prompt 
       ↓
Idea Generator Agent 
       ↓
Literature Search Agent (ArXiv / Semantic Scholar)
       ↓
Embedding & Similarity Engine
       ↓
Novelty Scoring Engine
       ↓
Research Blueprint Agent
       ↓
Final Output (JSON / Text / Notebook)

📂 Repository Structure
/ (root)
├── README.md
├── requirements.txt
├── notebooks/
│   └── demo_notebook.ipynb
├── src/
│   ├── idea_gen.py
│   ├── search_tools.py
│   ├── embeddings.py
│   ├── novelty.py
│   ├── blueprint.py
│   └── planner.py
└── tests/
    ├── test_search.py
    ├── test_novelty.py
    └── test_embeddings.py

🛠 Tech Stack
Component	Technology
LLM	Gemini / OpenAI
Agents	LangChain / Custom Agent Layer
Search	ArXiv API, Semantic Scholar
Embeddings	Sentence-Transformers
Similarity	FAISS / sklearn
IDE	Kaggle Notebook
Runtime	Python 3.9+
📦 Installation
pip install -r requirements.txt

▶️ Quick Start Example
from src.planner import run_pipeline

result = run_pipeline("AI for cybersecurity threat detection")
print(result["best_blueprint"])

🧪 Testing
pytest

🧭 Future Work

Add multi-language novelty evaluation

Auto-generate datasets + baselines

Research-graph visualization

Debate-style multi-agent refinement

Web dashboard for interactive evaluation

📘 Course Context

This project was built as the capstone for the
Google AI Agents Intensive Course (2024–2025)
to demonstrate advanced agent workflows and tool-use capabilities.
