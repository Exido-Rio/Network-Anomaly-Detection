## Network Anomaly Detection  
A Random Forest-based approach for detecting anomalies and potential intrusions in network traffic.

## Overview  
Purpose: Identify unusual network behaviors (malicious activities, intrusions) by modeling normal traffic and flagging outliers.  
Data: Uses the NSL-KDD dataset, an enhanced version of KDD Cup 1999 commonly used in intrusion detection research.  
Algorithm: Random Forest ensures robust classification through ensemble decision trees, bootstrapping, and voting.

## How It Works  
1. Data Preparation  
   • Load and explore the NSL-KDD dataset (training and test splits).  
   • Clean and preprocess the network traffic attributes.  

2. Feature Extraction  
   • Transform categorical features (e.g., protocol type) into numeric form (one-hot encodings).  
   • Assign labels for normal or various attack categories (DoS, Probe, Privilege Escalation, Access).  

3. Model Training  
   • Initialize a RandomForestClassifier with random_state for reproducibility.  
   • Train on labeled data (either binary or multi-class).  
   • Evaluate against a test set to measure accuracy, precision, recall, and F1-score.

## Usage  
Clone the repo:  
```bash
git clone https://github.com/YourUsername/Network-Anomaly-Detection.git
cd Network-Anomaly-Detection
