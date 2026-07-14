# Optimization Algorithms from Scratch

An educational implementation of popular gradient-based optimization algorithms using NumPy.

This repository explores how optimization algorithms work internally by implementing their update rules from scratch and applying them to linear regression. It includes experiments, visualizations, and diagnostics for understanding how different optimizers affect convergence and parameter updates.

> **Note:** This project was created for learning and educational purposes. It is not intended to present novel algorithms, original research contributions, or production-ready optimizer implementations.

## Overview

Optimization algorithms are a fundamental part of machine learning and deep learning. Although modern frameworks provide efficient built-in optimizers, implementing them from scratch can help develop a deeper understanding of:

* How gradients are used to update model parameters
* How learning rates affect convergence
* Why momentum can accelerate optimization
* How adaptive learning-rate methods work
* How optimizer state evolves during training
* Why bias correction is used in Adam
* How AdamW differs from standard Adam with L2 regularization
* How learning-rate scheduling and gradient clipping influence training

The implementations in this repository prioritize clarity and learning over performance or production use.

## Implemented Optimizers

The notebook covers the following optimization algorithms:

* Batch Gradient Descent
* Mini-Batch Stochastic Gradient Descent (SGD)
* SGD with Momentum
* Nesterov Accelerated Gradient
* AdaGrad
* RMSProp
* Adam
* AdamW

Additional optimization techniques include:

* Learning-rate scheduling
* Gradient clipping by value
* Gradient clipping by global norm

## Features

* NumPy-based implementations
* Linear regression experiments
* Mean Squared Error (MSE) loss
* Analytical gradient computation
* Numerical gradient checking
* Reusable optimizer abstractions
* Training and validation loss tracking
* Gradient-norm monitoring
* Parameter and update trajectory analysis
* Effective learning-rate analysis
* Optimizer convergence comparisons
* Visualizations of optimization behavior

## Repository Structure

```text
optimization-algorithms-from-scratch/
├── Optimisation_Implementation.ipynb
├── README.md
└── LICENSE
```

## Learning Objectives

This project aims to build an intuitive and implementation-level understanding of optimization algorithms.

By working through the notebook, you can explore questions such as:

* How does gradient descent minimize a loss function?
* What is the difference between batch and mini-batch optimization?
* How does momentum smooth parameter updates?
* Why does Nesterov momentum evaluate gradients at look-ahead parameters?
* How do AdaGrad and RMSProp adapt learning rates for individual parameters?
* How do Adam's first- and second-moment estimates affect optimization?
* Why is bias correction needed during Adam's early updates?
* How does AdamW decouple weight decay from gradient-based optimization?
* How do learning-rate schedules affect convergence?
* How can gradient clipping improve optimization stability?

## Requirements

The notebook uses standard Python libraries for numerical computation and visualization.

```bash
pip install numpy matplotlib
```

A Jupyter environment is also required:

```bash
pip install jupyter
```

Alternatively, the notebook can be opened in Google Colab.

## Usage

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/optimization-algorithms-from-scratch.git
cd optimization-algorithms-from-scratch
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
Optimisation_Implementation.ipynb
```

Run the notebook cells in order to reproduce the implementations, experiments, and visualizations.

## Educational Scope

The implementations are intentionally written to expose the internal mechanics of each optimizer.

They are not intended to replace optimized implementations available in machine-learning frameworks such as PyTorch, TensorFlow, or JAX. Production frameworks include additional considerations such as computational efficiency, numerical stability, hardware acceleration, distributed training, and extensive testing.

This repository should therefore be viewed as a learning resource and implementation exercise rather than a research contribution or production optimization library.

## Disclaimer

This project does not claim:

* Novel optimization algorithms
* Original theoretical contributions
* New research findings
* State-of-the-art performance
* Production-ready implementations

The algorithms implemented here are established methods from the machine-learning literature. The purpose of the repository is to study, implement, visualize, and better understand their behavior.

## License

This project is available under the MIT License.
