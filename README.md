# AI Research Idea Generator & Novelty Validator

An intelligent agent that generates research ideas, searches scientific
literature, evaluates novelty using embeddings, and produces a structured
research blueprint. Built for the **Google AI Agents Intensive Course**.

## Features
- Generate 3 unique research ideas based on a user prompt
- Retrieve related papers using ArXiv / Semantic Scholar APIs
- Embed abstracts and compute similarity using Sentence-Transformers
- Score novelty (0–100) with transparent explanation
- Generate a research blueprint (problem, method, datasets, metrics)
- End-to-end demonstration via Kaggle Notebook
## Architecture
User Prompt → Idea Generator → Literature Search → Embedding Similarity → Novelty Scoring → Blueprint
Generator → Output

### Components
- **Idea Generator (LLM)** — Produces candidate directions
- **Search Tools** — ArXiv / Semantic Scholar clients
- **Embeddings Module** — Converts abstracts to vectors
- **Novelty Engine** — Ranking + heuristics
- **Blueprint Generator** — Research summary + plan
## Repository Structure

/ (root) ├── README.md ├── requirements.txt ├── notebooks/ │ └── demo_notebook.ipynb
├── src/ │ ├── idea_gen.py │ ├── search_tools.py │ ├── embeddings.py │ ├── novelty.py │
├── blueprint.py │ └── planner.py └── tests/ ├── test_search.py └── test_novelty.py 

## Installation
```bash
pip install -r requirements.txt
