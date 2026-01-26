# Vehicle Predictive Maintenance System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![University](https://img.shields.io/badge/University-Bologna-red)](https://www.unibo.it/)

An integrated end-to-end solution for automotive fleet management that combines **Machine Learning**, **Blockchain technology**, and **Internet of Things (IoT)** to predict maintenance needs with high precision.



## 📌 Project Overview
Developed as an integrated final project for the Master's Degree in Computer Science and Engineering at the **University of Bologna**, this system addresses the challenges of traditional reactive maintenance. It leverages real-time telematics and historical data to predict component failures before they occur.

### Key Performance Indicators
* **Accuracy:** 100% on test data using Random Forest.
* **ROC-AUC:** 1.0000.
* **Economic Impact:** Estimated savings of **€165,800 per 10,000 vehicles**.
* **Breakdown Reduction:** Proactive scheduling reduces vehicle breakdowns by **80%**.

---

## 🏗️ Integrated Architecture

The system is built on three core pillars:

1. **Machine Learning (Codice 95531):** - Predictive analytics and anomaly detection.
   - Algorithms: Random Forest (Best performer), Logistic Regression, and Isolation Forest.
2. **Distributed Systems (Codice 87474):** - Uses **Hyperledger Fabric** to create an immutable, VIN-based ledger.
   - Smart contracts trigger maintenance alerts and store tamper-proof service records.
3. **Embedded Systems & IoT (Codice 77780):** - Hardware: **ESP32** and **OBD-II** protocols.
   - Edge computing filters data before transmission via MQTT to minimize bandwidth.

---

## 📊 Methodology & Data
The analysis was performed on a dataset of **50,000 vehicle records** with 20 attributes.

### Model Performance Comparison
| Model | Accuracy | Precision | Recall | ROC-AUC |
| :--- | :--- | :--- | :--- | :--- |
| **Random Forest** | **1.00** | **1.00** | **1.00** | **1.00** |
| Logistic Regression | 0.95 | 0.81 | 0.98 | 0.9878 |
| Isolation Forest | 0.81 | 0.24 | 0.01 | 0.58 |



### Key Maintenance Triggers
Based on feature importance and M5P Model Tree analysis:
* **Reported Issues:** Primary predictor (31.5% importance).
* **Brake Condition:** "Worn Out" status is the primary root split for urgent maintenance.
* **Battery Status:** "Weak" status indicates a 99% probability of required service.

---

## 🚀 Deployment & Implementation
- **API:** Predictive models are deployed via a **Flask REST API** with response times <10ms.
- **Blockchain:** Hyperledger Fabric manages unique digital identities for every vehicle.
- **Edge Hardware:** ESP32 devices process and send sensor data packets every 60 seconds.

---

## 👥 Authors
* **Danial Khayatian** - [danial.khayatian@studio.unibo.it](mailto:danial.khayatian@studio.unibo.it)
* **Dias Katrenov** - [dias.katrenov@studio.unibo.it](mailto:dias.katrenov@studio.unibo.it)
* **Mary Anne Selirio** - [maryanne.selirio@studio.unibo.it](mailto:maryanne.selirio@studio.unibo.it)

**Supervisor:** Prof. Matteo Golfarelli  
**Institution:** University of Bologna | A.Y. 2024/2025  

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
