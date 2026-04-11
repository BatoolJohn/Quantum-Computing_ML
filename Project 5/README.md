# ⚛️ Variational Quantum Classifier (VQC) with Classical Comparison

A research-oriented implementation of a **Variational Quantum Classifier (VQC)** using Qiskit, compared against a classical Logistic Regression model on a noisy binary classification dataset.

---

## 🚀 Project Overview

This project explores the capabilities and limitations of **quantum machine learning** by implementing a hybrid quantum-classical model and evaluating its performance against a classical baseline.

### 🎯 Objectives:

* Build a **Variational Quantum Classifier (VQC)**
* Train using classical optimization (COBYLA)
* Compare with **Logistic Regression**
* Analyze:

  * Training behavior
  * Model accuracy
  * Effect of quantum noise
  * Decision boundaries

---

## 🧠 Key Features

* ⚛️ Multi-layer Variational Quantum Circuit (VQC)
* 🔁 Classical optimization using SciPy (COBYLA)
* 📉 Training loss tracking and visualization
* 🔊 Noise simulation using Qiskit Aer
* 📊 Classical vs Quantum performance comparison
* 🧭 Decision boundary visualization

---

## 🗂️ Project Structure

```
📦 Quantum-Computing_ML
 ┣ 📜 Project_5_Hybrid_Quantum_Classical_Machine_Learning.ipynb
 ┣ 📜 README.md
 ┗ 📜 requirements.txt
```

---

## ⚙️ Installation

```bash
pip install qiskit qiskit-aer numpy matplotlib scikit-learn scipy
```

---

## 📊 Dataset

A synthetic dataset is generated using `make_classification` with:

* **2 features** (for visualization)
* **Low class separation (0.4)**
* **Noise introduced (flip_y = 0.2)**

👉 This creates a **challenging classification problem** with overlapping classes.

---

## 🧠 Classical Model

A **Logistic Regression** model is used as a baseline.

### Result:

```
Accuracy: ~0.80
```

### Interpretation:

* Performs well despite noise
* Serves as a strong benchmark

---

## ⚛️ Quantum Model (VQC)

### Architecture:

* 2 qubits
* RY encoding of features
* Multi-layer parameterized rotations
* CNOT entanglement

### Training:

* Optimizer: COBYLA
* Loss: Mean Squared Error

---

## 📉 Training Behavior

The loss curve shows:

* Initial decrease in loss
* Convergence after several iterations
* Plateau indicating limited model capacity

👉 Confirms that training is working correctly.

---

## 📊 Results

| Model                           | Accuracy |
| ------------------------------- | -------- |
| Classical (Logistic Regression) | ~0.80    |
| Quantum (Ideal Simulator)       | ~0.43    |
| Quantum (Noisy Simulator)       | ~0.43    |

---

## 🔊 Noise Analysis

A depolarizing noise model was introduced:

* Single-qubit and two-qubit errors
* Simulates real quantum hardware conditions

### Observation:

* No significant drop in performance
* Indicates model is already underfitting

---

## 🧭 Decision Boundary

The quantum model produces:

* Smooth probability gradients
* No sharp class separation

### Interpretation:

* Model outputs uncertain predictions
* Confirms limited expressive power

---

## ⚠️ Key Findings

### 1. Classical Models Outperform Quantum Models (Here)

For this dataset:

* Logistic Regression performs significantly better
* VQC struggles due to limited circuit complexity

---

### 2. Quantum Models Require Careful Design

Performance depends on:

* Circuit depth
* Ansatz design
* Feature encoding

---

### 3. Noise Is Not Always the Main Limitation

* Noise had minimal impact in this case
* Model capacity was the primary bottleneck

---

### 4. Optimization Converges but Hits Limits

* Training successfully reduces loss
* Model cannot achieve high accuracy

---

## 🏁 Conclusion

This project demonstrates that while Variational Quantum Classifiers can be trained successfully, they do not automatically outperform classical models.

### 🔍 Key Takeaways:

* Classical ML remains highly effective for low-dimensional problems
* Quantum models require deeper circuits and better design
* Noise is important but not always the dominant factor
* Achieving quantum advantage remains an open challenge

---

## 🔮 Future Improvements

* Increase circuit depth and number of parameters
* Use advanced ansätze (hardware-efficient circuits)
* Explore richer feature encoding techniques
* Test on higher-dimensional datasets
* Run experiments on real quantum hardware
* Apply error mitigation strategies

---

## 🛠️ Technologies Used

* Python
* Qiskit
* Qiskit Aer
* NumPy
* Scikit-learn
* Matplotlib
* SciPy

---

## 📌 How to Run

1. Clone the repository
2. Install dependencies
3. Open the notebook:

```bash
jupyter Project_5_Hybrid_Quantum_Classical_Machine_Learning.ipynb
```

4. Run all cells sequentially

---


## ⭐ Acknowledgment

This project is part of an exploration into **Quantum Machine Learning**, demonstrating both the **potential and limitations** of current quantum approaches.

---

## 📢 Final Note

> Quantum Machine Learning is promising, but practical advantage requires careful problem selection, circuit design, and hardware improvements.

---


## 📜 License

Apache-2.0 License

---

## 📬 Contact

**Attiya Batool**
LinkedIn: https://linkedin.com/in/attiya-b-996b832b
Email: batooljohn@gmail@com

---

⭐ If you found this project useful, consider giving it a star!
