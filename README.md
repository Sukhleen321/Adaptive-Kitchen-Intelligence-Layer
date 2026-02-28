# Adaptive-Kitchen-Intelligence-Layer
Simulation-based signal enhancement framework to improve Kitchen Prep Time (KPT) prediction stability and reduce error using bias correction and stress indexing.

Overview: 
This project was developed for Zomathon 2026 (Problem Statement 1).
The goal is to improve Kitchen Prep Time (KPT) prediction by improving input signals instead of changing the existing model.

Problem: 
KPT currently depends on merchant-marked “Food Order Ready” (FOR) timestamps, which can be biased or delayed.
This causes early rider arrivals, waiting time, and unstable ETAs.

Solution
We introduced a signal enhancement layer:
Merchant Bias Index (MBI) to correct systematic FOR timestamp bias.
Live Kitchen Stress Index (LKSI) to estimate real-time kitchen rush using operational signals.
Adjusted KPT using corrected timestamps and stress factors.

Simulation
A synthetic dataset was created to simulate:
Multiple merchants
Average prep time (~20 mins)
Merchant bias (2–3 mins)
Rush conditions

Performance was evaluated using:
Mean Absolute Error (MAE)
P50 and P90 error
Results showed improved prediction stability after signal correction

Improved KPT accuracy helps reduce rider waiting time, improve ETA reliability, and increase operational efficiency.
