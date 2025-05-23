# Entangled Learning 2.x — Teacher-Student Output Alignment

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/madara88645/entangled-ai-ts/blob/main/entangled_student_teacher.ipynb)

This project demonstrates **entangled learning**, where a small student model learns from both true labels and the output distribution of a larger teacher model. Two main modes are implemented:

- **Entangled 2.0:** Symmetric co-learning between teacher and student using both original and PCA-transformed inputs.
- **Entangled 2.1:** Asymmetric, distillation-like learning where only the student model is updated.

## 🚩 Features

- Bidirectional KL divergence alignment between models
- Dynamic λ coefficient (logarithmic schedule)
- PCA-based input simplification for the student
- Visualized training loss and KL divergence metrics

## 📁 Project Structure

- `entangled_student_teacher.ipynb` — Interactive demo notebook
- `entangled_train.py` — Standalone Python training script
- `requirements.txt` — Python dependencies
- `README.md` — Project overview and instructions

## 🚀 Getting Started

**Option 1: Run in Colab**  
Click the badge above to launch the interactive notebook in Google Colab — no setup required!

**Option 2: Local Installation**

```bash
pip install -r requirements.txt
python entangled_train.py
```
🔬 Results
Both student and teacher models improve their predictions with collaborative training. KL divergence analysis demonstrates the effects of asymmetric vs symmetric learning.

Feel free to open issues or pull requests for questions or improvements!


