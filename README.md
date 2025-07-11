# 📊 Optimization Methods for Recommender Systems

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Datasets](https://img.shields.io/badge/Datasets-MovieLens%20%26%20XWines-green)]()

---

## 🔍 Overview

Matrix completion aims to reconstruct a complete matrix from a
subset of observed entries, typically under a low-rank assumption.
We focus on the Frank–Wolfe (FW) algorithm and its pairwise
variant (PFW), which are projection-free methods suited for
large-scale problems. 

This project explores **matrix completion** for recommender systems under a low-rank assumption.  
We implement and compare the following optimization methods:

- **Frank–Wolfe (FW)**
- **Pairwise Frank–Wolfe (PFW)**

Each method is tested with four step-size strategies:

- `Fixed`
- `Exact Line Search`
- `Armijo Backtracking`
- `Lipschitz-based Step`

---

## 📁 Datasets

- **[MovieLens-100k](https://grouplens.org/datasets/movielens/100k/)**  
- **X-Wines** (custom or synthetic dataset)

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/optimization-recommender-systems.git
cd optimization-recommender-systems
pip install -r requirements.txt
