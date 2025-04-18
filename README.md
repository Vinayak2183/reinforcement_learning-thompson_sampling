# reinforcement_learning-thompson_sampling
# 🎯 Thompson Sampling - Ad Selection Optimization

This repository implements the **Thompson Sampling** algorithm to solve the ad selection problem using a simulated dataset. The algorithm aims to maximize the number of ad clicks over a series of 10,000 rounds across 10 different advertisements.

---

## 📊 Problem Statement

You are given a dataset that tracks user responses to 10 ads over **10,000 rounds**. Each row represents a round and contains binary values:

- `1` → The ad was clicked.
- `0` → The ad was not clicked.

The challenge is to use **Thompson Sampling** to choose the best ads dynamically, increasing total rewards by learning from past user behavior.

---

## 📁 Dataset Description

- **Rows:** 10,000 (each represents a round)
- **Columns:** 10 (each column is an ad)
- **Values:** Binary (1 = clicked, 0 = not clicked)

---

## 🧠 Algorithm Used

### Thompson Sampling

Thompson Sampling is a **probabilistic** algorithm for solving the **multi-armed bandit** problem. It uses Bayesian inference to estimate the probability of success for each option and makes selections based on samples from these distributions.

Advantages:
- Naturally balances exploration and exploitation.
- Performs well in practice for problems with binary rewards.

---

## 📓 Notebook Contents

- Loading and understanding the dataset
- Implementing the Thompson Sampling algorithm
- Counting ad selections
- Visualizing results and analyzing performance

---

## 📈 Visualization

The notebook provides:

- A histogram of the number of times each ad was selected
- Total reward across all rounds
- Best-performing ad based on observed outcomes

---

## 📦 Dependencies

Make sure the following Python libraries are installed:

```bash
pip install numpy matplotlib pandas
