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
│  │── shf_mvi_main_class.py # entry point
│── data/
│ ├── meta_dataset_sample.csv # example dataset
│── models/
│ ├── predict_top_k.pkl 
│ ├── train_rf_model.pkl 
│── requirements.txt
│── README.md


## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Hayaelshaweesh/thesis-software.git
   cd thesis-software


2. Install dependencies:
pip install -r requirements.txt  
pip install --only-binary=:all: -r requirements.txt


3. Training:
python models/train_rf_model.py


4. Run predictions with:
python src/shf_mvi_main_class.py --input data/meta_dataset_sample.csv --model models/SHF_MVI_model.pkl --encoder models/encoder.pkl --scaler models/scaler.pkl --columns models/column_info.pkl --top 5

5. Example output:
**Top 5 recommended imputation techniques:**
1. KNN Imputer
2. MissForest
3. Mean Imputation
4. MICE
5. Median Imputation
