# Neural Network From Scratch in PyTorch

### DS 593 Portfolio Piece 1

------------------------------------------------------------------------

## Overview

This project builds a simple **Multi-Layer Perceptron (MLP)** neural
network from scratch using **PyTorch** and evaluates how different
architectural and training choices affect model performance.

The goal is to understand how neural networks learn through **gradient
descent** and how changes to:

-   Number of layers
-   Activation functions
-   Learning rate
-   Training dataset size

impact convergence and generalization.

------------------------------------------------------------------------

## Conceptual Understanding

Neural networks learn by minimizing a **loss function** using gradient
descent.
At each step, model weights are updated based on prediction error.

In this project, I varied: 
- Model depth
- Activation functions
- Learning rate

to observe how these design choices affect training dynamics and
performance, as discussed in class.

------------------------------------------------------------------------

## Datasets 

-   **XOR Dataset** -- demonstrates the need for non-linear models
-   **Digits Dataset (scikit-learn)** -- 8×8 handwritten digit
    classification (0--9)

------------------------------------------------------------------------

## Experiments

-   Effect of network depth (1--3 hidden layers)
-   Activation function comparison (ReLU, Sigmoid, Tanh)
-   Learning rate tuning
-   Impact of training set size

------------------------------------------------------------------------

## Evaluation

Model performance was evaluated using:

-   Training loss curves
-   Test accuracy
-   Confusion matrix

Loss curves help visualize whether gradient descent is successfully
minimizing the loss over time.

------------------------------------------------------------------------

## Key Findings

-   XOR requires hidden layers to solve\
-   ReLU converges faster than Sigmoid/Tanh\
-   Learning rate strongly affects stability\
-   Larger datasets improve generalization

------------------------------------------------------------------------

## How to Run

1.  Clone the repo:

``` bash
git clone https://github.com/bu-cds-llms/portfolio-piece-1-riya-rb
cd portfolio-piece-1-riya-rb
```

2.  Install dependencies:

``` bash
pip install torch scikit-learn matplotlib numpy
```

3.  Run:

``` bash
jupyter notebook
```

Open and run:

    portfolio_neural_net_pytorch.ipynb

------------------------------------------------------------------------

## Requirements

-   Python 3.8+
-   PyTorch
-   NumPy
-   Matplotlib
-   scikit-learn

------------------------------------------------------------------------

## Structure

    PORTFOLIO-PIECE-1-RIYA-RB/
    ├── README.md
    ├── notebooks/
    │   └── portfolio_neural_net_pytorch.ipynb
    └── requirements.txt
