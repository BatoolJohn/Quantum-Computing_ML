# ⚛️ Quantum Computing & Machine Learning Portfolio

A comprehensive portfolio showcasing hands-on implementation of **quantum computing algorithms**, **quantum machine learning models**, and **noise analysis techniques** using Qiskit.

This repository demonstrates a structured exploration of:

* Quantum algorithms
* Quantum vs Classical comparisons
* Noise effects in quantum systems
* Hybrid quantum-classical machine learning

---

## 🚀 Overview

Quantum computing promises significant advantages over classical computation in specific domains.
This repository explores:

* When quantum methods work
* When they fail
* What limits their performance today

Each project is designed as an **experimental study**, focusing on both:

✔️ Implementation
✔️ Critical analysis

---

## 🧠 Learning Journey & Project Progression

This repository follows a logical progression:

### 🔹 1. Classical vs Quantum Machine Learning

➡️ Understanding whether quantum ML provides real advantages

### 🔹 2. Quantum Search Algorithms

➡️ Exploring theoretical speedups (Grover’s Algorithm)

### 🔹 3. Quantum Noise & Reliability

➡️ Studying real-world limitations of quantum systems

### 🔹 4. Hybrid Quantum-Classical Models

➡️ Implementing trainable quantum models (VQC)

---

## 📂 Projects

---

### 🟦 1. Quantum vs Classical Machine Learning (QSVM vs SVM)

📁 Folder: `Project 1`

* Implemented:

  * Classical Support Vector Machine (SVM)
  * Quantum Support Vector Classifier (QSVC)

* Dataset: Iris (petal features)

### 📊 Key Results:

* Classical Accuracy: **100%**
* Quantum Accuracy: **73%**
* Quantum execution significantly slower

### 🧠 Insight:

> Classical models outperform quantum models on small structured datasets.

---

### 🟦 2. Grover’s Algorithm (Quantum vs Classical Search)

📁 Folder: `Project 2`

* Implemented:

  * Classical linear search (O(N))
  * Grover’s quantum search (O(√N))

### 📊 Key Results:

* Quantum finds solution faster (theoretically)
* Simulation overhead makes it slower in practice

### 🧠 Insight:

> Quantum advantage exists theoretically but not yet practically in small systems.

---

### 🟦 3. Quantum Noise Analysis (Bell State)

📁 Folder: `Project 3`

* Created entangled Bell state
* Simulated depolarizing noise

### 📊 Key Results:

* Ideal: only `00`, `11`
* Noisy: additional incorrect states
* Accuracy decreases with noise

### 🧠 Insight:

> Even small noise significantly impacts quantum systems.

---

### 🟦 4. Grover’s Algorithm with Noise

📁 Folder: `Project 4`

* Extended Grover’s algorithm with noise simulation

### 📊 Key Results:

* Ideal success probability: **1.0**
* Noisy success probability: **~0.49**

### 🧠 Insight:

> Noise reduces quantum advantage and introduces uncertainty.

---

### 🟦 5. Variational Quantum Classifier (VQC)

📁 Folder: `Project 5`

* Built a hybrid quantum-classical model
* Used:

  * Parameterized circuits
  * Classical optimization (COBYLA)

### 📊 Key Results:

* Classical Accuracy: **~0.80**
* Quantum Accuracy: **~0.43**

### 🧠 Insight:

> Quantum models can learn but often underperform due to limited circuit expressivity.

---

## ⚠️ Key Global Insights

Across all projects, several important conclusions emerge:

---

### 🔹 1. Classical Models Are Still Strong

* Faster
* More accurate (in small datasets)
* More stable

---

### 🔹 2. Quantum Advantage Is Context-Dependent

* Exists theoretically (e.g., Grover’s Algorithm)
* Not always visible in practical implementations

---

### 🔹 3. Noise Is a Major Challenge

* Degrades performance significantly
* Limits real-world usability
* Requires error mitigation techniques

---

### 🔹 4. Model Design Matters

Quantum performance depends heavily on:

* Circuit depth
* Feature encoding
* Ansatz design

---

### 🔹 5. Quantum ML Is Still Emerging

* Promising but immature
* Requires better hardware and algorithms

---

## 🛠️ Technologies Used

* **Python**
* **Qiskit**
* **Qiskit Aer Simulator**
* **Scikit-learn**
* **NumPy**
* **Matplotlib**
* **SciPy**

---

## ▶️ How to Run

```bash
git clone https://github.com/BatoolJohn/Quantum-Computing_ML.git
cd Quantum-Computing_ML
pip install -r requirements.txt
jupyter notebook
```

---

## 🔮 Future Work

* Run experiments on real quantum hardware (IBM Quantum)
* Explore deeper quantum circuits
* Implement quantum error correction
* Test on larger datasets
* Investigate quantum advantage scenarios

---

## 🏁 Final Conclusion

This portfolio demonstrates both the **potential and limitations of quantum computing**.

### 🔍 Key Takeaway:

> Quantum computing is powerful in theory, but practical advantages are currently limited by noise, hardware constraints, and algorithm maturity.

---

## 👨‍💻 Author

**Attiya Batool**

* LinkedIn: https://linkedin.com/in/attiya-b-996b832b
* Email: [batooljohn@gmail.com](mailto:batooljohn@gmail.com)

---

## ⭐ Support

If you found this repository useful:

⭐ Star the repo
📢 Share it
💬 Connect with me

---


