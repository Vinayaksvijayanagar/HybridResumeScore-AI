HybridResumeScore AI is an ATS-style resume analysis system that automatically classifies every sentence in a resume into skill categories (ML, NLP, CV, DE, Backend, Experience, Other) and generates a final score showing how strongly the resume aligns with AI/ML roles.

The system uses a hybrid pipeline that combines:

Machine Learning (TF-IDF + Logistic Regression)

Action Verb Detection

Domain Keyword Validation

Confidence Thresholding

Rule-Based Personal/Education Filters

This creates an extremely accurate and clean classification system suitable for HR, hiring platforms, and automation tools.

🚀 Features
✔ Resume Parsing (PDF, DOCX, TXT)

Extracts text from multiple file formats.

✔ Sentence-Level Classification

Each sentence is categorized into:

ML / Modeling

NLP

Computer Vision

Backend

Data Engineering

Experience

Other

✔ Hybrid ML + Rule-Based Model

Stops misclassification with:

Personal info removal

Education line filtering

ML/NLP/CV keyword validation

Confidence threshold

✔ Skill Scoring System

For each resume:

AI/ML Match %

NLP Match %

Python Match %

Years of Experience

Experience Score %

Overall Score %

✔ ATS-Level Clean Output

Outputs two reports:

Sentence Predictions CSV

Resume Score Summary CSV

🧠 How It Works (Pipeline)
1. Extract text from resume
2. Split text into sentences
3. Remove personal/education sentences → OTHER
4. Convert sentence to TF-IDF vector
5. Add action-verb feature
6. ML classifier predicts category
7. Apply filters:
      - confidence < 0.60 → OTHER
      - missing ML/NLP/CV keywords → OTHER
8. Final clean category assigned
9. Compute ML%, NLP%, Python%, Experience%
10. Generate Resume Score
11. Export CSV reports

🛠 Technologies Used

Python 3.x

Scikit-Learn

Pandas

PDFPlumber

python-docx

Regex

TF-IDF Vectorizer

Logistic Regression (probability-based)

📦 Project Structure
Resume_Score/
│
├── big_resume_training_data.csv
├── resume_pipeline.py
├── resume_inference_superclean.py
├── resume_pipeline_output/
│     ├── resume_pipeline_artifacts.joblib
│     ├── resume_pipeline_test_predictions.csv
│     └── accuracy_comparison.png
│
├── resumes/
│     ├── resume1.pdf
│     ├── resume2.pdf
│     └── ...
│
└── README.md

🧪 Installation & Setup
1. Clone Repository
git clone https://github.com/https://github.com/Vinayaksvijayanagar/HybridResumeScore-AI.git
cd HybridResumeScore-AI

2. Install Dependencies
pip install -r requirements.txt


If requirements.txt doesn't exist, install manually:

pip install scikit-learn pandas pdfplumber python-docx scipy joblib

🎓 Training the Model

Make sure your dataset file is present:

big_resume_training_data.csv


Run:

python resume_pipeline.py


This will:

Train TF-IDF + Logistic Regression

Generate evaluation report

Save artifacts to resume_pipeline_output/resume_pipeline_artifacts.joblib

🧾 Running the Inference (Resume Scoring)

Place resumes inside the resumes/ folder.

Then run:

python resume_inference_superclean.py


This script:

Extracts text

Splits into sentences

Applies hybrid classification

Computes resume scores

Saves results

✔ Output 1: Sentence-level predictions
superclean_sentence_predictions.csv

✔ Output 2: Resume-level scoring
superclean_resume_scores.csv

📊 Example Output (Resume Score)
Resume	ML%	NLP%	Python%	Exp%	Overall
resume_vinayak.pdf	12%	5%	20%	40%	19.25%
praveen_resume.pdf	0%	0%	0%	0%	0%
🧩 Customization

You can customize:

✔ Confidence Threshold
if confidence < 0.60:
    return "OTHER"

✔ ML/NLP/CV Keyword Lists

Modify inside inference file.

✔ Python Skill Keywords

Add/remove libraries depending on job role.

✔ Experience Scoring Formula

Increase or decrease maximum score.

🛠 Future Improvements

Add OCR for scanned PDFs

Add LLM-based semantic scoring

Build Streamlit web UI

Deploy as API

Add database support

🏆 Author

Vinayak S V
AI/ML Engineer | GenAI | NLP | Computer Vision

🤝 Contributions

Pull requests are welcome.
