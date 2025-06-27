# 🛡️ Phishing Website Detection using Ensemble Learning and Neural Networks

This project implements a **machine learning-based phishing detection system** using a dataset of URLs. It integrates classical ML models (Random Forest, Gradient Boosting, LightGBM) with Neural Networks to accurately classify whether a URL is legitimate or malicious.

---

## 📁 Repository Contents

| File Name             | Description |
|----------------------|-------------|
| `1.py` – `4.py`       | Experimental/trial scripts (data loading, testing, training, etc.) |
| `model.py`            | Main script to train the final ML/ensemble model |
| `source_code.py.py`   | Possibly the full pipeline (naming can be cleaned) |
| `a3.pickle`           | Serialized trained model using `pickle` |
| `dataset_phishing.csv`| Dataset used for training and testing |
| `README.md`           | Project documentation (you’re reading it!) |

---

## 📊 Dataset

The dataset used is a labeled collection of phishing and legitimate URLs with extracted features like:
- URL length
- Presence of IP address
- Special characters
- Use of HTTPS
- Domain age

📥 Download similar datasets from:
- [Kaggle Phishing Detection Dataset](https://www.kaggle.com/datasets/madhan123/phishing-detection-dataset)
- [UCI Phishing Websites Data Set](https://archive.ics.uci.edu/ml/datasets/phishing+websites)

> **Note**: If the dataset is missing in your clone, please download manually and place it as `dataset_phishing.csv` in the root directory.

---

## 🧠 Models Used

The following machine learning models are used individually and in ensembles:

- ✅ Random Forest
- ✅ Gradient Boosting
- ✅ LightGBM
- ✅ Isolation Forest (for anomaly detection)
- ✅ Neural Networks (Feedforward NN)
- ✅ Stacking Classifier
- ✅ Voting (Soft & Hard)

---

## 🛠️ How to Run

1. **Install required packages**:
```bash
pip install pandas scikit-learn lightgbm matplotlib seaborn
```

2. **Run model training** (if needed):
```bash
python model.py
```

3. **Run inference using the saved model**:
```bash
python source_code.py.py
```

> Note: File names like `source_code.py.py` should ideally be renamed to something cleaner like `app.py`.

---

## 📈 Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC-AUC**

Example performance:
| Model               | Accuracy |
|--------------------|----------|
| Random Forest       | 96.5%    |
| Gradient Boosting   | 97.3%    |
| Stacked Ensemble    | **98.2%**|

---

## 👩‍💻 Developed By

- Satram Prashanti Sai  
- Kashetty Jahnavi Chakravarthy  
- Nareddy Sushank Reddy  
- Vippakayala Rahul

**Under the guidance of**: Mrs. B. Spandana  
Dept. of CSE (AI & ML), Sreyas Institute of Engineering and Technology

---

## 📜 License

This project is intended for **academic and research purposes only**.  
For commercial or deployment inquiries, please contact the authors or advisor.

