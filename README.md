# SIR Model: Simulating Epidemic Dynamics

## 📌 Project Overview
This project implements the **SIR (Susceptible-Infected-Recovered) model** to simulate the spread of infections in different geographic scenarios. The study is divided into multiple phases, incorporating epidemiological modeling, population movement, and vaccination strategies.

## 📊 Dataset & Simulations
We designed a simulated population distributed in different city geometries and modeled the spread of an infection using differential equations. The project explores:
- **Phase 1**: Basic SIR model without movement.
- **Phase 2**: Extended model with birth and death rates.
- **Phase 3**: Population movement and cluster-based infection dynamics.
- **Phase 4**: Dynamic simulation with animation, integrating a vaccination strategy.

## 🔬 Methodology
### 1️⃣ SIR Model Formulation
The SIR model is based on the following differential equations:

$$
\frac{dS}{dt} = - \beta \frac{I}{N} S
$$

$$
\frac{dI}{dt} = \beta \frac{I}{N} S - \gamma I
$$

$$
\frac{dR}{dt} = \gamma I
$$

where:
- **S**: Susceptible individuals
- **I**: Infected individuals
- **R**: Recovered individuals
- **β**: Infection rate
- **γ**: Recovery rate
- **N**: Total population

### 2️⃣ Phase-Based Enhancements
- **Phase 1**: Simulated a closed population with no external factors affecting the infection dynamics.
- **Phase 2**: Introduced birth and death rates, adjusting the model for demographic changes.
- **Phase 3**: Implemented movement dynamics in different city geometries (grid-based and clustered populations).
- **Phase 4**: Developed an animated simulation with **ggAnimate**, allowing visualization of disease spread in real time.

## 🚀 Key Findings
- Infection peaks depend on **R0 (basic reproduction number)**, calculated as:

  R_0 = β / γ

- Vaccination strategies can prevent outbreaks if at least **75% of the population is immunized**.
- Mobility and clustering significantly impact how an infection spreads, altering the effectiveness of containment measures.

## 📂 Files in This Repository
- `RetoFase1Final.pdf` - Phase 1: Basic SIR Model implementation.
- `RetoFase2Final1.pdf` - Phase 2: Birth & Death rates incorporated into SIR.
- `MA1002B_Actividad3_R.pdf` - Phase 3: Movement and clustering effects in urban environments.
- `1732945367000Modelo_SIR__Evidencia_Final.pdf` - Final Report covering all phases.

## 🔧 Technologies Used
- **R** (`ggplot2`, `deSolve`, `reshape2`, `ggAnimate`)
- **Mathematical Modeling** (Differential Equations, Epidemiology)
- **Visualization** (Heatmaps, Cluster Plots, Animated Simulations)

## 👨‍💻 How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/your-repository.git
   ```
2. Open the R scripts or PDF reports to explore different model implementations.
3. Adjust parameters (`β`, `γ`, population size) to simulate different outbreak scenarios.

## 🏆 Project Impact
This project provides insights into **epidemiological modeling** and how different variables affect disease spread. The simulation framework can be extended to model **real-world pandemics**, including the impact of interventions like vaccination and quarantine.

## 📩 Contact
For inquiries, feel free to reach out via GitHub or email.

---
*This project was conducted as part of an academic research initiative.*
