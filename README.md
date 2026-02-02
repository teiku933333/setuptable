# Fetch Setup Table Policy

This repository contains a neural network policy for the Fetch robot
to perform the "setup the table" task.

## Model
- Framework: PyTorch
- Input: observation vector of shape (30,)
- Output: action vector of shape (13,)
- Output range: [-1, 1] (normalized)

## Architecture
- MLP with 3 hidden layers
- Hidden size: 256
- Activation: ReLU
- Output activation: Tanh

## Files
- model.py: model definition
- model.pt: PyTorch weights
- model.onnx: exported ONNX model
- config.json: model metadata
- requirements.txt: dependencies

## Testing
- PyTorch forward pass tested
- ONNX runtime inference tested

This repository provides a standalone inference model.
No simulator or environment is included.
