<h1 align="center">🚀 HybridResumeScore AI</h1>
<p align="center">
  <b>ATS-Grade Resume Intelligence Engine</b><br>
  <i>Hybrid ML + Rule-Based System for Accurate Skill Classification</i>
</p>

---

## 🔥 Overview
**HybridResumeScore AI** analyzes resumes with high precision using a clean hybrid pipeline.

### It performs:
- Sentence-level skill classification  
- AI + rule-based filtering  
- ATS-style scoring  
- Export of structured CSV reports  

### Skill Categories:
ML · NLP · Computer Vision · Data Engineering · Backend · Experience · Other

shell
Copy code

### Hybrid Pipeline:
TF-IDF + Logistic Regression
Action Verb Detection
Keyword Validation
Confidence Thresholding
Rule-Based Personal/Education Filtering

yaml
Copy code

---

## ⭐ Core Features

### 📄 Multi-format Resume Parsing
Supports: PDF · DOCX · TXT

markdown
Copy code

### 🧠 Hybrid ML + Rule Engine
- Removes personal/education lines  
- Validation with domain keywords  
- Confidence cutoff (<0.60)  
- Action verbs improve classification  

### 📊 Resume Scoring Metrics
ML %
NLP %
Python %
Experience %
Overall Score

shell
Copy code

### 📁 Outputs
superclean_sentence_predictions.csv
superclean_resume_scores.csv

yaml
Copy code

---

## 🔧 Pipeline Flow
Extract text from resume

Split into sentences

Remove personal/education lines

TF-IDF vectorization

Add action-verb features

ML model predicts category

Apply rule-based corrections

Assign final label

Compute metrics

Generate final score

Save CSV reports

yaml
Copy code

---

## 📂 Project Structure
Resume_Score/
│
├── big_resume_training_data.csv
├── resume_pipeline.py
├── resume_inference_superclean.py
│
├── resume_pipeline_output/
│ ├── resume_pipeline_artifacts.joblib
│ ├── resume_pipeline_test_predictions.csv
│ └── accuracy_comparison.png
│
├── resumes/
│ ├── resume1.pdf
│ └── resume2.pdf
│
└── README.md

yaml
Copy code

---

## ⚙️ Installation
```bash
git clone https://github.com/YOUR_USERNAME/HybridResumeScore-AI.git
cd HybridResumeScore-AI
pip install -r requirements.txt
Manual install:

bash
Copy code
pip install scikit-learn pandas pdfplumber python-docx scipy joblib
🧪 Train the Model
bash
Copy code
python resume_pipeline.py
Artifacts saved at:

bash
Copy code
resume_pipeline_output/resume_pipeline_artifacts.joblib
🧾 Run Resume Scoring
bash
Copy code
python resume_inference_superclean.py
Outputs:

Copy code
superclean_sentence_predictions.csv
superclean_resume_scores.csv
📊 Example Output
markdown
Copy code
Resume                ML%   NLP%   Python%   Exp%   Overall
-----------------------------------------------------------
resume_vinayak.pdf     12%    5%      20%     40%    19.25%
praveen_resume.pdf      0%    0%       0%      0%     0%
🛠 Customization
Confidence Threshold
python
Copy code
if confidence < 0.60:
    return "OTHER"
Keyword Lists
You can edit ML/NLP/CV/Python keyword lists inside the inference script.

Scoring Formula
Adjust weight distribution:

shell
Copy code
ML% · NLP% · Python% · Experience%
<h3 align="center">🔹 Created by <b>Vinayak S V</b></h3> <p align="center"> AI/ML Engineer • GenAI • NLP • Computer Vision <br> ⭐ If this project helps you, please star the repository! </p> ```
