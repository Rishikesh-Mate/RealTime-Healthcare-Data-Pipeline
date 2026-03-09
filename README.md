# Real-Time Patient Vitals Monitoring System

## 🏥 Project Overview
This project simulates a high-velocity healthcare environment where wearable devices send continuous patient vitals (Heart Rate, SpO2, Temperature) to the cloud. The goal is to build a robust **Streaming Medallion Pipeline** that cleans data, identifies health risks in real-time using Machine Learning, and provides live clinical insights.

## 🛠️ Tech Stack
* **Language:** Python 3.x (Data Simulation & Ingestion)
* **Cloud Infrastructure:** Azure Event Hubs
* **Data Processing:** Databricks (PySpark Structured Streaming)
* **Storage:** Delta Lake (Bronze, Silver, Gold Layers)
* **Orchestration:** MLflow (for real-time inference)

## 📈 Pipeline Architecture
1. **Producer:** Python script generating randomized, JSON-formatted patient telemetry.
2. **Ingestion:** Azure Event Hubs acting as the real-time message broker.
3. **Refinery (Medallion):** - **Bronze:** Raw JSON ingestion.
   - **Silver:** Schema enforcement, deduplication, and data cleaning.
   - **Gold:** Real-time window aggregations and "Critical Alert" flagging.
4. **Analytics:** ML-based risk scoring for patient deterioration.

## 🚀 Current Status
- [x] **Phase 1:** Developed Python data generator with JSON serialization.
- [ ] **Phase 2:** Connect producer to Azure Event Hubs.
- [ ] **Phase 3:** Implement Spark Structured Streaming in Databricks.
- [ ] **Phase 4:** Integrate MLflow for real-time risk prediction.

---
*Note: This project is being developed as part of my preparation for the MS in Data Science program at the University of Minnesota (UMN).*
