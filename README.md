# GPT from Scratch (Tiny Shakespeare)

## Goal
This project implements a GPT-style Transformer model from scratch using PyTorch and trains it on the Tiny Shakespeare dataset using backpropagation.

## Architecture
The model follows the GPT architecture and includes:
- Character-level token embeddings
- Learned positional embeddings
- Multi-head causal self-attention
- Feed-forward layers
- Residual connections
- Layer normalization
- Causal (autoregressive) masking

## Training Method
- Loss function: Cross-Entropy Loss
- Optimization: AdamW optimizer
- Training is performed using backpropagation via automatic differentiation.
- Gradients are computed using `loss.backward()` and parameters are updated using `optimizer.step()`.

## Dataset
- Tiny Shakespeare dataset
- Automatically downloaded from Karpathy’s repository

## Results
The training loss decreases over time.
After training, the model is able to generate Shakespeare-like character-level text.

## How to Run
1. Open the Jupyter notebook
2. Run all cells from top to bottom
3. The dataset will be downloaded automatically
4. Training will start and loss will be printed
