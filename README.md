A/B Testing for Conversion Optimization

An E-commerce startup wants to know whether a new checkout funnel (Variant B) performs better than the old one (Variant A). This project answers that question using simulated visitor data and standard statistical tests in Python.

What this project does
Simulates data: 10,000 visitors per variant, with true conversion rates of 10% (A) and 12% (B).
Calculates conversion rates and 95% confidence intervals for both variants.
Plots conversion rates as a bar chart with error bars.
Runs a two-proportion z-test (one-sided, H1: B > A) to check if B significantly beats A.
Sequential testing: simulates visitors arriving in batches and tracks the p-value and observed lift in real time.
Tech stack
Python 3
NumPy, Pandas
SciPy, Statsmodels
Matplotlib
Setup
bash
pip install numpy pandas scipy statsmodels matplotlib ipython
How to run
bash
python testing.py

The sequential testing section uses IPython.display.clear_output, so it displays best in Jupyter or Google Colab.

Project structure
.
├── testing.py   # Full analysis: simulation, CI, plot, z-test, sequential testing
└── README.md
Key concepts
Confidence interval: range in which the true conversion rate likely lies (95% level).
Two-proportion z-test: checks whether the difference between two conversion rates is statistically significant.
Sequential testing: monitoring results batch by batch instead of waiting for the full sample.
Author


