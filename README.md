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

## 🧩 Problem Formulation

We solve the following optimization problem:

```math
\min_{X \in \mathbb{R}^{n_1 \times n_2}} \frac{1}{2} \| \mathcal{P}_\Omega(X - U) \|_F^2 \quad \text{s.t.} \quad \|X\|_* \leq \tau

Where:

U: the partially observed input matrix.

Ω: set of observed indices.

P_Ω(Z)[i,j] = Z[i,j] if (i,j) ∈ Ω, 0 otherwise.

||X||_*: nuclear norm (sum of singular values of X).

τ: rank-related constraint.


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


