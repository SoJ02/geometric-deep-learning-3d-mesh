# Geometric Deep Learning for 3D Mesh Classification

This repository contains a multi-experiment workflow for **3D mesh classification** using deep learning.  
It focuses on practical model training behavior, optimization dynamics, and iterative architecture-level refinement.

## Problem Statement

Unlike 2D images, 3D meshes encode non-Euclidean geometric structure.  
The goal is to classify mesh objects by learning shape-aware features that remain robust under variation in geometry and representation.

## What this project demonstrates

- mesh-oriented preprocessing and data handling,
- supervised training loops for geometric models,
- epoch-by-epoch evaluation tracking,
- convergence diagnostics and iterative refinement.

## Experiment Design

The work is organized as four experiment notebooks, each extending or validating a different part of the modeling pipeline:

- `mesh-classification-experiment-1.ipynb`
- `mesh-classification-experiment-2.ipynb`
- `mesh-classification-experiment-3.ipynb`
- `mesh-classification-experiment-4.ipynb`

Supporting implementation notes are captured in `*_modified.py.txt` files.

## Tech Stack

- Python
- PyTorch
- Jupyter
- NumPy / Matplotlib for analysis and visualization

## Environment Setup

```bash
python -m venv venv
venv\Scripts\activate
pip install torch torchvision numpy matplotlib jupyter
jupyter lab
```

## How to Run

1. Prepare the mesh dataset expected by the notebooks.
2. Launch Jupyter.
3. Run notebooks in sequence to follow experiment progression.
4. Inspect training logs, checkpoint behavior, and accuracy trends.

## Results and Observations

Logged runs show clear convergence patterns:

- Early epochs begin with low-to-mid performance (for example near `50%` test accuracy).
- Performance rises significantly through training progression.
- One tracked sequence reaches and sustains `100%` test accuracy in later epochs.

This indicates strong learnability for the evaluated setup, while also highlighting the importance of training duration and configuration.

## Repository Contents

- experiment notebooks (`mesh-classification-experiment-*.ipynb`)
- architecture/training change notes (`*_modified.py.txt`)
- summary artifact: `mesh-classification-report.pdf`

## Practical Next Steps

- validate on larger and more diverse mesh benchmarks,
- add cross-validation and robustness checks,
- test augmentation strategies and regularization,
- package final inference path as reproducible script/API.
