# Intrusion Detection System using Machine Learning (UNSW-NB15)

This project implements an **Intrusion Detection System (IDS)** that uses machine learning algorithms to detect and classify network intrusions. It is trained on the **UNSW-NB15 dataset**, which includes a wide range of modern attacks. Among the models evaluated, **Random Forest** showed the highest accuracy and is used for final predictions.

---

## Features

- Detects multiple attack types:
  - **Fuzzers**
  - **Exploits**
  - **Generic**
  - **Data Leaks**
- Compares multiple models:
  -  Random Forest *(Best performing)*
  -  Support Vector Machine (SVM)
  -  Gradient Boosting
- Predicts whether a network connection is **Benign** or **Malicious**
- Outputs classification reports, confusion matrices, and accuracy scores

---

##  Models Compared

| Model              | Accuracy | Notes                        |
|-------------------|----------|------------------------------|
| Random Forest      | Highest | Selected for final prediction |
| SVM                | Moderate | Good, but slower on large data |
| Gradient Boosting  | Good     | Competitive, but overfits slightly |

---

##  Dataset

- **Name:** UNSW-NB15
- **Source:** [UNSW Cyber Range Lab](https://www.unsw.adfa.edu.au/unsw-canberra-cyber/cybersecurity/ADFA-NB15-Datasets/)
- **Classes:** Benign and 9 Attack Types (filtered to 4 for this project)

