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

- 🐍 **Python** – core language
- `numpy`, `scipy` – numerical methods, ODE solvers
- `matplotlib`, `plotly` – plotting and animation
- `emcee` – Markov Chain Monte Carlo for uncertainty quantification
- `PyMC` – Bayesian regression (optional extension)
- `LaTeX` – scientific documentation and reporting

---

## 🔭 Project Scope

This simulation models:

- Orbital parameters of an interceptor spacecraft
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

> 🔬 _See `/notebooks/simulation.ipynb` for a step-by-step walkthrough._

---

## 📊 Visualisations

- 📈 Descent path over cost surface  
- 📉 Convergence of cost function  
- 🌌 Docking trajectory animation  
- 🔄 Posterior distributions of burn parameters

> 🖼️ Add `.png`, `.gif` or `.mp4` inside `/media` and embed them here using:
> ```markdown
> ![Trajectory](media/trajectory.gif)
> ```

---


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

- Assumes 2D docking plane and simplified gravitational model  
- Ignores fuel leakage, actuator delay, or collision dynamics  
- MCMC assumes Gaussian noise

---

## 🤝 Credits

- **Tszon Tseng** – project author  
- Supervised by [Insert Supervisor Name]  
- Inspired by orbital mechanics coursework & gradient-based ML methods  
- Visualisation techniques adapted from [Matplotlib/Plotly Docs]  
- MCMC logic adapted from [emcee GitHub](https://github.com/dfm/emcee)

---

## 📬 Contact

Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/tszon-tseng-a381aa297/) or raise an issue if you'd like to collaborate or suggest improvements.

---


