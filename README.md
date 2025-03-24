# AI Resume Screening & Candidate Ranking System

This project is a web-based AI system designed to help recruiters efficiently screen and rank resumes based on their relevance to a provided job description. It leverages NLP techniques such as TF-IDF vectorization and cosine similarity to automate and simplify the resume shortlisting process.

---

## Features

- Upload multiple resumes in PDF format.
- Input any custom job description.
- Extract text from resumes using PDF parsing.
- Compute similarity scores between resumes and job description.
- Display ranked resumes based on their relevance.

---

## Technologies Used

- **Python 3.10+**
- **Streamlit** for the web interface
- **PyPDF2** for extracting text from PDF resumes
- **scikit-learn (TfidfVectorizer & cosine_similarity)** for text vectorization and similarity calculation
- **pandas** for data handling

---

## Installation

1. **Clone the repository:**

```bash
git clone <repository_link>
cd <repository_folder>
```

2. **Create a virtual environment (optional but recommended):**

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install required packages:**

```bash
pip install -r requirements.txt
```

---

## How to Run

1. **Convert notebook (if needed):**

```bash
jupyter nbconvert --to script resume_ranking.ipynb
```

2. **Run the Streamlit app:**

```bash
streamlit run resume_ranking.py
```

3. **Access the app:**

The app will be available at `http://localhost:8501`.

---

## File Structure

```
├── resume_ranking.ipynb          # Jupyter notebook version
└── README.md                     # Project documentation
```

---

## How It Works

1. The recruiter enters a job description in the provided text area.
2. Resumes in PDF format are uploaded via the file uploader.
3. Text is extracted from each resume using PyPDF2.
4. TF-IDF Vectorizer converts text data into vectors.
5. Cosine similarity is computed between the job description and each resume.
6. Results are displayed in a ranked format with scores.

---

## References

1. Christopher D. Manning, Prabhakar Raghavan, Hinrich Schütze, “Introduction to Information Retrieval”, Cambridge University Press, 2008.
2. Gerard Salton, A. Wong, C. S. Yang, “A Vector Space Model for Automatic Indexing”, Communications of the ACM, Volume 18, Issue 11, 1975.
3. Kavita Ganesan, ChengXiang Zhai, “Opinion-Based Entity Ranking Using TF-IDF and Cosine Similarity”, IEEE/WIC/ACM International Conference on Web Intelligence, 2012.
4. Parul Sharma, Sonal Gupta, “Resume Shortlisting System Using Natural Language Processing and Machine Learning”, International Journal of Engineering Research & Technology (IJERT), Volume 8, Issue 6, 2019.
5. Sonal Singhal, “Modern Information Retrieval: A Brief Overview”, IEEE Data Engineering Bulletin, Volume 24, No. 4, 2001.
