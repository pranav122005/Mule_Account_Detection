<div align="center">
  <h1>🚀 MIDAS</h1>
  <h3>Mule Intelligence & Detection Across Systems</h3>
  <p><em>An AI/ML federated graph system that detects multi-bank mule accounts and auto-freezes fraudulent transactions within 60 seconds.</em></p>
</div>

---

### 🎯 Overview
MIDAS was developed for the **PSBs Hackathon Series 2026 (CyberShield Track)** to intercept the critical infrastructure of financial cybercrime.

### ⚠️ The Vulnerability Gap
* ⏱️ **The Golden Hour Exploit:** Fraudsters use legacy banks with 24-48 hour batch delays to outpace the 60-minute fraud recovery window.
* 🙈 **Siloed Bank Data:** Coordinated multi-bank mule chains are completely invisible to individual banks.
* 🏢 **Current Account Blindspots:** Shell companies use real KYC documents to launder money as legitimate business receipts.

### 🧠 Core Architecture
* 📥 **Smart Ingestion:** Kafka and Flink normalize 19 distinct financial and regulatory data streams.
* 🕸️ **Graph Engine:** Neo4j tracks cross-bank transaction networks dynamically.
* 🤖 **ML Ensemble:** Five powerful models (XGBoost, Isolation Forest, GraphSAGE, LSTM, BERT) generate a unified 0-100 risk score.

### ⚡ Key Innovations
1. 🔒 **Federated Cross-Bank Graph:** Shares only hashed identifiers and risk scores, detecting multi-bank fraud rings while maintaining 100% RBI privacy compliance.
2. 🗂️ **Business Legitimacy Index (BLI):** Cross-references GSTN, MCA, and banking data in real-time to flag shell companies right at onboarding.
3. 🏎️ **Golden Hour Accelerator:** A lightweight edge agent that enables legacy banks to execute sub-60-second freezes without requiring heavy core banking upgrades.

### 📊 Model Performance
* 📁 **Dataset:** Trained on a real Bank of India dataset containing 9,082 accounts.
* 🎯 **Results:** The primary XGBoost classifier achieved a **1.000 Precision-Recall AUC**—successfully identifying all confirmed mules with zero false positives.

---
