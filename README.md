# Federated Learning-Based Intrusion Detection System (IDS)

##  Project Overview
This project presents a **Federated Learning-Based Intrusion Detection System (IDS)** designed for distributed network environments. The system enables multiple network clients to collaboratively train machine learning models without sharing raw data, thereby ensuring **data privacy and security**.

The model is trained and evaluated using the **CIC-IDS 2017 dataset**, which contains realistic network traffic data including both benign and malicious activities.

---

## Objectives
- Develop a **privacy-preserving intrusion detection system**
- Simulate **distributed network environments** using federated learning
- Detect both **known and unknown cyber-attacks**
- Compare performance of multiple machine learning models
- Evaluate system effectiveness using standard classification metrics

---

## Dataset
- **Dataset Used**: CIC-IDS 2017  
- **Kaggle Link**: https://www.kaggle.com/datasets/chethuhn/network-intrusion-dataset
- Includes:
  - Benign (normal) traffic  
  - Attack types:
    - DoS / DDoS  
    - Brute Force  
    - Web Attacks  
    - Botnet  
    - Port Scanning  
    - Infiltration  

### 🔹 Preprocessing Steps
- Removed missing and infinite values  
- Converted all features to numeric format  
- Created binary classification:
  - `0 → Normal Traffic`
  - `1 → Attack Traffic`
- Feature scaling using `StandardScaler`

---

##  System Architecture

### 🔹 Federated Learning Workflow
1. Data is divided into multiple **network clients**
2. Each client trains a **local model**
3. Only **model parameters** are shared
4. Server performs **Federated Averaging**
5. Global model is created and redistributed
6. Process repeats for multiple rounds

### 🔹 Federated Clients
- Network A – Normal Traffic  
- Network B – Brute Force  
- Network C – DoS / Heartbleed  
- Network D – Web Attacks / Infiltration  
- Network E – Botnet / DDoS / PortScan  

---

## Machine Learning Models Used

### 1. Random Forest
- Ensemble learning method  
- Effective for classification tasks  

### 2. XGBoost
- Gradient boosting algorithm  
- High accuracy and efficiency  

### 3. MLP Neural Network
- Deep learning model  
- Captures complex patterns  

### 4. Isolation Forest
- Unsupervised anomaly detection  
- Detects zero-day attacks  

---

## Key Features
- Federated Learning implementation  
- Privacy-preserving training  
- Multi-model comparison  
- Adaptive threshold detection  
- Imbalanced data handling  
- Real-time alert simulation  
- Feature importance analysis  

---

## Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- False Positive Rate (FPR)  
- ROC-AUC Curve  

---

## Results
- High accuracy and F1-scores achieved  
- Random Forest and XGBoost performed best  
- Isolation Forest detected unknown attacks  
- Federated learning preserved privacy without compromising performance  

---

## Intrusion Detection Simulation
The system simulates real-time intrusion detection by:
- Analyzing network traffic samples  
- Detecting malicious activity  
- Generating alerts  
- Evaluating detection accuracy  

---

## Visualizations
- Label distribution plots  
- Client data distribution  
- Correlation heatmaps  
- Model comparison charts  
- Confusion matrices  
- ROC curves  
- Federated convergence graphs  

---

## Technologies Used
- Python  
- NumPy, Pandas  
- Scikit-learn  
- XGBoost  
- Matplotlib, Seaborn  
- Jupyter Notebook  


## Conclusion
This project demonstrates the effectiveness of **Federated Learning in Intrusion Detection Systems**, enabling collaborative model training across distributed networks while preserving data privacy. The system successfully detects both known and unknown cyber threats, making it a scalable and secure solution.
