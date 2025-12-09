<h1 align="center">
  <img src="https://capsule-render.vercel.app/api?type=venom&height=120&color=gradient&text=HybridResumeScore%20AI&fontAlign=50&fontSize=45&textBg=false&desc=ATS%20Resume%20Classification%20%26%20Scoring%20Engine&descAlignY=75&animation=fadeIn" />
</h1>

---

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=3" width="100%"/>

## 🌟 Overview
**HybridResumeScore AI** is a modern resume intelligence engine that blends  
**Machine Learning + Rule-Based Logic** for clean, ATS-ready resume scoring.

### It performs:
- Sentence-level skill classification  
- AI + rule-based post-processing  
- ATS-style scoring  
- Export of clean CSV reports  

### Skill Categories
ML · NLP · Computer Vision · Data Engineering · Backend · Experience · Other

shell
Copy code

### Hybrid Pipeline
TF-IDF + Logistic Regression
Action Verb Detection
Keyword Validation
Confidence Thresholding
Rule-Based Personal/Education Filtering

yaml
Copy code

---

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00d2ff,100:ff2d95&height=3" width="100%"/>

## ⚡ Core Features

### 📄 Multi-format Resume Parsing  
PDF · DOCX · TXT

markdown
Copy code

### 🧠 Hybrid ML + Rule Engine
- Removes personal/education lines  
- Validates domain-specific keywords  
- Applies confidence cutoff  
- Boosts accuracy using action verbs  

### 📊 Resume Score Metrics
ML %
NLP %
Python %
Experience %
Overall Score

shell
Copy code

### 📁 Outputs Generated
superclean_sentence_predictions.csv
superclean_resume_scores.csv

yaml
Copy code

---

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:ff2d95,100:fccf31&height=3" width="100%"/>

## 🔧 Pipeline Flow
Extract text from resume

Split into sentences

Remove personal/education lines

TF-IDF vectorization

Inject action-verb features

ML model predicts category

Apply rule-based filters

Assign final category

Compute metrics (ML%, NLP%, Python%, Exp%)

Generate overall ATS score

Export CSV results

yaml
Copy code

---

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:fccf31,100:00d2ff&height=3" width="100%"/>

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

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:6a11cb,100:2575fc&height=3" width="100%"/>

## ⚙️ Installation
```bash
git clone https://github.com/YOUR_USERNAME/HybridResumeScore-AI.git
cd HybridResumeScore-AI
pip install -r requirements.txt
Manual install:

bash
Copy code
pip install scikit-learn pandas pdfplumber python-docx scipy joblib
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:ff5f6d,100:ffc371&height=3" width="100%"/>
🧪 Train the Model
bash
Copy code
python resume_pipeline.py
Artifacts saved at:

bash
Copy code
resume_pipeline_output/resume_pipeline_artifacts.joblib
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00c6ff,100:0072ff&height=3" width="100%"/>
🧾 Run Resume Scoring
bash
Copy code
python resume_inference_superclean.py
Generated files:

Copy code
superclean_sentence_predictions.csv
superclean_resume_scores.csv
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:ad7aff,100:00eaff&height=3" width="100%"/>
📊 Example Output
markdown
Copy code
Resume                ML%   NLP%   Python%   Exp%   Overall
-----------------------------------------------------------
resume_vinayak.pdf     12%    5%      20%     40%    19.25%
praveen_resume.pdf      0%    0%       0%      0%     0%
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:11998e,100:38ef7d&height=3" width="100%"/>
🛠 Customization
Confidence Threshold
python
Copy code
if confidence < 0.60:
    return "OTHER"
Keyword Lists
Adjust ML/NLP/CV/Python keyword sets inside the inference script.

Scoring Formula
You may modify weight distribution:

shell
Copy code
ML% · NLP% · Python% · Experience%
<h2 align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=footer" /> </h2> <h3 align="center"> 🏆 Created by <b>Vinayak S V</b><br> <i>AI/ML Engineer • GenAI • NLP • Computer Vision</i> </h3> <p align="center"> ⭐ <b>If you like this project, please star the repository!</b> ⭐ </p> ```
