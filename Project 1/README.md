# Quantum vs Classical Machine Learning Models Comparison

## 🚀 Overview

This project presents a **comparative study between classical machine learning and quantum-enhanced machine learning models** using the Iris dataset.

The objective is to evaluate:

* Model accuracy
* Computational efficiency
* Practical feasibility of quantum machine learning

By implementing both a **classical Support Vector Machine (SVM)** and a **Quantum Support Vector Classifier (QSVC)**, this project highlights the current capabilities and limitations of quantum approaches in real-world scenarios.

---

## 🎯 Objectives

* Implement and evaluate a classical SVM model
* Build a quantum machine learning model using Qiskit
* Compare performance using accuracy, confusion matrix, and execution time
* Analyze strengths and limitations of quantum models
* Understand practical challenges in quantum computing

---

## 🛠️ Tech Stack

* **Programming Language**: Python
* **Classical ML**: Scikit-learn
* **Quantum ML**: Qiskit Machine Learning
* **Data Handling**: NumPy, Pandas
* **Visualization**: Matplotlib
* **Environment**: Jupyter Notebook

---

## 📂 Project Structure

```id="0b8kmr"
Quantum-Computing_ML/
│
├── notebook/
│   └── Project 1: Quantum Vs. Classical ML models comparison.ipynb
│
├── results/
│   └── figures/       
│
├── requirements.txt
└── README.md
```

---

## 📊 Dataset

* **Dataset**: Iris Dataset
* **Samples**: 150
* **Features**:

  * Sepal length
  * Sepal width
  * Petal length
  * Petal width

For model training, only:

* **Petal length**
* **Petal width**

were selected due to better class separability and compatibility with quantum models.

---

## ⚙️ Methodology

### 1. Data Exploration

* Loaded and inspected dataset
* Visualized feature distribution using scatter plots
<img width="894" height="706" alt="image" src="https://github.com/user-attachments/assets/72210bd5-3d0b-4f0a-9460-5de6b9d3ea75" />

### 2. Data Preprocessing

* Selected petal features for better classification
* Split dataset into training (80%) and testing (20%)
* Applied feature scaling using StandardScaler
* <img width="907" height="683" alt="image" src="https://github.com/user-attachments/assets/98240419-64bd-457d-9404-3f0b34cd6217" />


### 3. Classical Model (SVM)

* Implemented linear Support Vector Machine
* Trained on scaled features
* Evaluated using accuracy, classification report, and confusion matrix
* <img width="725" height="553" alt="image" src="https://github.com/user-attachments/assets/085f7e5e-b7bc-4c6a-ab67-9651e0a2ec35" />

### 4. Quantum Model (QSVC)

* Used Qiskit to implement Quantum SVM
* Applied:

  * ZZFeatureMap (data encoding)
  * FidelityQuantumKernel (similarity computation)
* Trained and evaluated on the same dataset
* <img width="721" height="555" alt="image" src="https://github.com/user-attachments/assets/5efaea37-b5a2-4c79-9a2e-4e156fab4972" />

### 5. Performance Comparison

* Compared:

  * Accuracy
  * Execution time
  * Prediction errors
  * <img width="506" height="328" alt="image" src="https://github.com/user-attachments/assets/00a05ab5-2bb8-4cb9-9bf1-ae6d2ea7f754" />




  


---

## 📈 Results

### 🔹 Accuracy Comparison

* **Classical Model (SVM)**: **1.00 (100%)**
* **Quantum Model (QSVC)**: **0.73 (73%)**
* <img width="892" height="716" alt="image" src="https://github.com/user-attachments/assets/48fb4993-6204-4384-894d-9dd839d7b54f" />


### 🔹 Time Comparison

* Classical Model: ~0.001 sec
* Quantum Model: ~14 sec

### 🔹 Confusion Matrix Insights

* Classical model achieved perfect classification
* Quantum model showed misclassifications, especially in overlapping classes
* <img width="503" height="898" alt="image" src="https://github.com/user-attachments/assets/868e562c-6bbe-4579-ae60-669144d7efac" />


---

## 🔍 Key Insights

* Classical models significantly outperform quantum models in this experiment
* Quantum models are:

  * Computationally expensive
  * Sensitive to feature encoding
* Quantum machine learning is still **experimental and evolving**
* Feature selection plays a critical role in performance

---

## 📊 Visualizations

The project includes:

* Scatter plots for data understanding
* Accuracy comparison bar chart
* Confusion matrices for both models

These visualizations provide clear insights into model performance differences.

---

## ▶️ How to Run

### 1. Clone the repository

```bash id="e1k6xv"
git clone https://github.com/BatoolJohn/Quantum-Computing_ML.git
cd Quantum-Computing_ML
```

### 2. Install dependencies

```bash id="q6k7dp"
pip install -r requirements.txt
```

### 3. Run the notebook

```bash id="m8d3zs"
jupyter notebook notebook/Project_1_Quantum_Vs_Classical_ML_models_comparison.ipynb
```

---

## 🚧 Future Improvements

* Test on larger and more complex datasets
* Optimize quantum circuits and feature maps
* Implement hybrid quantum-classical models
* Run experiments on real quantum hardware
* Apply hyperparameter tuning

---

## 💡 Why This Project Matters

This project demonstrates:

* Strong understanding of **machine learning fundamentals**
* Practical experience with **quantum computing frameworks (Qiskit)**
* Ability to perform **comparative experimental analysis**
* Awareness of **real-world limitations of emerging technologies**

---

## 🧠 Conclusion

While quantum computing offers theoretical advantages, this project shows that:

* Classical machine learning models currently provide **better accuracy and efficiency**
* Quantum models are limited by:

  * Simulation overhead
  * Algorithm maturity
  * Hardware constraints

👉 At present, **quantum machine learning is not yet competitive for small-scale practical problems**, but it holds strong potential for future advancements.

---

## 📜 License

This project is licensed under the Apache-2.0 License.

---

## 📬 Contact

**Attiya Batool**

* LinkedIn: https://linkedin.com/in/attiya-b-996b832b
* Email: batooljohn@gmail.com

---

⭐ If you found this project useful, consider giving it a star!
