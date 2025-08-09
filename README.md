# 🧠 TruthTrace-LLM: End-to-End Automated Claim Verification & Evidence Retrieval

**TruthTrace-LLM** is an integrated, AI-powered platform for rigorous, real-time claim verification and contextual evidence retrieval.  
It combines intelligent information retrieval, structured knowledge bases, multimedia enrichment, and large language model reasoning to deliver structured, transparent verdicts for any natural language claim.

---

## 🚀 Live Demo

🔗 [**Try it now → TruthTrace-LLM Web App**](https://truthtrace-llm-aa8ehtudvwvspzlqbqx2kg.streamlit.app/)

---

## 🔹 Key Features

### ✨ Intelligent Claim Preprocessing  
Extracts important keywords and context from user queries for targeted search and analysis.

### 🌐 Multi-Modal Evidence Acquisition  
- **Serper API** – Real-time, high-authority web search  
- **Wikipedia API** – Structured factual data  
- **Pixabay API** – Relevant contextual imagery  
- **YouTube Data API** – Multimedia references (videos)

### 📦 Evidence Aggregation & Filtering  
Ensures diversity, credibility, and contextual relevance of all retrieved sources.

### 🤖 Evidence-Constrained LLM Reasoning  
Uses **DeepSeek LLM** (via Azure) to evaluate and verify claims using only the retrieved evidence.

Verdicts include:
- ✅ `REAL`
- ❌ `FAKE`
- ⚠️ `MISLEADING`

### 🖼 Contextual Multimedia Enrichment  
Adds images and videos to verdicts for improved clarity and transparency.

### 🔁 Fully Autonomous Pipeline  
From claim input to final verdict — fully automated with minimal manual input.

---

## 🏗️ System Architecture

- **User Interface Layer** – Streamlit-based web app  
- **Data Acquisition Layer** – Real-time APIs for search, knowledge, and multimedia  
- **Processing Layer** – LLM-powered reasoning based on contextual evidence  
- **Presentation Layer** – Verdicts, explanations, sources, images, and videos

[User] → [Streamlit UI] → [Evidence Collection] → [LLM Analysis] → [Verdict + Media]

yaml
Copy
Edit

---

## 🛠 Tech Stack

| Component       | Technology                                 |
|----------------|---------------------------------------------|
| Frontend       | Streamlit                                   |
| Language       | Python 3.x                                  |
| APIs           | Serper · Wikipedia · Pixabay · YouTube Data API |
| LLM            | DeepSeek (Azure-hosted)                     |
| Env Management | python-dotenv + `.env`                      |

---

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/Srujan4812/TruthTrace-LLM_.git
cd TruthTrace-LLM_

# Install dependencies
pip install -r requirements.txt
pip install python-dotenv
🔐 Setup .env File
Create a .env file in the root directory and add your API keys:

env
Copy
Edit
AZURE_ENDPOINT=...
MODEL_NAME=...
AZURE_API_KEY=...
SERPER_API_KEY=...
PIXABAY_API_KEY=...
YOUTUBE_API_KEY=...
⚠️ Important: Never commit .env or API keys to GitHub.

▶️ Usage (Local)
bash
Copy
Edit
streamlit run app.py
Open the Streamlit interface in your browser.
Enter a claim → receive a verdict with explanation, source links, images, and videos.

🌍 Deployment
✅ Live App: Streamlit Cloud
Can also be deployed to:

Azure App Service

Heroku

Any modern cloud platform

Use built-in Secrets Management to securely store API keys.

📸 Screenshots
🔍 Claim Entry Interface

✅ Verdict with Explanation & Multimedia

🎥 Demo Video
Watch how TruthTrace-LLM works in action:
👉 Click to Watch Demo Video

🎬 A 1-minute walkthrough showing claim input, evidence collection, verdict generation, and multimedia enrichment.

📊 Model Performance Metrics
✅ Training & Validation
Metric	Epoch 1	Epoch 2	Epoch 3
Training Loss	0.0128	0.0024	0.0002
Validation Loss	0.000476	0.000191	0.000128
Accuracy	1.0000	1.0000	1.0000
Precision	1.0000	1.0000	1.0000
Recall	1.0000	1.0000	1.0000
F1 Score	1.0000	1.0000	1.0000

🧪 Test Set Evaluation
Metric	Value
Test Set Loss	0.0123
Test Set Accuracy	0.9983
Test Set Precision	1.0000
Test Set Recall	0.9967
Test Set F1 Score	0.9983
Eval Runtime	2.0685 s
Samples/Second	290.07
Steps/Second	9.186

✅ Summary: Near-perfect performance on both validation and test sets.
Ideal for real-time deployment in production environments.

💼 Professional Use Cases
📰 Media Fact-Checking – Accelerate editorial verification workflows

🎓 Academic Research – Back up claims and citations with evidence

🏢 Enterprise Validation – Automate compliance and internal knowledge validation

📄 License
Licensed under the MIT License.

⚠️ Disclaimer
This tool provides automated, evidence-supported verdicts to assist with decision-making.
It is not a replacement for legal, journalistic, or regulatory investigations.

🤝 Questions & Contributions
💬 Open an issue

📬 Submit a pull request

🛠 Help shape the future of AI-powered claim verification!