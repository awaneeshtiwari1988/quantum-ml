# Quantum Machine Learning

Building from quantum computing fundamentals toward hybrid quantum-classical machine learning — run as an independent track alongside classical deep learning, with explicit, documented points where the two intersect.

Part of an MTech specialization (BITS Pilani) in Quantum Machine Learning, extended through independent study using Qiskit and PennyLane.

---

## Planned notebooks (in build order)

### Fundamentals
- [ ] **Deutsch-Jozsa algorithm** — implementation in Qiskit with circuit diagrams and intuition write-up
- [ ] **Grover's search algorithm** — implementation and complexity discussion
- [ ] **Basic circuit playground** — gates, superposition, entanglement, measurement, worked examples

### Quantum Machine Learning
- [ ] **Variational Quantum Classifier (VQC) vs classical baseline** — the flagship project: a VQC benchmarked rigorously against a classical neural network of comparable parameter count, on a real (not toy) classification task, with honest analysis of where and why quantum helps or doesn't (dataset size, noise, barren plateaus)
- [ ] **Quantum GAN vs classical GAN** — benchmarking a small QGAN against a classical GAN on a toy distribution
- [ ] **Hybrid quantum-classical optimization** — using classical optimizers (Adam) to train a VQE/QAOA ansatz, documented as an explicit fusion point with classical deep learning optimization

## Explicit fusion points with classical DL

This repo deliberately documents where quantum and classical methods meet, rather than blending them without explanation:

| Quantum concept | Classical DL concept | Where it's explored |
|---|---|---|
| Variational Quantum Circuit | Feedforward NN layer | VQC vs classical baseline notebook |
| Parameter-shift rule | Backpropagation | Gradient comparison writeup |
| QAOA / VQE | SGD/Adam, non-convex optimization | Hybrid optimization notebook |
| Barren plateaus | Vanishing gradients | Comparative failure-modes note |

## Stack

Qiskit, PennyLane, Python, NumPy

## Status

🚧 Fundamentals phase — starting with Deutsch-Jozsa and Grover's algorithm before moving into QML.

---

*Part of a three-lane portfolio — see [ml-dl-research](https://github.com/awaneeshtiwari1988/ml-dl-research) for classical DL/NLP/RL work, and [ml-systems-engineering](https://github.com/awaneeshtiwari1988/ml-systems-engineering) for production ML systems.*
