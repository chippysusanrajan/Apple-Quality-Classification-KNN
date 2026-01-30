# 🍎 Apple Quality Classification using K-Nearest Neighbours (KNN)

## 📌 Project Overview
This project applies **machine learning classification techniques** to assess the quality of apples based on physical and sensory attributes.  
The goal is to classify apples as **“Good”** or **“Bad”**, supporting data-driven decision-making in an **agricultural quality control** context.

A **K-Nearest Neighbours (KNN)** classifier was implemented and evaluated using multiple performance metrics.

---

## 📊 Dataset Description
The dataset contains numerical features describing apple characteristics:

| Feature | Description |
|------|-----------|
| Size | Physical size of the apple |
| Weight | Weight of the apple |
| Sweetness | Degree of sweetness |
| Crunchiness | Texture indicating crunchiness |
| Juiciness | Level of juiciness |
| Ripeness | Stage of ripeness |
| Acidity | Acidity level |
| Quality | Target variable (Good / Bad) |

---

### Target Variable
- **Quality**: Categorical  
  - `Good`
  - `Bad`

---

## 🧠 Methodology

### 1️⃣ Data Splitting
- Dataset split into **training(80%) and test sets(20%)**
- Ensured fair evaluation of model performance

### 2️⃣ Data Preprocessing
- Applied **feature scaling (standardisation)**  
- Necessary due to the **distance-based nature of KNN**

### 3️⃣ Model Implementation
- Implemented **K-Nearest Neighbours classifier**
- Reason: KNN was chosen due to its simplicity and effectiveness for classification tasks where feature similarity is meaningful.
- Number of neighbours selected using a predefined rule based on one's University Student ID(e.g., zID mod 5 + 2 )
- Used Euclidean distance for classification

### 4️⃣ Model Evaluation
The model was evaluated on unseen test data using:
### Overall Performance
- **Accuracy:** **88%**

### Classification Metrics
- **Precision**
  - Bad: **0.83**
  - Good: **0.94**
- **Recall**
  - Bad: **0.95**
  - Good: **0.80**
- **F1-score**
  - Bad: **0.89**
  - Good: **0.87**
---

## 📈 Results & Insights
- The model is highly effective at identifying **bad-quality apples**, reducing the risk of poor produce reaching customers.
- Feature scaling significantly improved model reliability
- Evaluation metrics provided insight into trade-offs between false positives and false negatives
- Some high-quality apples are misclassified as bad, which could impact revenue.
- Overall, the model demonstrates a strong balance between precision and recall.
- Results demonstrate the suitability of KNN for structured, numerical classification problems

---

## 🛠 Tools & Technologies
- Python  
- Pandas & NumPy  
- scikit-learn  
- KNN Classification
- Feature Scaling & Outlier Detection
- Model Evaluation Metrics 

---

## 📂 Repository Structure
├── data/  
│   └── apple_quality.csv  
├── notebooks/  
│   └── apple_quality_knn.ipynb    
├── README.md  

---

## 🔗 Project Context
This project demonstrates practical skills in:
- Data preprocessing for real-world datasets
- Distance-based machine learning models
- Model evaluation and interpretation
- Translating analytical results into business-relevant insights

---

## 🚀 How to Run This Project

1. Clone the repository:
```bash
git clone https://github.com/chippysusanrajan/apple_quality_knn.git
exit 0

2. Install dependencies:  

pip install -r requirements.txt  

3. Run the notebook or script to train and evaluate the model.

---


---

## 👩‍💻 Author
**Chippy Susan Rajan**  
Master of Data Science and Decisions, UNSW  
📎 [LinkedIn](https://www.linkedin.com/in/chippy-susan-rajan-b1433ab2/)  
🐙 [GitHub](https://github.com/chippysusanrajan)

---

## 📄 License
This project is for academic and portfolio purposes.

