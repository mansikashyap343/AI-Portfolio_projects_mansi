 Quantum Biomarker Classifier

A hybrid quantum–classical machine learning model to classify synthetic health biomarkers (oxygen saturation & HRV).

Details

This project demonstrates how quantum circuits can be used for binary medical classification.
Using Qiskit’s Variational Quantum Classifier (VQC), it predicts whether a person is healthy or diseased based on two features:

Oxygen saturation (SpO₂)

Heart Rate Variability (HRV)

The project simulates a complete QML workflow:

Generate synthetic health data

Prepare a quantum feature map

Build a variational ansatz

Train with COBYLA optimizer

Evaluate performance on test split

Tech Stack

Python

NumPy / Pandas

scikit-learn

Qiskit

ZFeatureMap

RealAmplitudes

Sampler

VQC

Files Included
File	Description
quantum.ipynb	Main notebook containing data generation, model building & training
requirements.txt	All necessary dependencies
assets/	Screenshots, small example images, or result illustrations
 How to Run
1. Install dependencies
pip install -r requirements.txt

2. Run the notebook (Jupyter/Colab)

You can open it in Colab instantly:
File → Open Notebook → Upload

 How It Works
 1. Data

Synthetic data is generated to simulate health conditions.
Healthy group:

O₂: 0.7–1.0

HRV: 0.6–1.0

Diseased group:

O₂: 0.3–0.6

HRV: 0.2–0.5

 2. Quantum Model

2 qubits

ZFeatureMap(2) to encode two features

RealAmplitudes(2) as trainable circuit

COBYLA optimizer

The classifier is trained using Qiskit’s VQC.

Results

The VQC typically learns clear separation between the synthetic biomarker classes.
Training ends successfully with a converged loss value.

 Author

Mansi — AI/ML student building hybrid quantum-AI systems.
