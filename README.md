# Optimization with Golden Section Search

A from-scratch Python implementation of the **Golden Section Search** algorithm — a derivative-free one-dimensional optimization method — applied to two different practical problems.

## Overview

The Golden Section Search algorithm, which progressively narrows the interval of uncertainty using the golden ratio constant (~0.618), is implemented from scratch and applied to two separate optimization problems. For each problem, an iteration table is produced, the result found by the algorithm is verified against the derivative-based analytical solution, and the results are visualized with plots.

## Problems

**1. Profit Maximization**
Determining the optimal selling price for a rare collection in a secondhand bookstore.

- Function: f(x) = -2.1x² + 84.4x - 150
- Range: 10–30 (thousand TL) · Tolerance: ε = 0.1
- Result: Optimal price ≈ **20.10**, maximum profit ≈ **698.02** (analytical solution: x = 20.1)

**2. Error Minimization**
Calculating the optimal daily nutritional supplement amount for the healthy growth of elephant calves.

- Function: E(x) = 1.2x² - 7.6x + 15
- Range: 0–6 (kg) · Tolerance: ε = 0.1
- Result: Optimal amount ≈ **3.16 kg**, minimum error ≈ **2.97** (analytical solution: x ≈ 3.166)

## Method

- Manual implementation of the Golden Section Search algorithm (no built-in optimization libraries)
- Tracking the interval of uncertainty (b − a) at each iteration with an iteration table
- Verifying the results against the derivative-based analytical solution (first and second derivative checks)
- Visualizing the optimal points with `matplotlib`

## Libraries Used

`math` · `numpy` · `matplotlib`

## Usage

```bash
pip install numpy matplotlib
jupyter notebook YapayZekaOptimizasyonu.ipynb
```

## License

This project is licensed under the MIT License.
