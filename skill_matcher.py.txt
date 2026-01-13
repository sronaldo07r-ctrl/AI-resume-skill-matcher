from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.metrics.pairwise import cosine_similarity

with open("resume.txt", "r") as f:
    resume = f.read()

with open("job_description.txt", "r") as f:
    job_desc = f.read()

vectorizer = TfidfVectorizer()
vectors = vectorizer.fit_transform([resume, job_desc])

similarity = cosine_similarity(vectors[0:1], vectors[1:2])[0][0]

print("Skill Match Percentage:", round(similarity * 100, 2), "%")
