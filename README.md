# Probabilistic Modeling of Gas Hydrates Kinetics

---

## 📌 Overview

This repository contains the implementation of **probabilistic models** to predict and analyze the **kinetics of gas hydrate formation and dissociation**. Gas hydrates are crystalline structures formed by gas molecules trapped in water cages under high pressure and low temperature conditions.

Understanding their kinetics is crucial for applications in:
- Flow assurance in pipelines
- Energy recovery
- Climate studies

This project implements **Maximum Likelihood Estimation (MLE)**, **Maximum A Posteriori (MAP)**, and **Bayesian Inference** based approaches for parameter estimation.



---

## 🚀 Features

- 📊 **Data preprocessing & thermodynamic setup:** Prepare experimental data and establish the thermodynamic framework for analysis.
- ⚙️ **Implementation of MLE, MAP, and Bayesian models:** Core algorithms for parameter estimation.
- 🔬 **Application of thermodynamic equations:** Integrate physical laws governing hydrate growth.
- 📈 **Visualization:** Generate plots for growth curves, probability distributions, and parameter convergence.
- 🔄 **Comparative Analysis:** Compare model predictions with experimental or benchmark data to validate results.

---

## 🛠️ Technologies Used

- **Python 3.10+**
- **NumPy & SciPy** – for numerical computation
- **Pandas** – for data handling and manipulation
- **Matplotlib & Seaborn** – for plotting and visualization
- **PyMC / ArviZ** – for Bayesian inference and model checking
- **Jupyter Notebook** – for experimentation and documentation

---

## 📂 Repository Structure

```bash
.
├── dataset/
│   └── # Raw and processed data for different experimental conditions
├── MLE-MAP/
│   └── # Scripts and notebooks for ML & MAP modeling
├── full-bayesian-inference/
│   └── # PyMC/ArviZ implementation of the Bayesian model
├── requirements.txt
└── README.md
```

---

## 🧪 The Dataset

The experimental data used in this project was generated to study the effects of various kinetic promoters and conditions on gas hydrate formation. The dataset encompasses experiments conducted in two different scales of reactors:
- A small-scale reactor with a volume of 500 ml.
- A large-scale reactor with a volume of 25 L.

Experiments were performed using three distinct chemical promoters (catalysts) at various concentrations:
###### 1. Methionine
###### 2. SDS
###### 3. Tryptophan

Furthermore, to study the influence of surface area on kinetics, the experiments were run under two surface conditions: with and without the use of surface packing material.

---

## 📊 Methodology

### 1. Thermodynamic Preprocessing
- Implemented hydrate formation equations using **pressure, temperature, and fugacity relations**.
- Computed derived kinetic parameters like gas conversion, growth rate, and induction time (t90).

### 2. Probabilistic Models
- **MLE (Maximum Likelihood Estimation):** Estimates parameters that maximize the likelihood of observing the given data. This approach is purely data-driven.
- **MAP (Maximum A Posteriori):** Extends MLE by incorporating **prior knowledge** about the parameters. The final estimate is a balance between the prior belief and the data likelihood.
- **Bayesian Inference:** Generates full **posterior distributions** for parameters using Markov Chain Monte Carlo (MCMC) sampling, providing a complete picture of parameter uncertainty.

### 3. Validation
- Compared model-predicted growth curves against experimental data.
- Analyzed parameter uncertainty and convergence diagnostics (e.g., trace plots).
- Visualized the resulting probability density functions to understand parameter distributions.

---

## ⚡ Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/pushpdeep07/probabilistic-modeling-gas-hydrates.git](https://github.com/pushpdeep07/probabilistic-modeling-gas-hydrates.git)
    cd probabilistic-modeling-gas-hydrates
    ```

2.  **Create and activate a virtual environment (recommended):**
    ```bash
    # Create the environment
    python -m venv venv

    # Activate on macOS/Linux
    source venv/bin/activate

    # Activate on Windows
    venv\Scripts\activate
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

---

## ▶️ Usage

All models and analyses are organized into their respective directories.
- ### For MLE and MAP modeling:
   Navigate to the MLE-MAP/ directory and run the Jupyter notebooks or Python scripts contained within.
- ### For Full Bayesian Inference:
  Navigate to the full-bayesian-inference/ directory to run the PyMC models.

---

## 📈 Example Results

#### Hydrate Growth Curve Prediction
*A comparison between the model-predicted hydrate growth curve and the experimental data.*

#### Posterior Distribution (from Bayesian Model)
*Posterior probability distributions for kinetic parameters, showing the mean values and uncertainty.*

---

## 📖 References

1.  Sloan, E. D., & Koh, C. A. (2007). *Clathrate Hydrates of Natural Gases*. CRC press.
2.  Smith, J. M., Van Ness, H. C., & Abbott, M. M. *Introduction to Chemical Engineering Thermodynamics*.
3.  Atkins, P., & de Paula, J. *Physical Chemistry*.

---

## 👨‍💻 Author

**Pushpdeep Teotia**

-   IIT Kanpur | Mechanical Engineering
-   [GitHub](https://github.com/pushpdeep07)

---

## 📜 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
