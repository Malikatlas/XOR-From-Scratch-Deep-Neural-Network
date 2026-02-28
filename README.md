# Solving XOR with a Deep Neural Network 

Implementation of a Deep Neural Network (DNN) from scratch in NumPy to solve the classic XOR problem.

---

## 🧠 Problem Overview

The XOR function is not linearly separable.  
A single-layer perceptron cannot solve it.

This project demonstrates how adding a hidden layer with non-linear activation enables a neural network to learn a non-linear decision boundary.

---

## 📐 Architecture

- Input Layer: 2 neurons (binary inputs)
- Hidden Layer: 4 neurons (tanh activation)
- Output Layer: 1 neuron (sigmoid activation)
- Loss Function: Binary Cross-Entropy
- Optimizer: Gradient Descent (implemented manually)
- Learning Rate: 0.1
- Epochs: Up to 20,000 (early stopping enabled)

---

## 📊 Training Results

- Converged in: 59 epochs
- Final Loss: 0.603267
- Predictions:

| Input | Output |
|-------|--------|
| (0,0) | 0 |
| (0,1) | 1 |
| (1,0) | 1 |
| (1,1) | 0 |

The model successfully learned the XOR mapping.

---

## 🔍 Why XOR Requires Non-Linearity

The XOR dataset cannot be separated using a single linear boundary.

Points (0,1) and (1,0) lie diagonally, making the problem non-linearly separable.

By introducing a hidden layer with a non-linear activation (tanh), the network combines multiple linear regions to form a non-linear decision boundary.

---

## 📈 Training Curve

The Binary Cross-Entropy loss decreases smoothly until convergence, demonstrating stable gradient descent optimization.

---

## 📂 Repository Structure

```
XOR-From-Scratch-Deep-Neural-Network/
│
├── XOR_Assignment_Notebook_Atlas_Malik_DL.ipynb
├── Solving XOR with Deep NN.pdf
├── README.md
└── LICENSE
```

---

## 🛠 Tech Stack

- Python
- NumPy
- Matplotlib

---

## 🎯 Key Learning Outcomes

✔ Understanding linear vs non-linear separability  
✔ Manual forward & backward propagation  
✔ Implementing BCE loss  
✔ Gradient descent from scratch  
✔ Importance of hidden layers  

---

## 📜 License

MIT License

---

## ⚠ Disclaimer

This project was developed for academic purposes to demonstrate core deep learning fundamentals.
