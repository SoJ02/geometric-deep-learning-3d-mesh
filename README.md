# Geometric Deep Learning for 3D Mesh Classification

This repository contains experiments for classifying 3D meshes with deep learning, including training diagnostics and iterative architecture/training refinements.

## What this project demonstrates

- 3D geometric data preprocessing and representation
- Mesh classification model training
- Experiment tracking via notebook-based runs and logs
- Performance progression across training epochs

## Tech stack

- Python
- PyTorch
- Jupyter

## How to run

1. Prepare a Python environment with deep learning dependencies.
2. Download/prepare the mesh dataset used by the notebooks.
3. Open and run notebooks in order for each experiment track.

```bash
python -m venv venv
venv\Scripts\activate
pip install torch torchvision numpy matplotlib jupyter
jupyter lab
```

## Results snapshot

Notebook training logs show strong convergence in key runs:

- Test accuracy improves from early low-baseline values (for example `50.0%`) to high-performing checkpoints.
- One tracked run reaches and sustains `100.0%` test accuracy after sufficient epochs in the logged experiment sequence.

## Repository contents

- Multiple experiment notebooks (`Question1` to `Question4`)
- Model/training modification notes in `*_modified.py.txt`
- Supporting report artifact

## Notes

- Large datasets/checkpoints are not included in this repository.
