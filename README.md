# CBC-Report-Interpreter
# CBC Report Interpreter

A Streamlit-based application that extracts CBC (Complete Blood Count) values from medical reports using OCR and predicts the urgency level using a machine learning model.

> This project is developed for educational purposes and is not intended to replace professional medical advice.

---

## Features

- Upload CBC reports (PDF, JPG, PNG)
- Extract CBC values using Tesseract OCR
- Edit extracted values if required
- Predict urgency using a Random Forest model

---

## Tech Stack

- Python
- Streamlit
- Scikit-learn
- OpenCV


---

## Project Structure

```
project/
│
├── app.py
├── extractor.py
├── file_predict.py
├── explain_cbc_model.py
├── cbc_model.pkl
├── label_encoder.pkl
├── requirements.txt
```

---

## Installation

Clone the repository:

```bash

```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it:

```bash
# Windows
.venv\Scripts\activate

# Linux/macOS
source .venv/bin/activate
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Install Tesseract OCR and update its path in `extractor.py` if required.

---

## Run



---

## Model

- Random Forest Classifier
- Predicts four urgency levels:
  - Normal
  - Mild
  - Urgent
  - Emergency

Features used:

- HGB
- WBC
- RBC
- PLT


---

## Limitations

- OCR accuracy depends on report quality.
- The model is trained on a limited dataset.
- Results should be considered supportive and not a medical diagnosis.

---

## Future Improvements

- Improve OCR accuracy
- Train on a larger dataset
- Add confidence scores
