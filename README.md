# AI-based-Resume-Screening-System
This project is a Flask-based web application for automated resume screening that supports PDF and TXT resume files. The system provides functionalities including resume categorization, job recommendation, and detailed resume parsing (information extraction).

---

## Features

- **Resume Upload:** Supports uploading resumes in PDF and TXT formats.
- **Resume Categorization:** Classifies resumes into relevant professional categories using a pre-trained Random Forest classifier.
- **Job Recommendation:** Recommends suitable job roles based on the resume content.
- **Information Extraction:** Extracts key information from resumes including:
  - Candidate’s Name
  - Contact Phone Number
  - Email Address
  - Skills (from a comprehensive predefined list)
  - Education details (matched through keyword search)
- **Text Processing:** Uses pdfminer and PyPDF2 to extract text from PDFs, and UTF-8 decoding for TXT files.
- **Clean and Preprocess:** Cleans extracted text for noise such as URLs, special characters, and unnecessary whitespace.
- **Machine Learning Models:** Uses TF-IDF vectorizer and Random Forest models for classification and recommendation.
- **Responsive Web UI:** Provides an easy-to-use front end with Flask and Jinja2 templates.

----


## Dependencies

- Flask
- PyPDF2
- pdfminer.six
- scikit-learn
- pandas
- numpy
- regex (re)

-----

## Notes

- The system distinguishes only PDF and TXT files; other formats are rejected.
- Regex-based extraction may not catch all variants of contact details; further NLP improvements are possible.
- Error handling around file reading/parsing can be extended.
- Models and vectorizers are pre-trained; custom training notebooks are included.
- Ensure resume files have readable text (non-image PDFs are preferred).

Thankyou for exploring AI-based-Resume-Screening-System!!!
