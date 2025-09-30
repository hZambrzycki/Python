# Python Projects (CLI, Packages & Notebooks)

---

A small collection of **Python learning projects**:
- **Calculator** – a simple calculator (turn it into a CLI).
- **Messages** – package/import examples.
- **Udemy Notebooks** – Jupyter notebooks from a Python course.

> Goal: show clean structure, reproducible envs, and a tiny test suite.

---

##  Project structure
```
.
├─ calculator/ # Calculator app (turn into CLI)
│ ├─ calculator.py
│ └─ tests/
├─ messages/ # Import/package demo
│ ├─ init.py
│ └─ example.py
├─ notebooks/ # Jupyter notebooks (formerly "Python Udemy Course")
│ └─ *.ipynb
├─ pyproject.toml # (optional) build system & tools
├─ requirements.txt # runtime/dev deps
└─ README.md
```

---

## Getting started

```bash
# Create and activate a virtual env (uv or venv)
python -m venv .venv && source .venv/bin/activate
pip install -U pip
pip install -r requirements.txt
```

## Run the calculator
```
python -m calculator.calculator  # or: python calculator/calculator.py
```
## Open notebooks
```
pip install jupyter
jupyter lab

```

##  Tests & Quality
```
pip install -r requirements.txt  # includes pytest/ruff/black if you keep them here
pytest -q
ruff check .
black --check .
```
# Tech

Python 3.11+ recommended

Jupyter Notebooks for exploration

pytest, ruff, black (optional)
