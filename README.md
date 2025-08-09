
# TruthTrace-LLM: End-to-End Automated Claim Verification & Evidence Retrieval

**TruthTrace-LLM** is an integrated, AI-driven platform for **rigorous, real-time claim verification** and **contextual evidence retrieval**.  
It combines advanced **information retrieval**, **knowledge bases**, **multimedia enrichment**, and **large language model reasoning** to deliver structured, transparent verdicts for any natural language claim.

---

## 🔹 Key Features

- **Intelligent Claim Preprocessing**  
  Extracts the important keywords & context from user queries for targeted search.

- **Multi-Modal Evidence Acquisition**
  - 🌐 **Web Search** – Serper API for real-time, high-authority sources  
  - 📚 **Knowledge Base** – Wikipedia API for factual data and images  
  - 🖼 **Images** – Pixabay API for relevant contextual images  
  - 🎥 **Videos** – YouTube Data API for multimedia references

- **Evidence Aggregation & Filtering**  
  Ensures diversity, authority, and relevance of retrieved sources.

- **Evidence-Constrained LLM Reasoning**  
  Uses **Azure-hosted DeepSeek LLM** to produce unbiased explanations with verdicts:  
  `REAL`, `FAKE`, or `MISLEADING`.

- **Contextual Multimedia Enrichment**  
  Augments verdicts with related images and videos for clarity.

- **Fully Autonomous Pipeline**  
  From claim input to verdict — fully automated, minimal manual intervention required.

---

## 🏗 System Architecture

1. **User Interface Layer** – Streamlit web app for claim input and output display.  
2. **Data Acquisition Layer** – APIs for search, knowledge, and multimedia content.  
3. **Processing & Reasoning Layer** – LLM-powered reasoning based only on retrieved evidence.  
4. **Presentation Layer** – Displays verdict, explanation, sources, images & videos.

---

## 🛠 Tech Stack

- **Frontend:** Streamlit  
- **APIs:** Serper · Wikipedia · Pixabay · YouTube Data API  
- **LLM:** DeepSeek via Azure  
- **Environment Management:** `.env` with `python-dotenv`  
- **Language:** Python 3.x  

---

## 📦 Installation

Clone the repository
git clone https://github.com/Srujan4812/TruthTrace-LLM_.git
cd TruthTrace-LLM_

Install dependencies
pip install -r requirements.txt
pip install python-dotenv

Create a .env file and add:
AZURE_ENDPOINT=...
MODEL_NAME=...
AZURE_API_KEY=...
SERPER_API_KEY=...
PIXABAY_API_KEY=...
YOUTUBE_API_KEY=...

text

---

## ▶ Usage

streamlit run app.py

text

- Open the Streamlit web interface.
- Enter a claim → receive verdict, explanation, related sources, images, and videos.

---

## 🌎 Deployment

- Can be deployed on **Streamlit Cloud**, **Azure App Service**, **Heroku**, etc.  
- Use platform **Secrets Management** to keep API keys secure.  
- Never commit `.env` or API keys to GitHub.

---

## 📊 Model Performance Metrics

| Metric                   | Value       | Description                                        |
|--------------------------|-------------|----------------------------------------------------|
| **Epochs Trained**       | 3           | Number of training epochs completed               |
| **Training Loss**        |             | Model training loss per epoch                      |
| – Epoch 1                | 0.0128      |                                                    |
| – Epoch 2                | 0.0024      |                                                    |
| – Epoch 3                | 0.0002      |                                                    |
| **Validation Loss**      |             | Validation loss per epoch                          |
| – Epoch 1                | 0.000476    |                                                    |
| – Epoch 2                | 0.000191    |                                                    |
| – Epoch 3                | 0.000128    |                                                    |
| **Validation Accuracy**  | 1.0000      | Perfect accuracy on validation set                 |
| **Validation Precision** | 1.0000      | Perfect precision on validation set                |
| **Validation Recall**    | 1.0000      | Perfect recall on validation set                   |
| **Validation F1 Score**  | 1.0000      | Perfect F1 score on validation set                 |
| **Test Set Eval Loss**   | 0.0123      | Loss on unseen test data                           |
| **Test Set Accuracy**    | 0.9983      | Nearly perfect test accuracy                       |
| **Test Set Precision**   | 1.0000      | Perfect precision on test set                      |
| **Test Set Recall**      | 0.9967      | Very high recall on test set                       |
| **Test Set F1 Score**    | 0.9983      | Excellent balance of precision & recall            |
| **Evaluation Runtime**   | 2.0685 sec  | Time taken to evaluate test dataset                |
| **Samples/Second**       | 290.07      | Processing speed for test samples                  |
| **Steps/Second**         | 9.186       | Steps per second during evaluation                 |

> **Summary:** Achieved extremely high precision, recall, and accuracy, indicating outstanding reliability for real-time claim verification.

---

## 💼 Professional Use Cases

- 📰 **Media Verification** – Speed up editorial fact-checking workflows.  
- 🎓 **Academic Research** – Provide evidence summaries for citations & claim validation.  
- 🏢 **Enterprise Knowledge Validation** – Automated evaluation for compliance, risk, and internal comms.

---

## 📄 License

MIT License

---

> **Disclaimer:** This system provides evidence-supported verdicts for informational purposes. Not a substitute for full legal or regulatory verification.

---

**Questions / Contributions:**  
Open an issue or PR via [GitHub Issues](https://github.com/Srujan4812/TruthTrace-LLM_/issues)