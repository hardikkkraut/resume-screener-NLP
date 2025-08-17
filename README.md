A machine learning project that automatically screens resumes by extracting text, analyzing skills, and predicting candidate-job match scores. Includes NLP preprocessing, feature extraction (TF‑IDF, word embeddings), classification/regression modeling, evaluation metrics, and an optional Streamlit app for interactive resume uploads. Designed for recruiters, students, and portfolio demonstration.

🚀 Features

Resume text extraction (PDF/DOCX parsing)

NLP preprocessing (cleaning, tokenization, stopword removal)

Feature engineering with TF‑IDF and word embeddings

Machine learning model for predicting job-fit scores or categories

Model evaluation with precision, recall, F1-score

Streamlit app for uploading resumes and viewing screening results

📂 Project Structure

resume-screener/
│
├── data/
│   └── resumes.csv            # Sample dataset of resumes & labels
├── src/
│   ├── preprocess.py          # Text cleaning and NLP utilities
│   ├── train.py               # Training ML model
│   ├── infer.py               # Model inference on new resumes
│   └── utils.py               # Helper functions
├── app.py                     # Streamlit app for resume upload
├── requirements.txt           # Dependencies
├── model.joblib               # Saved trained model
└── README.md                  # Project documentation

🛠️ Installation

git clone https://github.com/<your-username>/resume-screener.git
cd resume-screener
pip install -r requirements.txt

📊 Usage

1. Train Model

python src/train.py

2. Run Resume Screener App

streamlit run app.py

Upload resumes in PDF/DOCX format and get predicted screening results.

📈 Example Output

Candidate Skill Extraction: Python, SQL, Machine Learning

Predicted Job Role Fit: Data Analyst

Confidence Score: 87%

✅ Tech Stack

Python (pandas, scikit-learn, numpy)

NLP (NLTK, spaCy, TF‑IDF, embeddings)

Machine Learning (Logistic Regression, RandomForest, SVM)

Deployment (Streamlit)

📌 Future Enhancements

Support for parsing images in resumes (OCR)

Advanced embeddings with BERT/transformers

Dashboard for recruiters to manage multiple resumes

📢 Built as a portfolio project to demonstrate end-to-end ML pipeline with NLP and deployment.

