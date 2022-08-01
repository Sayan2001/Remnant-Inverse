# Remnant-Inverse

***Summer Project in June-July 2022 with Matthew Mould & Davide Gerosa***

# The Problem

Given the final spin of a remnant, can we speak about the properties of its parents?

# Solution

Implement a Deep Neural Network which can provide us the probability distribution of the parent's properties (namely, the mass ratio, the dimensionless spin vector magnitudes, the inclinations and the delta_phi.

We implemented a class of ***Normalizing Flows*** called **Masked Autoregressive Flows** using the Tensorflow Probability package.

In a nutshell, the flow takes a normal distribution and applies successive **invertible** transformations to it to achieve the desired probability distrubution.

# Testing

We then compared our results to a standard MCMC on the same data (using the emcee package)

Using a standardised statistic like the KS-Test, we conclude that the Normalizing Flow is quite good at reproducing the MCMC results.
The Q-Q (Quantile) Plots confirms the same visually. (The plots are available in the ppt)

The network is then implmented on the **GW190412** event and the distribution of its parent's properties are obtained as a corner plot.

Refer to the ppt for a comprehensive overview of this repository.








