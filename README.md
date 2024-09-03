# Quantum Machine Learning with the Iris Dataset

This project explores the application of Quantum Machine Learning (QML) techniques, specifically using Variational Quantum Circuits (VQC), to classify the famous Iris dataset. The project also compares the performance of the VQC model with a classical Logistic Regression model.

## Table of Contents
- [Installation](#installation)
- [Project Overview](#project-overview)
- [Data Preprocessing](#data-preprocessing)
- [Quantum Model](#quantum-model)
  - [Feature Map](#feature-map)
  - [Ansatz](#ansatz)
  - [Optimizer](#optimizer)
  - [Training and Evaluation](#training-and-evaluation)
- [Classical Model](#classical-model)
- [Results](#results)
- [Conclusion](#conclusion)

## Installation

To run this project, you need to install the following dependencies:

```bash
pip install qiskit
pip install pylatexenc
pip install azure-quantum[qiskit]
pip install qiskit_machine_learning
pip install pennylane
pip install pennylane-sf --upgrade
```
## Project Overview
The Iris dataset is one of the most well-known datasets in the pattern recognition literature. It consists of 150 samples with 4 features each, representing the dimensions of iris flowers. The goal is to classify the samples into one of three classes: Iris-Setosa, Iris-Versicolour, or Iris-Virginica.

This project uses both classical and quantum machine learning approaches to classify the Iris dataset and compares their performances.

## Data Preprocessing
The data is normalized to bring all features within the range [0, 1]. This is important for quantum circuits, which are sensitive to the scale of input data.

## Quantum Model
## Feature Map
A feature map is used to encode classical data into a quantum state. In this project, the ZZFeatureMap from Qiskit is used.

## Ansatz
An ansatz is a parameterized quantum circuit used to find the optimal quantum state that represents the solution. The RealAmplitudes ansatz is used in this project.

## Optimizer
The COBYLA optimizer is used to optimize the parameters of the quantum circuit.

## Training and Evaluation
The VQC model is trained using a quantum simulator. The performance is evaluated on the test set using metrics like accuracy, precision, recall, and F1 score.

## Classical Model
A classical Logistic Regression model is also trained and evaluated on the same dataset for comparison.

## Results
The performance of the VQC model is compared to the classical Logistic Regression model. The results are visualized using a bar chart.

## Conclusion
While the classical Logistic Regression model outperformed the VQC model on this specific dataset, the project demonstrates the potential of quantum machine learning. As quantum hardware and algorithms improve, quantum models may become more competitive in practical applications.
