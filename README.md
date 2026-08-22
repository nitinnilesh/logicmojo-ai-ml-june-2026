# LogicMojo AI/ML - June 2026

Lecture notes, live class notebooks, assignments, and supporting material for the LogicMojo AI/ML June 2026 batch.

Instructor: Nitin Nilesh

## Repository Structure

```text
logicmojo-ai-ml-june-2026/
├── lecture_materials/
│   ├── 01_linear_regression/
│   │   ├── notes/
│   │   └── notebooks/
│   ├── 02_polynomial_regression/
│   │   ├── notes/
│   │   └── notebooks/
│   └── 03_logistic_regression/
│       ├── notes/
│       └── notebooks/
├── assignments/
├── datasets/
└── assets/
```

## Lecture Schedule

| Lecture Number | Lecture Name | Date | Materials |
| --- | --- | --- | --- |
| 1 | Linear Regression Univariate | 08th Aug | `lecture_materials/01_linear_regression/` |
| 2 | Linear Regression Multivariate | 09th Aug | `lecture_materials/01_linear_regression/` |
| 3 | Polynomial Regression | 15th Aug | `lecture_materials/02_polynomial_regression/` |
| 4 | Logistic Regression | 16th Aug | `lecture_materials/03_logistic_regression/` |
| 5 | Logistic Regression Imbalanced Data | 22nd Aug | `lecture_materials/03_logistic_regression/` |

## Notebooks

Each topic folder contains the notebooks used during live teaching sessions.

## Assignments

Assignments are placed topic-wise inside the `assignments/` folder.

## Setup

Create a virtual environment and install the required packages:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Open notebooks using Jupyter:

```bash
jupyter notebook
```

## Dataset Policy

Large datasets should not be committed directly to this repository. Prefer notebooks that download datasets automatically, or add small sample datasets only when required.
