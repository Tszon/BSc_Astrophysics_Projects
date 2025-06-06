# Final-Year Project: Gradient-Based Orbital Transfer Optimisation with MCMC-Driven Random Walkers

An orbital dynamics simulation that models the docking manoeuvre of two spacecraft using **differential equations**, optimises fuel usage and transfer time with **gradient descent**, and estimates uncertainty using **MCMC-based random walkers**.

---

## 📚 Table of Contents

- [🧠 Project Motivation](#-project-motivation)
- [📐 Technologies Used](#-technologies-used)
- [🔭 Project Scope](#-project-scope)
- [⚙️ How It Works](#️-how-it-works)
- [📊 Visualisations](#-visualisations)
- [🚧 Challenges](#-challenges)
- [🎯 Intended Use](#-intended-use)
- [📌 Limitations](#-limitations)
- [🤝 Credits](#-credits)

---

## 🧠 Project Motivation

This project emerged from my final-year research at the **University of Hertfordshire**, where I aimed to apply theoretical astrophysics to a practical engineering problem—docking optimisation in multi-body orbital mechanics. The goal was to simulate and improve autonomous spacecraft docking via algorithmic optimisation and probabilistic modelling.

---

## 📐 Technologies Used

- **Python**
- `numpy`, `scipy` – numerical methods, ODE solvers
- `matplotlib`, `seaborn` – plotting and animation
- `emcee` – Markov Chain Monte Carlo for uncertainty quantification
- `PyMC` – Bayesian regression (optional extension)
- `LaTeX` – scientific documentation and reporting

---

## 🔭 Project Scope

This simulation models:

- Orbital parameters (e.g. positions & velocities in `x`, `y` & `z`-axis) of an interceptor spacecraft
- Optimal velocity (`v`) and trajectory angle (`θ`) using **gradient descent**
- Cost function `J(v, θ)` minimised iteratively
- Uncertainty quantification via **Bayesian inference** using **MCMC**
- Animated visualisation of convergence and trajectory paths

---

## ⚙️ How It Works

1. **Define physical model**: orbital mechanics via Newtonian physics
2. **Formulate cost function**: based on docking constraints
3. **Optimise**: gradient descent updates `(v, θ)` iteratively
4. **Quantify uncertainty**: use `emcee` to explore the posterior distribution
5. **Visualise**: plot contours, convergence, and trajectory path

> 🔬 _See `BSc_Astrophysics_Projects/GradientDescentOptimisation_MCMC/02_transfer_optimisation+MCMC.ipynb` for a step-by-step walkthrough._

---

## 📊 Visualisations

- Descent path over cost surface  
- Convergence of cost function  
- Posterior distributions of burn parameters
-  Optimised Trajectory 

<!-- Gradient Descent Image -->
<img src="https://github.com/user-attachments/assets/cb2ed5df-9130-438f-bc8b-3c01050a4555" width="600"/>

> *Fig. 1*: Gradient descent over the contour surface plot of the cost function `J`. The white dashed line on the left shows the cost of a classic Hohmann transfer.

<!-- Cost vs Iteration -->
<img src="https://github.com/user-attachments/assets/8396b779-e1fb-4147-a851-974feeff4c9f" width="600"/>

> *Fig. 2*: Changes in the cost function `J` over gradient descent steps. Notice that it is not a perfectly horizontal
line after reaching the valley (around 130 steps) of the cost function. The descent process becomes much slower when the minimum is close.

<!-- Random Walkers -->
<img src="https://github.com/user-attachments/assets/8a92c9a9-11a6-4c80-8baf-b5da989b2d8f" width="600"/>

> *Fig. 3*: Simulation of random walkers to search for the final converged parameters `(v, θ)`. We observe a sign of stable convergence at around 150 iterations (red dashed lines) for both parameters.

<!-- Optimised Trajectory -->
<img src="https://github.com/user-attachments/assets/26e0c27a-ceae-437f-8ad3-4ee8ac0b3b7c" width="600"/>

> *Fig. 4*: Results of the optimised transfer. Note that a heavier penalty (grey dashed line ---) allows for faster transfer.
.

---

## 🚧 Challenges

- Dealing with stiffness in ODE solvers  
- Tuning learning rate and momentum in gradient descent  
- Ensuring MCMC convergence and burn-in  
- High computational time for repeated sampling

---

## 🎯 Intended Use

- Academic: share with peers, mentors, and for viva demonstration  
- Public: open-source learning resource for aerospace and AI students  
- Portfolio: showcase numerical optimisation and simulation capabilities

---

## 📌 Limitations

- Assumes a 2D docking plane and a simplified gravitational model  
- Ignores fuel leakage, actuator delay, or collision dynamics  
- MCMC assumes Gaussian noise

---

## 🤝 Credits

- **Tszon Tseng** – project author  
- Supervised by [Dr. James Collett](https://researchprofiles.herts.ac.uk/en/persons/james-collett) and [Professor Detlef Mueller](https://researchprofiles.herts.ac.uk/en/persons/detlef-mueller)
- Inspired by orbital mechanics applications & gradient-based ML methods in Deep Learning
- MCMC logic adapted from [emcee GitHub](https://github.com/dfm/emcee)

---

## 📬 Contact

Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/tszon-tseng-a381aa297/) or raise an issue if you'd like to collaborate or suggest improvements.

---


