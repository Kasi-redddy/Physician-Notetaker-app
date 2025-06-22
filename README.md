# 🩺 Physician Notetaker: Medical NLP & Sentiment Analysis

This project is a powerful AI-driven web application that extracts structured medical insights from physician-patient conversation transcripts. It uses NLP techniques to generate SOAP notes, extract symptoms and keywords, and detect patient sentiment and intent.

---

## 🔍 Features

- ✅ Named Entity Recognition (NER) for symptoms, diagnosis, treatment, prognosis
- ✅ Medical keyword extraction
- ✅ Sentiment & intent detection from patient dialogues
- ✅ Structured report generation (JSON format)
- ✅ Auto-generated SOAP Notes
- ✅ Live Streamlit interface

---

## 🚀 Live Demo

Access the app here:  
🔗 **[Live Application URL](https://babc-34-125-72-155.ngrok-free.app)**

---

## 🧠 Technologies Used

- **Python 3**
- **Streamlit** – For frontend UI
- **spaCy** – Named Entity Recognition
- **Hugging Face Transformers** – Sentiment analysis (`distilbert-base-uncased-finetuned-sst-2-english`)
- **Regular Expressions** – Custom medical rule-based NER

---

## 📦 Installation

### ✅ Clone the repo

```bash
git clone https://github.com/Kasi-redddy/Physician-Notetaker-app.git
cd Physician-Notetaker-app
```

### ✅ Install dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` is not present, install manually:
```bash
pip install streamlit spacy transformers
python -m spacy download en_core_web_sm
```

---

## ▶️ Run the App Locally

```bash
streamlit run physician_notetaker_app.py
```

The app will be available at:  
📍 http://localhost:8501

---

## 🌐 Hosting (Ngrok Method)

If you are using Google Colab or want to make your app live:

1. Install ngrok and pyngrok
```bash
pip install pyngrok
```

2. Add your ngrok authtoken
```bash
ngrok config add-authtoken YOUR_AUTHTOKEN
```

3. In Python (or Colab), run:
```python
from pyngrok import ngrok
public_url = ngrok.connect(8501)
print("App URL:", public_url)
!streamlit run physician_notetaker_app.py &
```


---

## 🧭 Methodology

- **Entity Extraction**: Rule-based regex + spaCy parsing
- **Sentiment Analysis**: Hugging Face transformer pipeline
- **SOAP Generation**: Rule-based structuring from extracted context
- **UI**: Streamlit with sectioned results for better interpretability

---

## 🙋‍♂️ Author

**Kasi Visweswar Reddy**  
📧 reddykasivisweswar@gmail.com  
🔗 [GitHub](https://github.com/Kasi-redddy)

---

## 🏁 Conclusion

This project demonstrates a practical application of NLP in healthcare documentation. It improves efficiency for physicians by auto-generating structured clinical notes, enabling quick review and easy integration into EMR systems.

---


