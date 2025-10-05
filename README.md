# thesis-software
This script predicts the most suitable imputation techniques for a dataset based on meta-features using a trained meta-classifier.



# Meta-Dataset Guided Technique Recommendation

This repository contains the software developed as part of my MSc thesis.  
The system predicts the **top 5 most suitable imputation techniques** based on a given meta-dataset.

---

## 📌 Features
- Load a meta-dataset (CSV format).
- Preprocess and extract meta-features.
- Apply a trained classifier to predict rankings of imputation methods.
- Output the **top 5 recommended techniques**.

---

## 🗂 Repository Structure


thesis-software/
│── src/
│ ├── main.py # entry point
│
│── data/
│ ├── meta_dataset_sample.csv # example dataset
│
│── models/
│ ├── trained_model.pkl # optional pre-trained classifier
│
│── requirements.txt
│── README.md
│── LICENSE



## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Hayaelshaweesh/thesis-software.git
   cd thesis-software


2. Install dependencies:
pip install -r requirements.txt



