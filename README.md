PyTorch Multi-GPU Example
This repository contains a Python script demonstrating the use of PyTorch for creating a simple neural network that leverages multiple GPUs for parallel computation, if available. The example includes creating a custom dataset, defining a model, and configuring the model to run on multiple GPUs using nn.DataParallel.

Features
Custom Dataset Generation: Uses a Dataset subclass to generate a dataset of random numbers.
Simple Neural Network Model: Defines a simple linear model with PyTorch's neural network module (nn.Module).
Multi-GPU Support: Demonstrates how to use nn.DataParallel to parallelize model computations across multiple GPUs.
Dynamic Device Usage: Automatically uses CUDA if GPUs are available, and falls back to CPU otherwise.
Requirements
Python 3.x
PyTorch 1.x (The script was tested on PyTorch 1.8.1, but it should be compatible with other versions. Adjust as necessary for newer versions.)
Setup
Install Python: Ensure Python 3.x is installed on your system. You can download it from python.org.

Install PyTorch: Follow the installation instructions on the official PyTorch website to install PyTorch. Make sure to select the CUDA version compatible with your system if you wish to use GPUs.

Running the Script
To run the script, simply execute it with Python from your terminal or command prompt:

sh
Copy code
python multi_gpu_example.py
Ensure you are in the directory containing the script before running the above command.

Output
When running the script, it will print the size of the input and output for each batch processed by the model. If multiple GPUs are available and detected, it will also print a message indicating the number of GPUs being used.

Note
The script is a basic demonstration meant for educational purposes and may need modifications for use in production environments.
For systems with a single GPU or only CPU, the script will automatically adjust, thanks to PyTorch's dynamic device management.
License
This project is open-sourced under the MIT license. See the LICENSE file for more details.
