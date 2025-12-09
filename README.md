<h1 align="center">
     <img src="https://capsule-render.vercel.app/api?type=waving&color=0:00f5d4,33:00bbf9,66:9b5de5,100:f15bb5&height=170&section=footer&text=HybridResumeScore%20AI&fontColor=ffffff&fontSize=34&fontAlignY=70&animation=fadeIn"/>



</h1>

## Overview
**HybridResumeScore AI** analyzes resumes using a hybrid ML + rule-engine pipeline.

### It performs:
- Sentence-level skill classification  
- AI + rule-based filtering  
- ATS-style scoring  
- Export of clean CSV reports  

### Skill Categories
ML · NLP · Computer Vision · Data Engineering · Backend · Experience · Other

 

### Hybrid Pipeline
TF-IDF + Logistic Regression<br>
Action Verb Detection<br>
Keyword Validation<br>
Confidence Thresholding<br>
Rule-Based Personal/Education Filtering

 
---

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00d2ff,100:ff2d95&height=3" width="100%"/>

## Core Features

### Multi-format Resume Parsing
PDF · DOCX · TXT

 
### Hybrid ML + Rule Engine
- Removes personal and education lines  
- Validates domain-specific keywords  
- Applies confidence threshold  
- Action verbs improve classification  

###  Resume Score Metrics
ML %<br>
NLP %<br>
Python %<br>
Experience %<br>
Overall Score<br>

 
###  Outputs
superclean_sentence_predictions.csv<br>
superclean_resume_scores.csv

 

---

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:ff2d95,100:fccf31&height=3" width="100%"/>

##  Pipeline Flow
Extract text

Split into sentences

Remove personal/education lines

TF-IDF vectorization

Add action-verb features

ML model predicts category

Apply rule-based filters

Assign final category

Compute metrics

Generate overall score

Export CSV results

 

---

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:fccf31,100:00d2ff&height=3" width="100%"/>

##  Project Structure

 Resume_Score/<br>
│<br>
├── big_resume_training_data.csv<br>
├── resume_pipeline.py<br>
├── resume_inference_superclean.py<br>
│<br>
├── resume_pipeline_output/<br>
│   ├── resume_pipeline_artifacts.joblib<br>
│   ├── resume_pipeline_test_predictions.csv<br>
│   └── accuracy_comparison.png<br>
│<br>
├── resumes/<br>
│   ├── resume1.pdf<br>
│   └── resume2.pdf<br>
│<br>
└── README.md<br>

 



<img src="https://capsule-render.vercel.app/api?type=rect&color=0:6a11cb,100:2575fc&height=3" width="100%"/>
sInstallation
 
git clone https://github.com/Vinayaksvijayanagar/HybridResumeScore-AI.git<br>
cd HybridResumeScore-AI<br>
pip install -r requirements.txt<br>

Manual install:<br>
pip install scikit-learn pandas pdfplumber python-docx scipy joblib
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:ff5f6d,100:ffc371&height=3" width="100%"/>
 Train the Model<br>
python resume_pipeline.py<br>

Artifacts saved at:<br>
resume_pipeline_output/resume_pipeline_artifacts.joblib
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00c6ff,100:0072ff&height=3" width="100%"/>
Run Resume Scoring<br>
python resume_inference_superclean.py<br>

Generated files:<br>
superclean_sentence_predictions.csv<br>
superclean_resume_scores.csv
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:ad7aff,100:00eaff&height=3" width="100%"/>
 Example Output
<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=12HGKmTIl8dfDs6IpCO1Smv-y5iZm6yrq" width="450">
</p>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:11998e,100:38ef7d&height=3" width="100%"/>

<h2 align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=footer" /> </h2> <h3 align="center">   <b>Vinayak S V</b><br> <i>AI/ML · GenAI · NLP · Computer Vision</i> </h3> <p align="center"> <b>Nyukt.AI hiring round project</b> </p> 
