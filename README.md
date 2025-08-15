# 👤 Gender Classification by Names using Machine Learning

## 📌 Overview
This project predicts a person's gender (Male or Female) based solely on their **first name** using machine learning models.  
Two main approaches were implemented:
1. **Naive Bayes Classifier** using `CountVectorizer` on names.
2. **Decision Tree Classifier** using custom name-based features (first letter, last letter, etc.).

Both models are trained and stored for later use.

---

## 📂 Dataset
- **File**: `Names_dataset.csv`
- **Rows**: 125,231
- **Columns**:  
  - `name` — Person's first name  
  - `gender` — Gender label (`m` = Male, `f` = Female)

### Class Distribution:
- Female: **151,942 names**
- Male: **98,520 names**

---

## 🛠 Data Preprocessing
1. **Label Encoding**
   - `f` → `0` (Female)  
   - `m` → `1` (Male)

2. **Missing Values**
   - No missing data found.

3. **Vectorization Approaches**
   - **CountVectorizer**: Converts names into bag-of-words format for Naive Bayes.
   - **DictVectorizer**: Encodes custom dictionary-based features for Decision Tree.

---

🤖 Models Used
1️⃣ Naive Bayes Classifier (with CountVectorizer)
Train Accuracy: ~99.13%

Test Accuracy: ~71.04%

Stores the trained vectorizer in gender_vectorizer.pkl

Stores the trained model in naivebayes.pkl

2️⃣ Decision Tree Classifier (with Custom Features)
Uses extracted letter patterns for classification.

Stores the trained model in decisiontree.pkl and name_detector_model.pkl


---
📦 Dependencies

Python 3.x

pandas

numpy

scikit-learn

joblib

pickle

---

🔮 Future Improvements

Use character-level embeddings with deep learning for better accuracy.

Expand dataset with more international names.

Build a Streamlit web app for interactive gender prediction.

Add probability scores for predictions.

---
📜 License

This project is licensed under the MIT License.

---

Author
SANIYA CHHABRA
