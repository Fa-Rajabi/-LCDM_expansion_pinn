
## Physics-Informed Neural Network for $\Lambda CDM$ Cosmology

### Overview
This project investigates the application of Physics-Informed Neural Networks (PINNs) to reconstruct the history of cosmic expansion in the flat ΛCDM cosmological model.
A conventional neural network (NN) is compared with a physics-informed neural network (PINN) through controlled experiments using synthetic data—incorporating different levels of Gaussian noise. 
The study is then extended to observational measurements of the Hubble parameter, H(z), obtained from cosmic chronometers.
The main goal is to investigate whether imposing physical constraints into the training of a neural network can improve model performance and enable the estimation of cosmological parameters.

### Objectives

- Reconstruct the expansion history H(z) using neural network and physics-informed neural network(PINNs).

- Comparing the performance of NN and PINN using noise-free and noisy synthetic data.

- Investigating the sensitivity of PINN predictions and parameter estimates to observational noise.

- Applying the physics-informed approach to cosmic chronometers measurements.

- Estimating the matter density parameter and the Hubble constant.

### Theoretical Background

The cosmological expansion history H(z) in a flat ΛCDM cosmological model

<p align="center">
  <img src="https://latex.codecogs.com/svg.latex?H(z)=H_0%5Csqrt%7B%5COmega_m(1+z)%5E3+1-%5COmega_m%7D" alt="Hubble parameter equation">
</p>
Differentiating this expression with respect to redshift gives the physics-informed constraint used in the PINN:
<p align="center">
  <img src="https://latex.codecogs.com/svg.latex?2H%5Cfrac%7BdH%7D%7Bdz%7D-3%5COmega_m(1+z)%5E2%3D0" alt="Physics-informed constraint equation">
</p>

### Results

- Both NN and PINN can reconstruct the expansion history of the underlying ΛCDM model.

- In the noisy-data comparison, the PINN achieves a lower mean squared error relative to the true analytical solution.

- In the Cosmic Chronometer Analysis, the parameter estimates reported in the notebook are:

<p align="center">
  <img src="https://latex.codecogs.com/svg.latex?%5COmega_m%20%5Capprox%200.30652" alt="Omega_m approximately 0.30652">
</p>
<p align="center">
  <img src="https://latex.codecogs.com/svg.latex?H_0%20%5Capprox%2068.846%5C%2C%5Cmathrm%7Bkm%5C%2Fs%5E%7B-1%7D%5C%2FMpc%5E%7B-1%7D%7D" alt="H0 approximately 68.846 km s^-1 Mpc^-1">
</p>

These estimates depend on the chosen model, the loss function, data uncertainties, and the training process. 

### Project Status

This is a research and exploratory learning project at the intersection of cosmology, scientific machine learning, and physics-informed deep learning.

