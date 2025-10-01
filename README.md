# Synchronization Threshold in Coupled Logistic Maps: A Numerical Reproduction

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17244363.svg)](https://doi.org/10.5281/zenodo.17244363)

This repository provides a **reproducible numerical study** of the synchronization transition in coupled logistic-map lattices (CMLs). We compute both the **largest Lyapunov exponent (LLE)** and the **transverse Lyapunov exponent (TLE)** using a Benettin-style method and show a **sustained TLE zero-crossing** at **ε ≈ 0.3462** for mean-field coupling, while **LLE remains positive** (≈0.45–0.50) — i.e., *chaos preserved, differences killed*.

> 📄 The archival white paper (PDF), figure, and data bundle are on Zenodo:  
> **https://doi.org/10.5281/zenodo.17244363**

---

## What’s in here

- `synchronization_threshold_cml_whitepaper_with_fig.pdf` – the scientific white paper  
- `lle_tle_vs_eps.png` – LLE & TLE vs ε plot with the crossing marked  
- `lle_tle_vs_eps_data.csv` – example (ε, LLE, TLE) data (for format/repro)  
- `notebooks/` – optional Colab-ready one-cell scripts (LLE/TLE sweep, snapshots)

---

## Quick start (Colab)

1. Open a new Google Colab notebook.
2. Paste a **one-cell mean-field sweep** (LLE + TLE) block from `notebooks/meanfield_zoom.py` (or the snippet in the paper).
3. Run. You should see:
   - LLE ~ 0.45–0.50 across the range,
   - TLE crossing < 0 at **ε ≈ 0.346** (sustained),
   - Figure saved, CSV written.

> Tip: Increase `measure_T` near the crossing and try 2–3 seeds to tighten the estimate.

---

## Results (tl;dr)

- **Measured sustained crossing:** ε_c ≈ **0.3462**  
- **Predicted from single-map Lyapunov:** ε_c = 1 − exp(−Λ_single)  
  - With Λ_single ≈ 0.45 → ε_c ≈ **0.362**  
- **Agreement:** measured and predicted values are in close accord  
- **Interpretation:** synchronized chaos; common trajectory stays chaotic (LLE>0), transverse differences decay (TLE<0)

---

## Why this repo exists

This is a **clean, scoped reproduction** of a classic phenomenon in spatiotemporal chaos (Kaneko, 1990). It’s suitable for:
- teaching/learning **Lyapunov exponent** computation in extended systems,
- lab exercises in **nonlinear dynamics / computational physics**,
- serving as a template for **reproducible simulations**.

---

## Reference

Kaneko, K. (1990). *Clustering, coding, switching, hierarchical ordering, and control in a network of chaotic elements.* **Physica D** 41(2), 137–172.

---

## Cite this work

> Devine, J.M. (2025). *Synchronization Threshold in Coupled Logistic Maps: A Numerical Reproduction* (v3.8). Zenodo. https://doi.org/10.5281/zenodo.172443633
