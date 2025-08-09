# Quantum Walks and Monte Carlo
## Team Name:

## Team Members & WISER Enrollment IDs:
Harini Muthurengan -

Manas Ranjan Nayak - 

## Project Summary:
In the era of Noisy Intermediate-Scale Quantum (NISQ) computers, environmental noise and gate imperfections present a significant barrier to reliable quantum computation. This project addresses this challenge by providing a detailed analysis of noise's impact on quantum circuits. We use the PennyLane library to build and simulate various circuits, including a "Quantum Galton Board" as an intuitive analogy for a one-dimensional quantum walk. This framework allows for a clear and quantitative study of computational accuracy under noisy conditions.

Our methodology involves creating three distinct circuits, the Quantum Galton Board, a Hadamard based Quantum Walk, and an Amplitude Encoding circuit for an exponential distribution. This diversity allows us to explore how different circuit structures react to noise. To simulate real-world conditions, we apply various noise models specifically, a depolarizing channel, amplitude damping, phase damping, bit flip, and phase flip after each gate. This gate level application of noise provides a more realistic representation of imperfections compared to applying noise only at the end of the circuit. We then employ a Monte Carlo simulation, running each noisy circuit thousands of times to generate a statistical sample of the output and form an empirical probability distribution.

The analysis phase compares the noiseless (ideal) and noisy distributions using a suite of quantitative metrics. We use Fidelity to measure the similarity between the states, aiming for a score of 1.0. We also use Hellinger, Kullback-Leibler (KL) Divergence and Total Variation Distances to quantify the statistical difference, with an ideal score of 0.0. Our findings show a clear and direct relationship, as the noise probability per gate increases, the Fidelity systematically decreases and all distance metrics increase. This degradation is visually demonstrated by a flattening of the distribution peaks, which signals a loss of the quantum state's intended structure and a randomization effect from the noise.

In conclusion, this project establishes a robust framework for exploring quantum noise and its effects on circuit fidelity. It demonstrates the fragility of NISQ era computation through the Quantum Galton Board analogy and provides a powerful, quantitative method for assessing this challenge. Our work lays the groundwork for future research into error mitigation techniques  and the investigation of more complex, correlated noise models. The project offers valuable insights that are critical for advancing the development of reliable quantum algorithms and hardware.

## Project Presentation Deck
[Presentation Deck]((C:\Users\seeni\Downloads\Quantum Galton Board Implementation Project (2).pptx))

