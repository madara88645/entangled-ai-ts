
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/madara88645/entangled-ai-ts/blob/main/entangled_student_teacher.ipynb)

📖 **Read the full article on Medium**:  
[Entangled Learning 2.x — Think Together, Train Smarter](https://medium.com/@mehmet.ozel2701/entangled-learning-2-x-92ea4f84345a)

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
