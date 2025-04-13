# Detecting and Defending Against IoT Intrusions Leveraging Data for Enhanced Security

## 📌 Project Overview

This project focuses on developing a robust machine learning-based framework to detect and defend against intrusion attempts in Internet of Things (IoT) environments. Using advanced data analysis and classification algorithms, the system leverages network traffic data to identify and classify malicious activities, enhancing the overall security of IoT infrastructures.

This work is being published in **Springer Nature SNAPP, Journal of Network and Systems Management**.

---

## 🔍 Objectives

- Analyze IoT network traffic using real-world intrusion datasets.
- Apply feature engineering to improve detection accuracy.
- Train multiple machine learning models (e.g., Random Forest, SVM, Neural Networks).
- Evaluate and compare models on classification performance metrics.
- Propose defensive mechanisms based on data insights.

---

## 📁 Project Structure

```
IoT-Intrusion-Detection/
│
├── data/
│   ├── CICIDS2017.csv            # Cleaned and preprocessed dataset
│   ├── features_selected.csv     # Feature-selected dataset
│
├── models/
│   ├── random_forest.pkl         # Trained model
│   └── svm_model.pkl
│
├── notebooks/
│   └── analysis.ipynb            # Full exploratory and model training notebook
│
├── src/
│   ├── preprocessing.py          # Data cleaning and encoding
│   ├── feature_selection.py      # Feature selection techniques
│   ├── model_training.py         # ML model training
│   └── evaluation.py             # Metrics calculation
│
├── report/
│   └── Final_Report.pdf          # Research report (max 3 pages)
│
├── README.md
├── requirements.txt
└── run.py                        # Script to execute the pipeline
```

---

## 🧪 Dataset Used

**CICIDS2017 Dataset** – Provided by the Canadian Institute for Cybersecurity.  
It includes labeled attack traffic for various intrusion scenarios (DDoS, PortScan, Brute Force, etc.).

Dataset link: https://www.unb.ca/cic/datasets/ids-2017.html

---

## ⚙️ Installation and Setup

1. **Clone the Repository**
```bash
git clone [https://github.com/your-username/IoT-Intrusion-Detection.git](https://github.com/srinithshrajkumar/Detecting-and-Defending-Against-IoT-Intrusions-Leveraging-Data-for-Enhanced-Security/blob/main/Detecting%20and%20Defending%20Against%20IoT%20Intrusions%20Leveraging%20Data%20for%20Enhanced%20Security%20Source%20Code.ipynb)

cd IoT-Intrusion-Detection
```

2. **Create a Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install Dependencies**
```bash
pip install -r requirements.txt
```

---

## 🚀 Running the Project

1. **Preprocess and Train Models**
```bash
python run.py
```

2. **Notebook for Analysis**
Open `notebooks/analysis.ipynb` in JupyterLab or VSCode for step-by-step execution.

---

## 📊 Evaluation Metrics

Models are evaluated using the following:
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- ROC Curve and AUC
- Feature Importance Visualization

---

## 🛡️ Key Findings

- Random Forest provided the highest accuracy (~99%) in intrusion classification.
- Top contributing features included `Flow Duration`, `Dst Port`, `Packet Length`, and `Flow Bytes/s`.
- Feature selection significantly improved both performance and model generalization.

---

## 💡 Future Enhancements

- Incorporate Deep Learning architectures (LSTM, CNNs).
- Integrate real-time detection using stream-processing frameworks.
- Extend the framework for federated learning on edge IoT devices.

---
