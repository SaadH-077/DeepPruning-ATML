# 🧠 Neural Network Pruning — Comparative Analysis & Distillation  
A course project exploring pruning strategies in deep learning: unstructured, structured, and the lottery ticket hypothesis. The experiments include analysis of sparsity, parameter efficiency, accuracy tradeoffs, and knowledge distillation.

> 🧠 **Course**: Advanced Topics in Machine Learning (ATML - CS)  
> 📅 **Semester**: Fall 2024  
> 🎓 **Institution**: LUMS

---

## 📁 Directory Structure

```
Neural-Network-Pruning-ATML/
│
├── notebooks/                     
│   ├── Task1.1_Unstructured_Pruning.ipynb
│   ├── Task1.2_Structured_Pruning.ipynb
│   ├── Task1.3_Comparison_Analysis.ipynb
│   ├── Task2_Knowledge_Distillation.ipynb
│   └── Task3_Lottery_Ticket_Hypothesis.ipynb
│
├── report/
│   └── DeepPruning - Final Report.pdf
```

---

## 🧪 Tasks & Methodology

### 🔹 **Task 1: Pruning Strategies**
- **1.1 Unstructured Pruning**:  
  Magnitude-based weight pruning using global and layer-wise approaches.

- **1.2 Structured Pruning**:  
  Channel-wise and filter-wise pruning to evaluate hardware-friendly sparsity.

- **1.3 Comparative Analysis**:  
  - Accuracy vs sparsity
  - Parameter count and FLOPs
  - Convergence plots

### 🔹 **Task 2: Knowledge Distillation**
- A teacher-student training paradigm where a pruned model is trained using softened outputs from a higher-capacity teacher.

### 🔹 **Task 3: Lottery Ticket Hypothesis**
- Demonstrates the existence of a sparse subnet that, when trained from scratch, can match or outperform the original network.
- Includes iterative pruning + reset approach for identifying "winning tickets".

---

## 📈 Key Results

| Task | Objective | Outcome |
|------|-----------|---------|
| Task 1 | Compare pruning methods | Structured pruning more hardware-friendly but less accurate |
| Task 2 | Knowledge distillation | Student model benefits from teacher guidance |
| Task 3 | Lottery Ticket Hypothesis | Sparse subnetworks outperform random pruned ones |

---

## 🧠 Core Learnings
- **Unstructured pruning** yields high sparsity but lacks structured efficiency.
- **Structured pruning** provides better FLOPs reduction for deployment.
- **Distillation** improves generalization in pruned networks.
- **Lottery ticket subnetworks** often outperform arbitrary pruned networks when retrained.

---

## 🛠 How to Run
Open each notebook under `/notebooks` in a Jupyter environment and execute sequentially.

Ensure that you have installed:
- `torch`
- `torchvision`
- `matplotlib`
- `numpy`

```bash
pip install torch torchvision matplotlib numpy
```

---

## 📄 Citation
If you reference this project or build upon it:
```bibtex
@project{NNPruningATML2025,
  title = {Neural Network Pruning — Structured, Unstructured, and Hypothesis-Based Strategies},
  note = {Developed as part of ATML course at LUMS, Spring 2025}
}
```

---

> “A smaller network that learns what matters can outperform a larger one that learns everything.”

