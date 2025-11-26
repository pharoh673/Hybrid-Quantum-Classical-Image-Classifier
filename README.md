# Hybrid-Quantum-Classical-Image-Classifier
A deep learning + quantum neural network system capable of recognizing animals, clothing, EMNIST letters, KMNIST kana, and handwritten digits — with an interactive image upload tool.

📌 Overview

This project implements a hybrid Quantum Machine Learning (QML) architecture that combines:

ResNet-based deep CNN feature extraction

A classical fully connected branch

A multi-qubit quantum variational circuit (QNN)

A final fused classifier that learns jointly from both worlds

The model reaches strong performance across several datasets and tasks:

🐶 Animal image classification (with Grad-CAM visual explanations)

👚 Fashion-MNIST 10-class image recognition

✉️ EMNIST Letters classification (26 classes)

🈁 KMNIST (Japanese kana) recognition + example word reconstruction

🔢 10-digit sequence (phone number) classification using hybrid and classical models

It also includes a Jupyter-based interactive tool where users can upload their own image, run live inference, and visualize Grad-CAM heatmaps.

✨ Key Features

Hybrid Deep Learning + QNN pipeline (PyTorch + TorchQuantum)

Custom 8-qubit quantum circuit layer

Dual-branch architecture (classical + quantum fused)

Grad-CAM visualization for explainable AI

Confusion matrices + misclassification grids

Support for multiple datasets (Animals, Fashion-MNIST, EMNIST, KMNIST, MNIST digits)

Phone number multi-digit inference framework

Upload-your-own-image inference widget

📂 Contents

hybrid_qml_final.ipynb — Full training, evaluation, and visualization notebook

hybrid_dual_resnet_qnn.pth — Trained model weights

img_upload_classifier — Interactive inference UI (inside the notebook)

🧠 Why Hybrid Quantum ML?

This project demonstrates that quantum layers can complement deep neural networks, even on real image data.
The QNN branch learns compact but expressive transformations that enhance classification accuracy across datasets.

Even on CPU-only systems, the quantum simulation remains efficient and practical.

▶️ Live Demo (Inside the Notebook)

After opening the notebook, scroll to the bottom to find the Upload Image & Classify section:

Upload any photo (animal dataset works best)

Get the model prediction

See a top-probs bar chart

Inspect the Grad-CAM heatmap showing where the model focused

🏁 Results Summary (High-Level)
Dataset	Best Accuracy	Notes
Animals	~85%	Hybrid QNN significantly boosts confidence + explainability
Fashion-MNIST	~90%	Stable hybrid performance
EMNIST Letters	92%	QNN handles 26-class handwriting well
KMNIST	~90%	Tested on real Japanese words
Phone Number Recognition	Perfect sequence predictions	Works with classical, deep, and hybrid modes
