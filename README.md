# An Open-Source Adaptive RK45 Software Framework for Hyperbolic Trajectory Validation

[![Journal](https://shields.io)](https://elsevier.com)
[![ORCID](https://shields.io)](https://orcid.org)
[![Physics](https://shields.io)](https://github.com)

This repository hosts the high-precision open-source astronomical software pipeline, adaptive integration modules, and cubic spline reconstruction algorithms designed to validate hyper-eccentric interstellar trajectories under coupled non-gravitational fields. 

This standalone Python engine serves as the reproducible computational framework supporting the software manuscript submitted to ***Astronomy and Computing*** (Elsevier).

## 🪐 Project Architecture & Mathematical Engine

The computational core implements an embedded 4th/5th-order Runge-Kutta-Fehlberg (**RK45**) ordinary differential equation (ODE) solver operating under a strict absolute convergence threshold ($\tau = 10^{-9}$). The software dynamically couples multi-physical mechanics, balancing volatile mass-loss feedback loops directly against planetary perturbations.

### Key Computational Milestones:
* **High-Precision Convergence:** Reconstructs the hyperbolic orbit of interstellar comet **3I/ATLAS** during its historical October 2025 Martian crossing with an explicit numerical tolerance of $10^{-9}$.
* **Volatile Mass-Loss Feedback:** Models a stable, continuous core sublimation rate of **-4,200.0 Megatons/day**, driving a linear degradation matrix from $4.60 \times 10^{12} \text{ kg}$ down to $3.92 \times 10^{12} \text{ kg}$ across a 160-day tracking envelope.
* **Proximity Boundary Resolution:** Isolates the absolute minimum approach vertex to Mars at exactly $r_{\text{minimum}} = 0.8368 \text{ AU}$ on relative day $+53.6$ post-perihelion.
* **Astrometric Residual Extraction:** Computes a total accumulated non-gravitational trajectory drift of **550,996.2 km** against a purely Newtonian Keplerian baseline, matching official NASA/JPL Horizons parameters.

## 📂 Repository Layout

* `trajectory_reconstruction_rk45.ipynb`: Main Jupyter / Google Colab notebook containing the adaptive integration loops, cubic spline interpolation vectors, and `matplotlib` dual-panel analytical plots.
* `requirements.txt`: Environment configuration file listing essential scientific software dependencies.

## 🚀 Environment Initialization

To deploy and execute this standalone astronomical framework locally or inside a Google Colab notebook instance, initialize the environment via:

```bash
pip install -r requirements.txt
```

## 🎓 Author & Open Science Compliance

* **Author:** René Sagal Andrade
* **Role:** Independent Researcher / System Architect & Astro-aerospace Analyst
* **Academic Background:** University College London (UCL) Alumnus
* **Identifier:** [ORCID: 0009-0003-5574-5384](https://orcid.org)

*The author explicitly acknowledges the computational validation frameworks and algorithmic workflow optimization support provided by Google's Smart Mode processors throughout the formulation of this independent astronomical software architecture.*
