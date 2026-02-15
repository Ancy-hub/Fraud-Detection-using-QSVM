# Fraud Detection using QSVM (Quantum Support Vector Machine)

This project is an exploratory implementation of a **Quantum Support Vector Machine (QSVM)** applied to a fraud detection use case in the financial payments domain.
The primary goal of this work was to **learn and experiment with quantum machine learning** concepts and understand how quantum kernels can be used for real-world classification problems.

Rather than building a production fraud system, this project focuses on:

* Understanding quantum feature maps
* Implementing QSVM end-to-end
* Comparing classical vs quantum intuition
* Exploring the **Cirq + Google Colab** quantum software stack

---

## Motivation

I built this project as part of my journey into **quantum computing and quantum machine learning**.
I wanted a hands-on way to move beyond theory and actually:

* Encode classical financial data into quantum states
* Construct a quantum kernel
* Train a QSVM for binary classification (fraud vs non-fraud)
* Run simulations using Cirq

This repository represents my **learning experiment in quantum ML**, not a production-ready fraud detection system.

---

## What is QSVM?

A **Quantum Support Vector Machine** uses a **quantum kernel** to map classical data into a high-dimensional Hilbert space using a quantum feature map.
The intuition is similar to classical SVM, but the kernel is computed using quantum circuits, which may offer advantages for certain complex data distributions.

Workflow used in this project:

1. Preprocess financial transaction data
2. Encode features into a quantum feature map
3. Generate a quantum kernel matrix using Cirq simulation
4. Train an SVM classifier using the quantum kernel
5. Evaluate classification performance

---

## Tech Stack

* **Python**
* **Cirq** – quantum circuit simulation
* **Google Colab** – experimentation environment
* **NumPy / Pandas** – data handling
* **Scikit-learn** – SVM training and evaluation

---

## Problem Statement

Binary classification of transactions:

* `0` → Legitimate transaction
* `1` → Fraudulent transaction

Due to quantum simulation limits, a **reduced feature set** was used so the data could be encoded into a small number of qubits.

---

## Implementation Steps

* Data preprocessing and normalization
* Dimensionality reduction for qubit compatibility
* Quantum feature map construction
* Quantum kernel computation using Cirq simulator
* Training classical SVM with quantum kernel
* Model evaluation (accuracy, confusion matrix)

---

## Results

This project demonstrates:

* A working **end-to-end QSVM pipeline**
* Successful classification using a quantum kernel (simulated)
* Practical understanding of quantum data encoding challenges

Performance is **not meant to beat classical models**, since the goal was learning and experimentation with quantum workflows.

---

## Key Learnings

* How classical data is embedded into quantum states
* Limitations of current quantum simulators (qubit count, runtime)
* Differences between classical kernels and quantum kernels
* Practical workflow for quantum ML experiments

---

## 📌 Note

This project is part of my **quantum computing learning journey** and serves as a hands-on exploration of QSVM rather than a production fraud detection solution.

---
