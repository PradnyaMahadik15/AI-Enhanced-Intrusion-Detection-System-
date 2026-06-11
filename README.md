# AI-Enhanced-Intrusion-Detection-System-
AI-Enhanced Intrusion Detection System is a machine learning-based cybersecurity project designed to detect and classify network intrusions in real time. It analyzes network traffic, identifies suspicious activities, and enhances threat detection accuracy using AI techniques, helping improve network security and attack prevention.
# AI-Enhanced Intrusion Detection System (AI-IDS) 🛡️

An enterprise-grade, real-time Network Security Monitoring and Security Operations Center (SOC) platform. This system utilizes advanced Machine Learning techniques paired with an interactive, responsive web interface to ingest network packet profiles, predict threat vectors, and visualize live intrusion metrics.

Built on the **UNSW-NB15 dataset**, the system identifies and classifies multiple malicious threat classifications—including DoS, Reconnaissance, Exploits, Fuzzers, and Generic attacks—with high operational accuracy.

---

## 📁 Project Structure

```text
ai_ids/
├── backend/
│   └── main.py          # Flask REST API engine (Handles model inference & simulation) [Runs on Port 5000]
├── dashboard/
│   ├── app.py           # Dashboard App Router (Serves HTML pages) [Runs on Port 5001]
│   └── templates/
│       └── index.html   # Main SOC Frontend UI (Compiled Chart.js workspace)
├── ml/
│   ├── train.py         # Sklearn processing pipeline and Random Forest Engine
│   └── model.pkl        # Serialized pipeline containing estimators, encoders, and metrics
├── data/
│   └── UNSW_NB15_training-set.csv  # Network dataset corpus
└── requirements.txt     # Global Application Dependencies
