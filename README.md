# Entangled Learning 2.x — Teacher-Student Output Alignment

This project demonstrates **entangled learning** where a small student model learns from both true labels and the output distribution of a larger teacher model. Two modes are implemented:

- **Entangled 2.0**: Symmetric co-learning between teacher and student using original and PCA-transformed inputs.
- **Entangled 2.1**: Asymmetric distillation-like learning where only the student is updated.

### 📌 Features

- Bidirectional KL divergence alignment
- Dynamic λ coefficient (logarithmic increase)
- PCA-based input simplification for student
- Visualized training loss and KL divergence

### 📁 Files

- `entangled_student_teacher.ipynb`: Full interactive notebook
- `entangled_train.py`: Standalone Python training script
- `requirements.txt`: Dependencies
- `README.md`: Project overview

### 🚀 Run

```bash
pip install -r requirements.txt
python entangled_train.py
```

> Or open the notebook directly in JupyterLab.

### 🔬 Results

Both student and teacher improve their predictions with collaborative training.
KL divergence analysis shows the effects of asymmetric vs symmetric learning.
