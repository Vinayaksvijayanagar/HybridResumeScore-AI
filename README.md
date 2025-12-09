<h1 align="center" style="color:#00f2ff;"> HYBRIDRESUMESCORE AI </h1>
<p align="center">
  <b><span style="color:#ff00ff;">Neon ATS Resume Intelligence Engine</span></b><br>
  <i><span style="color:#39ff14;">Hybrid ML + Rule-Based Filtering System</span></i>
</p>

---

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=00f2ff&height=120&section=header"/>

## ✨ <span style="color:#00f2ff;">Overview</span>
**HybridResumeScore AI** analyzes resumes with neon precision:

- Sentence-level classification  
- AI + rule-based filtering  
- ATS-style scoring  
- Clean CSV outputs  

Skill Categories:
ML ⚡ NLP ⚡ CV ⚡ DE ⚡ Backend ⚡ Experience ⚡ Other

yaml
Copy code

Hybrid Pipeline:
TF-IDF + Logistic Regression
Action Verb Detection
Keyword Validation
Confidence Threshold
Rule-Based Personal/Education Filtering

yaml
Copy code

---

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=ff00ff&height=4"/>

## 🌌 <span style="color:#ff00ff;">Core Features</span>

### 🔮 Multi-Format Parsing
PDF • DOCX • TXT

markdown
Copy code

### 🧠 Hybrid ML + Rule Engine
- Removes personal/education lines  
- Keyword validation  
- Confidence cutoff (0.60)  
- Action verbs boost accuracy  

### 📊 Neon Resume Score
ML %
NLP %
Python %
Experience %
Overall Score

shell
Copy code

### 📁 Outputs
superclean_sentence_predictions.csv/n
superclean_resume_scores.csv

yaml
Copy code

---

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=39ff14&height=4"/>

## 💠 <span style="color:#39ff14;">Pipeline Flow</span>
Extract text

Split into sentences

Remove personal/education lines

TF-IDF vectorization

Add action-verb feature

Predict using ML model

Apply neon filters

Assign final label

Compute stats

Generate score

Save CSVs

yaml
Copy code

---

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=00f2ff&height=4"/>

## 🗂️ <span style="color:#00f2ff;">Project Structure</span>
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

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=ff00ff&height=4"/>

## ⚙️ <span style="color:#ff00ff;">Installation</span>
```bash
git clone https://github.com/YOUR_USERNAME/HybridResumeScore-AI.git
cd HybridResumeScore-AI
pip install -r requirements.txt
Manual:

bash
Copy code
pip install scikit-learn pandas pdfplumber python-docx scipy joblib
<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=39ff14&height=4"/>
🧪 <span style="color:#39ff14;">Train the Model</span>
bash
Copy code
python resume_pipeline.py
Artifacts saved at:

bash
Copy code
resume_pipeline_output/resume_pipeline_artifacts.joblib
<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=00f2ff&height=4"/>
🧾 <span style="color:#00f2ff;">Run Resume Scoring</span>
bash
Copy code
python resume_inference_superclean.py
Outputs:

Copy code
superclean_sentence_predictions.csv
superclean_resume_scores.csv
<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=ff00ff&height=4"/>
🌈 <span style="color:#ff00ff;">Example Output</span>
markdown
Copy code
Resume                ML%   NLP%   Python%   Exp%   Overall
-----------------------------------------------------------
resume_vinayak.pdf     12%    5%      20%     40%    19.25%
praveen_resume.pdf      0%    0%       0%      0%     0%
<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=39ff14&height=4"/>
🛠️ <span style="color:#39ff14;">Customization</span>
Confidence Rule
python
Copy code
if confidence < 0.60:
    return "OTHER"
Keyword Lists
Modify ML/NLP/CV/Python keywords.

Scoring Formula
Adjust:

shell
Copy code
ML% • NLP% • Python% • Experience%
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=ff00ff&height=120&section=footer"/> <h3 align="center"> <span style="color:#ff00ff;">🏆 Created by Vinayak S V</span><br> <span style="color:#39ff14;">AI/ML Engineer • GenAI • NLP • CV</span> </h3> <p align="center"> <b><span style="color:#00f2ff;">⭐ Star this repository if you love neon!</span></b> </p> ```
