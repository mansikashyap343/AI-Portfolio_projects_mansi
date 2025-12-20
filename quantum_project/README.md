**Quantum Biomarker Classification using Variational Quantum Circuits**

This project implelments a hybrid quantum-classical machine learning model to classify synthetic health biomarkers using Qiskit's Variational Quantum Classifier(VQC).

The model predicts whether an individual is healthy or diseased based on two features:

Oxygen saturation (SpO₂)

Heart Rate Variability (HRV)

**Project Overview**

The project demonstrates a complete Quantum Machine Learning (QML) workflow, including:

Synthetic biomedical data generation

Quantum feature encoding

Variational circuit design

Hybrid optimization and training

Model evaluation

**How It Works**
Data Generation

Synthetic health data is generated to simulate medical conditions:

Healthy Group

SpO₂: 0.7 – 1.0

HRV: 0.6 – 1.0

Diseased Group

SpO₂: 0.3 – 0.6

HRV: 0.2 – 0.5

Quantum Model

Number of qubits: 2

Feature Map: ZFeatureMap(2)

Variational Ansatz: RealAmplitudes(2)

Optimizer: COBYLA

Classifier: Qiskit VQC

**Results**

The Variational Quantum Classifier successfully learns a clear separation between the synthetic biomarker classes. Training converges reliably with a stable loss value, demonstrating the feasibility of quantum approaches for medical classification tasks.

**Tech Stack**

Python

NumPy / Pandas

scikit-learn

Qiskit

**How to Run**
pip install -r requirements.txt


Open and run:

quantum.ipynb

**Files**

quantum.ipynb — Main notebook

requirements.txt — Dependencies

assets/ — Visuals and results
