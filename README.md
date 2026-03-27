# 🩺 Multi Disease Prediction System

<img width="1915" height="1033" alt="Screenshot 2026-03-27 151732" src="https://github.com/user-attachments/assets/9190b698-b9e5-4d3e-9683-8a8040870544" />


## 📌 Project Overview

The **Multi Disease Prediction System** is a machine learning application that predicts possible diseases based on user-selected symptoms. The system uses a trained classification model to analyze symptom patterns and output the most probable disease along with prediction confidence.

This project demonstrates the use of **machine learning, data preprocessing, and interactive visualization** to assist in early disease detection.

The application provides:

* Disease prediction based on symptoms
* Confidence probability for predictions
* Visualization of prediction scores
* Identification of key symptoms contributing to the prediction

---

# 🎯 Objectives

* Build a machine learning model that predicts diseases from symptoms
* Provide probability-based predictions instead of a single label
* Create an interactive interface for user input
* Visualize prediction results for better interpretability

---

# 🧠 Machine Learning Model

The system uses **XGBoost Classifier**, a powerful gradient boosting algorithm known for high performance on tabular datasets.

### Model Parameters

* `n_estimators = 200`
* `max_depth = 6`
* `learning_rate = 0.05`
* `subsample = 0.8`
* `colsample_bytree = 0.8`
* `objective = multi:softprob`
* `eval_metric = mlogloss`

### Why XGBoost?

* High accuracy on structured datasets
* Handles multi-class classification efficiently
* Provides probability outputs
* Resistant to overfitting with proper tuning

---

# 📂 Project Structure

```
project_root/
│
├── dataset/
│   ├── training.csv
│   └── testing.csv
│
├── notebook/
│   └── multi_disease_prediction.ipynb
│
├── output/
│   └── models/
│       ├── disease_prediction_model.pkl
│       └── label_encoder.pkl
│
├── app.py
└── README.md
```

---

# ⚙️ Technologies Used

* Python
* Streamlit
* XGBoost
* Scikit-learn
* Pandas
* NumPy
* Matplotlib

---

# 🔄 Workflow

### 1️⃣ Data Collection

The dataset contains symptom–disease relationships used to train the model.

### 2️⃣ Data Preprocessing

* Symptom encoding
* Label encoding for diseases
* Feature selection

### 3️⃣ Model Training

The XGBoost classifier is trained using the processed dataset.

### 4️⃣ Model Saving

The trained model and label encoder are saved using pickle.

### 5️⃣ Prediction System

Users select symptoms through the interface, and the model predicts the most probable disease.

### 6️⃣ Visualization

Prediction probabilities are displayed using charts to help users understand model confidence.

---

# 📊 Output

The system produces:

* Predicted disease
* Prediction confidence score
* Probability distribution chart
* Key symptoms visualization

---

# 🚀 How to Run the Project

### 1️⃣ Clone Repository

```
git clone https://github.com/your-username/multi-disease-prediction.git
```

### 2️⃣ Navigate to Project Folder

```
cd multi-disease-prediction
```

### 3️⃣ Install Dependencies

```
pip install -r requirements.txt
```

### 4️⃣ Run the Application

```
streamlit run app.py
```

---

# 💡 Example Prediction

Input Symptoms:

* Fever
* Headache
* Body Pain

Output:

```
Predicted Disease: Dengue
Confidence: 82%
```

---

# 🔮 Future Improvements

* Deep learning models for improved accuracy
* Real-time symptom extraction from text input
* Integration with medical knowledge bases
* Mobile application deployment

---

# ⚠️ Disclaimer

This system is intended for **educational and research purposes only**.
It should **not replace professional medical diagnosis**.

---

# 👨‍💻 Author

**Yashwardhan Shinde**

B.Tech CSE (AI & Data Analytics)

---

# 📜 License

This project is open-source and available for educational use.
