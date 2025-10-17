# Copilot Instructions for AI Coding Agents

## Project Overview
This repository contains Google Colab notebooks and reports for the Deep Learning course at UBA. Each practical assignment (TP) is organized in its own folder (`TP1/`, `TP2/`), with corresponding notebooks and PDF reports. The main focus is on neural network architectures, training strategies, and experiment documentation.

## Key Directories & Files
- `TP1/tp1.ipynb`, `TP2/tp2.ipynb`: Main Colab notebooks for each assignment. All code and experiments are here.
- `TP1/informe.pdf`, `TP2/Trabajo Práctico 2.pdf`: Assignment reports.
- `TP1/imagenes/`: Contains image datasets used in experiments, organized by resolution.
- `README.md`: High-level project description and usage notes.

## Developer Workflow
- **Notebook-first development:** All code, experiments, and results are maintained in `.ipynb` files. Do not create standalone Python scripts unless explicitly requested.
- **Google Colab compatibility:** Ensure all code runs in Colab. Use Colab-specific features (e.g., `from google.colab import drive`) only if required by the notebook context.
- **Data access:** Image datasets are local to the repo. For Colab, instruct users to upload or mount the dataset as needed.
- **Documentation:** Each TP must have a corresponding PDF report summarizing methodology and results.

## Project Conventions
- **No external dependencies** beyond standard Python ML/data libraries (e.g., TensorFlow, PyTorch, NumPy, Matplotlib) unless specified in the notebook.
- **Experiments and results** should be reproducible from the notebook alone.
- **File organization:** Keep all files for each TP within its respective folder. Do not move or rename files unless updating the assignment structure.
- **Naming:** Use clear, descriptive names for notebooks and reports (e.g., `tp1.ipynb`, `informe.pdf`).

## Integration & Patterns
- **No cross-TP code sharing:** Each TP is self-contained. Do not refactor code across TPs unless creating a shared utility is explicitly requested.
- **Image loading:** Reference images using relative paths (e.g., `imagenes/50x50/panda.bmp`).
- **Results storage:** Save experiment outputs (plots, metrics) within the notebook or in the TP folder.

## Example: Loading Images in a Notebook
```python
from PIL import Image
img = Image.open('imagenes/50x50/panda.bmp')
```

## Summary
- Focus all work in notebooks within TP folders
- Ensure reproducibility and Colab compatibility
- Maintain clear separation between assignments
- Document results in both notebook and PDF report

---
If any conventions or workflows are unclear, ask for clarification before proceeding with major changes.
