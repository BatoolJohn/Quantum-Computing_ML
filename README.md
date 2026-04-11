# ⚛️ Grover’s Algorithm with Noise Analysis

## 🚀 Overview

This project demonstrates **Grover’s Search Algorithm**, a fundamental quantum algorithm used to locate a target element in an unsorted database with quadratic speedup over classical methods.

The project also explores the **impact of quantum noise** on algorithm performance by comparing ideal (noise-free) and realistic (noisy) simulations using Qiskit.

---

## 🎯 Objectives

* Implement Grover’s Algorithm for a 2-qubit system
* Search for a specific target state (`01`)
* Simulate ideal quantum behavior
* Introduce depolarizing noise
* Analyze performance degradation due to noise

---

## ⚛️ Key Quantum Concept

### 🔍 Grover’s Search Algorithm

Grover’s algorithm amplifies the probability of a target state in an unsorted search space.

### 📊 Search Space:

* Number of qubits: 2
* Total states: 4 → `00`, `01`, `10`, `11`

### 🎯 Target State:

```
01
```

---

## ⚙️ Algorithm Structure

Grover’s algorithm consists of four main steps:

1. **Superposition**
   Creates equal probability across all states

2. **Oracle**
   Marks the target state by flipping its phase

3. **Diffusion Operator**
   Amplifies the probability of the marked state

4. **Measurement**
   Returns the final result

📌 *For N = 4, only one Grover iteration is required.*

---

## 🔧 Oracle Design

To mark the target state `01`, the circuit:

* Applies an X gate to transform `01 → 11`
* Applies a Controlled-Z (CZ) gate to flip the phase of `|11⟩`
* Reverses the transformation
*   <img width="496" height="115" alt="image" src="https://github.com/user-attachments/assets/1f73dea6-62a5-4e2a-95d0-a9dbd7a1cad8" />

This ensures only the target state is marked for amplification.

---

## 📊 Results

### ✅ Ideal Simulation (No Noise)

```id="c8u7xi"
{'01': 1024}
```

* Success Probability: **1.0**
* The algorithm perfectly identifies the target state

---

### 🔊 Noisy Simulation (10% Depolarizing Noise)

```id="1g6m53"
{'01': 505, '11': 196, '10': 134, '00': 189}
```

* Success Probability: **~0.49**

---

## 📉 Performance Analysis

| Condition | Success Probability |
| --------- | ------------------- |
| Ideal     | 1.0                 |
| Noisy     | ~0.49               |

📌 *As shown in the chart (page 8), noise significantly reduces performance.* 

---

## 📊 Visualization

* Bar chart comparison of success probabilities
* Clearly illustrates degradation from ideal to noisy execution
* <img width="621" height="443" alt="image" src="https://github.com/user-attachments/assets/3a24b5d7-9883-4255-9844-796e216d5ac8" />


---

## ⚠️ Key Insights

* Grover’s algorithm performs perfectly in ideal conditions
* Noise introduces incorrect states and reduces success probability
* Quantum advantage diminishes as noise increases

---

## 🧠 Conclusion

This project highlights the sensitivity of quantum algorithms to noise.

### 🔍 Key Learnings:

* Grover’s algorithm efficiently finds target states in ideal environments
* Noise disrupts amplitude amplification
* Real-world quantum computing requires error mitigation

### 🚀 Final Thought:

While quantum algorithms provide computational advantages, **managing noise is essential for practical implementation**.

---

## 🛠️ Tech Stack

* Python
* Qiskit
* Qiskit Aer Simulator
* Matplotlib

---

## 📂 Project Structure

```id="fjokrs"
Grover-Noise-Analysis/
│── Project 4. Quantum Noise Analysis using Grover’s Algorithm.ipynb
│── README.md
│── requirements.txt
```

---

## 📦 Installation

```bash id="c2u9dz"
pip install -r requirements.txt
```

---

## 🔮 Future Improvements

* Implement quantum error correction
* Run on real quantum hardware (IBM Quantum)
* Analyze larger search spaces
* Compare different noise models

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
