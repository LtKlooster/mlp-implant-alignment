# mlp-implant-alignment
A demo for how to use (multi-task) MLPs for estimating implant alignment in total knee arthroplasty.

## Introduction
This repository demonstrates how to train a simple **Multi-Layer Perceptron (MLP)** and **multi-task MLP** for estimating implant alignment quality in total knee arthroplasty. 
For more details, please see our paper:
\todo (insert citation)

The notebooks included are designed as an example to show how the model and data pipeline work for a synthetic dataset.

## Dataset Overview

The provided dataset (`dummy_data.csv`) contains:
- **Input features:**  
  - `Fem_Fle(+)Ext(-)`  
  - `Fem_Var(+)Val(-)`  
  - `Fem_Int(+)Ext(-)`  
- **Target outputs:**  
  - `EI`, `VV`, `LM`, `AP`, `PD`, `PCL`, `dMCL`, `sMCL`, `LCL`, `ALL`, `OPL`, `PC`  
- **Aggregated output:**  
  - `f` (weighted sum of kinematics + ligaments)

All data values are synthetic and randomly generated for demonstration purposes.

## Dependencies

This project requires the following Python packages:

- torch
- pandas
- numpy
- scikit-learn
- matplotlib (optional, for plotting)
- jupyter

You can install them using:

```bash
pip install -r requirements.txt
