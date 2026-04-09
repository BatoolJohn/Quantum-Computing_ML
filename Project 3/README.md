# ⚛️ Quantum Noise Analysis using Bell State

## 🚀 Overview

This project explores the impact of **quantum noise** on an entangled quantum system using a **Bell state circuit**. By simulating both ideal and noisy environments, the project demonstrates how real-world imperfections affect quantum computation reliability.

The implementation is carried out using **Qiskit** and focuses on understanding noise behavior in quantum systems.

---

## 🎯 Objectives

* Create a Bell state using quantum gates
* Simulate ideal (noise-free) quantum behavior
* Introduce depolarizing noise into the system
* Analyze accuracy and error rates
* Study the impact of varying noise levels

---

## ⚛️ Key Quantum Concept

### 🔗 Bell State (Entanglement)

A Bell state is a maximally entangled quantum state of two qubits:

*<img width="310" height="101" alt="image" src="https://github.com/user-attachments/assets/500f624b-d5f5-4284-94c4-c13f1c17b346" />

### 📌 Key Property:

* Measurement results are always **correlated**
* Only two outcomes appear:

  * `00`
  * `11`

This reflects perfect quantum entanglement.

---

## 🛠️ Tech Stack

* Python
* Qiskit
* Qiskit Aer Simulator
* Matplotlib

---

## 🔬 Methodology

### 1️⃣ Bell State Circuit

* Apply Hadamard gate → superposition
* Apply CNOT gate → entanglement
* Measure qubits
* <img width="362" height="181" alt="image" src="https://github.com/user-attachments/assets/5cf534c1-b2f6-4ca7-a842-b1620cddace2" />

---

### 2️⃣ Ideal Simulation

* Run circuit without noise
* Expected output:

  * Only `00` and `11`
  * Nearly equal probabilities
  * <img width="726" height="57" alt="image" src="https://github.com/user-attachments/assets/64bdf0b4-3cbd-4318-95eb-399ac7a3427d" />


---

### 3️⃣ Noise Modeling

* Apply **depolarizing noise (10%)**
* Added to:

  * Single-qubit gates (H)
  * Two-qubit gates (CX)

---

### 4️⃣ Noisy Simulation

Example output:

```
{'00': 459, '11': 502, '01': 33, '10': 30}
```

### 🔍 Observation:

* Correct states: `00`, `11`
* Error states: `01`, `10`

---

### 5️⃣ Visualization

* Histogram comparison:

  * Ideal vs Noisy results
* Shows probability distribution changes due to noise
* <img width="967" height="745" alt="image" src="https://github.com/user-attachments/assets/c8fdf825-4415-4217-9ff1-03aecbf07b89" />


---

### 6️⃣ Noise Impact Analysis

| Metric     | Value  |
| ---------- | ------ |
| Accuracy   | 93.85% |
| Error Rate | 6.15%  |
*<img width="380" height="180" alt="image" src="https://github.com/user-attachments/assets/004e5887-fe58-478e-bca0-bf841a5266fc" />

### 📌 Insight:

Even small noise introduces measurable errors in quantum systems.

---

### 7️⃣ Noise Level Experiment

Tested noise levels:

* 5%
* 10%
* 20%

| Noise Level | Effect                  |
| ----------- | ----------------------- |
| 0.05        | Near ideal results      |
| 0.10        | Moderate errors         |
| 0.20        | Significant degradation |

*<img width="641" height="252" alt="image" src="https://github.com/user-attachments/assets/de685a69-6bd6-458f-9100-37c1f5f11383" />

### 📊 Key Insight:

As noise increases:

* Accuracy decreases
* Error states increase
* <img width="957" height="740" alt="image" src="https://github.com/user-attachments/assets/734f8678-1404-4105-9991-7f6af91bf76e" />


---

## 📊 Results Summary

* Ideal system produces perfectly correlated outputs
* Noise introduces incorrect states
* System reliability decreases with noise

---

## ⚠️ Challenges

* Quantum systems are highly sensitive to noise
* Error rates increase rapidly with noise levels
* Real quantum hardware requires advanced error mitigation

---

## 💡 Why This Project Matters

This project demonstrates:

* Understanding of **quantum entanglement**
* Practical implementation of **noise models**
* Ability to analyze **quantum system reliability**
* Hands-on experience with **quantum simulation tools**

---

## 🚀 Future Improvements

* Implement quantum error correction techniques
* Run experiments on real quantum hardware
* Explore advanced noise models
* Extend to multi-qubit systems

---

## 🧠 Conclusion

Quantum computing offers powerful computational advantages, but **noise remains a fundamental challenge**.

This project highlights the importance of:

* Noise modeling
* Error analysis
* Robust quantum system design

---

## 📂 Project Structure

```
Quantum-Noise-Analysis/
│── notebook.ipynb
│── README.md
│── requirements.txt
```

---

## 📦 Installation

```bash
pip install -r requirements.txt
```

---

## 📜 License

Apache-2.0 License

---

## 📬 Contact

**Attiya Batool**
LinkedIn: https://linkedin.com/in/attiya-b-996b832b
Email: batooljohn@gmail.com)

---

⭐ If you found this project useful, consider giving it a star!
