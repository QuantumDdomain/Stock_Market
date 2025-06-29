# 🧠 Quantum Stock Market Analysis and Prediction

This project explores quantum machine learning and quantum optimization techniques for stock market applications using **Qiskit**. It consists of two main modules:

1. **Stock Prediction with Contextual Quantum Neural Network**  
2. **Portfolio Risk Analysis with QAOA and QUBO Modeling**

---

## 📁 Project Structure

- `QSTL.ipynb` – Implements a Contextual Quantum Neural Network (CQNN) for sequential stock return prediction.
- `QAOA_portfolio_optimization.ipynb` – Performs portfolio optimization using QUBO encoding and solves it via QAOA.

---

## 🧠 1. Stock Prediction using Contextual QNN (`QSTL.ipynb`)

This notebook implements a **Contextual Quantum Neural Network (CQNN)** for predicting future stock returns based on a historical sequence of prices.

### 🔬 Key Features

- **Contextual State Encoding:** Encodes a time window of past stock prices into qubits using a hardware-efficient ansatz.
- **Parameterized Quantum Circuit (PQC):** Applies a learnable PQC to predict the next time step.
- **Swap Test and Fidelity Loss:** Uses quantum state overlap as a fidelity-based loss function to evaluate predictions.
- **Training:** Optimized using **SPSA** (Simultaneous Perturbation Stochastic Approximation).
- **Evaluation:** Prediction accuracy is quantified using **KL Divergence** and **fidelity scores**.

### 📈 Data Used

- Historical price data of **GOOG** or other chosen assets.
- Preprocessed and encoded into quantum states for sequential modeling.

---

## 📊 2. Portfolio Optimization using QAOA (`QAOA_portfolio_optimization.ipynb`)

This module formulates a **quantum risk analysis and portfolio optimization** task as a **QUBO** problem and solves it using the **Quantum Approximate Optimization Algorithm (QAOA)**.

### 🧩 Key Features

- **QUBO Formulation:** Encodes risk-return trade-off in a quadratic binary model.
- **Quantum Circuit:** Constructs QAOA circuit using cost and mixer Hamiltonians.
- **Expectation Evaluation:** Measures and optimizes the QAOA energy landscape to select optimal portfolio assets.

---

## 🚀 Technologies Used

- **Qiskit** (QAOA, QNN, Optimization, Aer)
- **Python (NumPy, Matplotlib, Pandas)**
- **Jupyter Notebooks**

---

## 🛠 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/QuantumDdomain/Stock_Market.git
   cd Stock_Market
