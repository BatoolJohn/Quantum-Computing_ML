# Grover’s Algorithm: Quantum vs Classical Search with Noise Analysis

## 🚀 Overview

This project implements **Grover’s Algorithm**, a fundamental quantum search algorithm, and compares it with a **classical linear search** approach.

In addition, the project explores the **impact of quantum noise** on algorithm performance using simulation.

The goal is to demonstrate:

* Quantum speedup in search problems
* Differences between classical and quantum computation
* The effect of noise on quantum systems

---

## 🎯 Objectives

* Implement classical linear search for baseline comparison
* Build Grover’s Algorithm using Qiskit
* Compare classical vs quantum search complexity
* Simulate quantum noise and analyze its impact
* Visualize results using histograms and plots

---

## 🛠️ Tech Stack

* **Programming Language**: Python
* **Quantum Framework**: Qiskit
* **Simulation**: Qiskit Aer Simulator
* **Visualization**: Matplotlib, Qiskit Visualization
* **Other Libraries**: NumPy

---

## 📂 Project Structure

```id="k9q3xp"
grovers-algorithm/
│
├── notebook/
│   └── grovers_algorithm.ipynb
│
├── results/
│   └── figures/       
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Problem Setup

* **Search Space**: 2 qubits → 4 possible states

  ```
  00, 01, 10, 11
  ```
* **Target State**: `"10"`

### 🔍 Complexity Comparison:

* Classical Search: **O(N)**
* Quantum Search (Grover): **O(√N)**

---

## 🔍 Classical Search

A simple **linear search algorithm** is implemented:

* Iterates through all elements
* Checks each item sequentially
* Stops when the target is found

### 📊 Result:

* Steps taken: **3**
* Time: ~0.0002 sec

---

## ⚛️ Quantum Implementation (Grover’s Algorithm)

The quantum solution consists of the following steps:

### 1. Superposition

* Apply Hadamard gates
* Creates equal probability of all states

### 2. Oracle

* Marks the target state (`"10"`)
* Applies phase flip to correct solution

### 3. Diffusion Operator

* Amplifies probability of target state
* Reduces probability of other states

### 4. Measurement

* Converts quantum state to classical output

---

## 📊 Results

### 🔹 Ideal Quantum Output

* Target state `"10"` appears with **100% probability**

### 🔹 Noisy Quantum Output

Example result:

```
{'10': 534, '00': 194, '11': 183, '01': 113}
```

### 🔹 Observations:

* Target state still dominant
* Noise introduces errors and uncertainty

---

## ⚖️ Classical vs Quantum Comparison

| Metric         | Classical Search | Quantum Search      |
| -------------- | ---------------- | ------------------- |
| Complexity     | O(N)             | O(√N)               |
| Steps (N=4)    | 3                | ~2                  |
| Execution Time | Very Fast        | Slower (simulation) |
| Accuracy       | Exact            | Affected by noise   |

---

## 🔊 Noise Simulation

A **depolarizing noise model (10%)** is applied to simulate real quantum hardware conditions.

### 🔹 Noise Effects:

* Reduces probability of correct result
* Introduces incorrect states
* Demonstrates limitations of current quantum systems

---

## 📈 Visualizations

The project includes:

* Step comparison bar chart (Classical vs Quantum)
* Histogram comparison:

  * Ideal results
  * Noisy results

These visualizations clearly illustrate:

* Quantum advantage in theory
* Practical limitations due to noise

---

## ▶️ How to Run

### 1. Clone the repository

```bash id="4r6znt"
git clone https://github.com/BatoolJohn/Quantum-Computaing_ML.git
cd Project 2: Grover's algorithm implementation
```

### 2. Install dependencies

```bash id="d9v3pa"
pip install -r requirements.txt
```

### 3. Run the notebook

```bash id="r2n8xs"
jupyter notebook notebook/Project 2: Grover's algorithm implementation.ipynb
```

---

## 🚧 Future Improvements

* Extend to more qubits (larger search space)
* Optimize oracle construction
* Implement multiple target states
* Run on real quantum hardware
* Apply error mitigation techniques

---

## 💡 Why This Project Matters

This project demonstrates:

* Strong understanding of **quantum algorithms (Grover’s Algorithm)**
* Ability to compare **classical vs quantum computation**
* Knowledge of **quantum noise and its impact**
* Practical experience using **Qiskit and quantum simulations**

---

## 🧠 Conclusion

Grover’s Algorithm demonstrates a clear **theoretical advantage** over classical search by reducing complexity from **O(N) to O(√N)**.

However, this project also highlights key challenges:

* Quantum simulations are computationally expensive
* Noise significantly affects accuracy
* Current hardware limitations restrict real-world performance

👉 While quantum computing shows strong potential, **practical advantages are still limited by noise and hardware constraints**.

---

## 📜 License

This project is licensed under the Apache-2.0 License.

---

## 📬 Contact

**Attiya Batool**

* LinkedIn: https://linkedin.com/in/your-profile
* Email: batooljohn@gmail.com

---

⭐ If you found this project useful, consider giving it a star!
