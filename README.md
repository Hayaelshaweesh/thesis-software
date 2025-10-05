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

3.Run predictions with:
python src/main.py --input data/meta_dataset_sample.csv --top 5

4. Example output:
**Top 5 recommended imputation techniques:**
1. KNN Imputer
2. MissForest
3. Mean Imputation
4. MICE
5. Median Imputation




## 📘 Notes

trained_model.pkl must be placed inside models/.
meta_dataset_sample.csv is provided as an example input.
For reproducibility, the original Colab notebook is included (thesis_notebook.ipynb).
