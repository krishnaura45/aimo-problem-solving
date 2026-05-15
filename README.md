# AI Mathematical Olympiad - Progress Prize 3 ~ `92nd Place Solution`
> Solving olympiad-level mathematical reasoning problems using open-source LLM inference pipeline and competitive reasoning workflow.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![LLM](https://img.shields.io/badge/Open--Source-LLMs-purple?style=for-the-badge)
![Math Reasoning](https://img.shields.io/badge/AI-Math%20Reasoning-blueviolet?style=for-the-badge)
![Best Score](https://img.shields.io/badge/Best%20Score-43.0-2ECC71?style=for-the-badge)
![Rank](https://img.shields.io/badge/Rank-92%20of%204138-brightgreen?style=for-the-badge)
![Solo](https://img.shields.io/badge/Submission-Solo-orange?style=for-the-badge)

### **Project Duration**: April 01, 2026 - April 15, 2026

---

## File Structure

```bash
├── INFO.md                      # Competition details, evaluation, rules and timeline
├── README.md
├── aimo-inference.ipynb         # Main competition inference pipeline
├── dependency-install.ipynb     # Dependency installation and environment setup
├── inference.py                 # Standalone inference script
├── utils.ipynb                  # Utility experiments and helper workflows
├── assets
│   └── eval_info.png            # helper image
└── output
    └── submission.parquet       # Best submission file
```

### Installation

```bash
git clone https://github.com/krishnaura45/aimo-problem-solving.git
cd aimo-problem-solving
```

### Usage

```bash
# Open notebook workflow
jupyter notebook aimo-inference.ipynb

# or run standalone inference
python inference.py
```

---

## Problem Statement

The goal of the **[AI Mathematical Olympiad - Progress Prize 3](https://www.kaggle.com/competitions/ai-mathematical-olympiad-progress-prize-3)** Kaggle competition was to create open-source algorithms capable of solving olympiad-level mathematical reasoning problems written entirely in LaTeX notation.

The competition featured highly challenging problems spanning:

- Algebra
- Combinatorics
- Geometry
- Number Theory

with difficulty ranging from national olympiad level up to IMO-standard mathematics.

Hosted on Kaggle, the challenge evaluated submissions using a specialized penalized accuracy framework across public and hidden private reruns. Each problem required predicting a non-negative integer answer between `0` and `99999`.

The competition emphasized genuine mathematical reasoning capabilities and robust inference under constrained notebook environments.

---

## Approach

### Inference Pipeline

The primary workflow was implemented in:

- `aimo-inference.ipynb`
- `inference.py`

The overall pipeline focused on efficient large language model inference under strict Kaggle notebook constraints.

---

### Problem Processing

- Processed olympiad-style mathematical problems written in LaTeX
- Structured prompts for reasoning-oriented inference
- Managed sequential problem evaluation using Kaggle's competition API

---

### Reasoning Workflow

The inference workflow emphasized:

- Multi-step mathematical reasoning
- Symbolic interpretation of problem statements
- Integer answer extraction and normalization

The system was designed to remain robust under:

- Randomized evaluation ordering
- Hidden private reruns
- Runtime and memory limitations

---

### Submission Strategy

- Generated predictions sequentially through the official evaluation API
- Exported final outputs into:
  - `submission.parquet`

The workflow complied with competition constraints including:

- Internet-disabled execution
- GPU notebook runtime restrictions
- API-generated submission files

---

### Supporting Utilities

Additional repository components included:

- Dependency installation notebooks
- Utility experimentation workflows
- Evaluation visualization assets

---

## Competition Results

- Announced on: May 13, 2026.

- **Public/Private Leaderboard Scores**:
  - `37`
  - `38`
  - `39`
  - `40`
  - `42`
  - `43`

- **Performance**:
  - **Best Private Score**: `43.0`
  - Placed **92nd out of 4066 participants** and **4138 teams** as a **solo participant**.

---

## References

- Dataset: [AIMO - PP3](https://www.kaggle.com/competitions/ai-mathematical-olympiad-progress-prize-3/data)
- Competition Info: `INFO.md`
- Main Inference Notebook: `aimo-inference.ipynb`
- Official Models Page: https://www.kaggle.com/competitions/ai-mathematical-olympiad-progress-prize-3/models

---

## Tech Stack

- **Language**: Python
- **Libraries / Frameworks**:
  - `transformers`
  - `torch`
  - `pandas`
  - `numpy`
- **Techniques**:
  - LLM Inference
  - Mathematical Reasoning
  - Sequential API-based Evaluation
  - Prompt-based Solving
- **Tools**:
  - Jupyter Notebook
  - Kaggle Notebooks
  - GPU-based inference environments

---

📌 *This project demonstrates the growing capability of open-source reasoning systems in solving olympiad-level mathematical problems under competitive inference constraints.*
