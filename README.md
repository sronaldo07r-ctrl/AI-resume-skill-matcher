# AI Resume Skill Matcher using NLP

This project uses Natural Language Processing (NLP) to compare a resume with a job description and calculate a skill match percentage.

## Tech Stack
- Python
- Scikit-learn
- TF-IDF
- Cosine Similarity

## How It Works
1. Reads resume and job description text files
2. Converts text into numerical vectors using TF-IDF
3. Computes similarity score using cosine similarity
4. Outputs a skill match percentage

## Real-World Relevance
This project demonstrates how NLP techniques can be applied to automate resume screening and improve hiring efficiency.

## Learning Outcomes
- Text vectorization using TF-IDF
- Similarity measurement with cosine similarity
- Practical NLP pipeline in Python

## How to Run
```bash
pip install -r requirements.txt
python skill_matcher.py
