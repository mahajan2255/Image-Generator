# 🎨 Simple Generative Model with PyTorch

This project demonstrates a basic **generative neural network** built using **PyTorch**, which learns to produce data points that mimic a target distribution. Instead of using a standard dataset like MNIST, the model trains on a **synthetically generated dataset** — typically 2D points sampled from a Gaussian or similar distribution.

## 🧠 How It Works

The core of the model is a **feedforward neural network (Generator)**. It takes in random noise as input and learns to generate outputs that resemble the target distribution. The network consists of fully connected layers with **ReLU** activations and a final **Tanh** layer to keep outputs bounded.

Training is performed using **Mean Squared Error (MSE)** between the generated points and the true synthetic data. The network is optimized using **Adam**, gradually improving its ability to produce structured, meaningful outputs from noise.

## 🌀 Visualization

The notebook visualizes the output of the generator during training. Initially, generated samples appear random and unstructured. Over time, they begin to mirror the original synthetic data distribution — showing the model has learned to generate coherent patterns.

## 📦 Requirements

Install the required libraries with:

```bash
pip install torch numpy matplotlib
