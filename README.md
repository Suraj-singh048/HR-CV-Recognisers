# HR CV Recognizer App

This **HR CV Recognizer** is a Streamlit-based web application that classifies incoming resumes into various **job categories** (e.g., Data Science, Software Development, HR, etc.). It can handle resumes in PDF, DOCX, or TXT format.

---

## Features

- **Text Extraction**  
  Automatically extracts and cleans text from uploaded resumes:
  - PDF (via `PyPDF2`)
  - DOCX (via `python-docx`)
  - TXT (with various encodings)

- **Model-Based Classification**  
  Uses:
  - A pre-trained **SVC** (Support Vector Classifier) loaded from `clf.pkl`
  - A **TF-IDF** vectorizer loaded from `tfidf.pkl`
  - An **Encoder** (Label Encoder) loaded from `encoder.pkl` to map numeric labels back to job category names.

- **User-Friendly Interface**  
  Built with [Streamlit](https://streamlit.io/), allowing easy file uploads and quick predictions right in your browser.

---
