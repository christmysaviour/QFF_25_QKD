# 🔐 Quantum Key Distribution - BB84 & B92  
### Qiskit Fall Fest 25 Hackathon Project | Implemented using Qiskit  
_Notebooks: `BB84_hackathon.ipynb`, `b92.ipynb`_

---

## 🧠 Abstract  
This project implements **end-to-end Quantum Key Distribution (QKD)** protocols — **BB84** and **B92** — using **Qiskit**, demonstrating secure quantum key exchange leveraging the principles of quantum mechanics.

The implementation simulates:
- **Qubit preparation, transmission, and measurement**
- **Basis reconciliation (sifting)**
- **Error rate estimation (QBER)**
- **Detection of eavesdropping (Eve attack simulation)**
- **Comparison of BB84 and B92 performance** under varying noise conditions.

By comparing both protocols, we analyze trade-offs in **security**, **efficiency**, and **noise tolerance**, offering insight into the practical feasibility of QKD on today’s quantum simulators.

---

## ⚙️ Implementation Details

### 🧩 1. BB84 Protocol
- Implements random **basis selection (Z/X)** for encoding qubits.  
- Models **quantum channel noise** using Qiskit’s **depolarizing noise model**.  
- Includes **intercept-resend Eve simulation** to observe induced QBER.  
- Performs **sifting** to extract shared keys where bases align.  
- Computes **Quantum Bit Error Rate (QBER)** to evaluate protocol integrity.

### 🪩 2. B92 Protocol
- Implements a simplified **two-nonorthogonal-state QKD** scheme.  
- Simulates **probabilistic conclusive measurements** and sifting process.  
- Measures QBER and key generation efficiency under different noise levels.  
- Enables direct comparison with BB84 to study **noise resilience** and **key rate**.
- 
---

## 🧪 Results & Plots
- **QBER vs Noise Probability:**  
  Shows how error rate increases with depolarizing noise and eavesdropping.  
- **Sifted Key Rate Comparison:**  
  Demonstrates that BB84 maintains a higher usable key fraction than B92.

*(Refer to the notebook outputs for detailed plots and numerical results.)*

---

## 🧰 Tools & Libraries
- [Qiskit](https://qiskit.org/) — Quantum circuit simulation  
- [NumPy](https://numpy.org/) — Numerical computations  
- [Matplotlib](https://matplotlib.org/) — Data visualization  

---

## 🧑‍💻 Contributors
**Team QFF Hackathon — Quantum Key Distribution**
- Implemented by students of *Quantum Technology, IISc Bangalore*
- Developed during the **RPI Quantum Future Hackathon (QFF)**

---

## 📈 Future Work
- Integrate **error correction** (Cascade protocol) and **privacy amplification** stages.  
- Implement **explicit POVM-based measurement** for B92 (unambiguous state discrimination).  
- Run on **real IBM Quantum backends** to test under physical noise models.  
- Extend to **E91 (Entanglement-based QKD)** and **continuous-variable QKD** schemes.

---

## 📜 License
This project is released under the **MIT License**.  
Feel free to use, modify, and share with attribution.

---

> _“Quantum cryptography is not about stronger math — it’s about physics that refuses to be copied.”_
