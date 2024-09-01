# Machine-Learning-Models-for-Predicting-Quantum-Spin-Interactions-in-NMR-Simulations
### Problem Statement
- Nuclear Magnetic Resonance (NMR) is an experimental technique that allows for the control and measurement of nuclear spins in crystals and molecules.
- A common "recipe" for NMR is called the spin echo: the spins start aligned, begin to disperse, and are then refocused. This creates a sharp peak, or "echo", in the net magnetization of the material at a later time. When the spins interact with each other, this refocused echo can become highly distorted.
- Materials with strong electron-electron couplings have a variety of applications, from superconductivity to ferromagnetism. They also tend to enhance the nuclear spin-spin couplings, allowing NMR to act as a probe of these important systems.
- Design and train a model that predicts the strength and shape of interactions between the nuclear spins from simulated time-dependent magnetization curves.

### Electronic and nuclear spins
- Most materials can be classified by their electronic properties into three categories: metal, insulator, and semiconductor. These terms are based on a semi-classical description of the electrons in a crystal. The electrons are treated as a collection of classical particles, with energies that depend on their momentum in a way determined by the atomic structure of the crystal.
- However, there are other electronic phases of matter that are truly "quantum" and cannot be described accurately with a classical analogy. In these scenarios, complicated structures in the electron states can give rise to large electronic spin density or strong electron-electron coupling. Because of these strong couplings between electrons, they are often hard to probe experimentally.
- Luckily, electrons can interact with the nuclar spins of a material (by way of the hyperfine-interaction). If the electron-nuclear coupling becomes strong enough, then a non-neglible two-step process can couple the nuclei with each other throughout the material. That two-step process is when a nuclear spin couples to an electron and changes its motion, and then that electron later "scatters" off another nuclear spin elsewhere in the material.
- We represent this two-step scattering prcoess by way of an effective spin-spin coupling between a nuclei at position. There are two datasets, "gauss" and "RKKY", and thus you will have to generate TWO models and hand in two models.


### Goal
Predict three real numbers from an input vector of complex numbers. Which are the coupling strength, the coupling length and the decay rate of the spin information which will depend on the details of the nuclear-electron coupling and the quantum state of the electrons.

### Solution
- For the two model performances with distibutions and the determined variables ($\\alpha$, $\\xi$, and $d$) from a single $M(t)$ curve with whole documentation for respective models are presented [NMR_Challenge_gauss.ipynb](https://github.com/aviiacharya/Machine-Learning-Models-for-Predicting-Quantum-Spin-Interactions-in-NMR-Simulations/blob/main/3_Hackathon_NMR_Challenge_gauss.ipynb) and [NMR_Challenge_RKKY.ipynb](https://github.com/aviiacharya/Machine-Learning-Models-for-Predicting-Quantum-Spin-Interactions-in-NMR-Simulations/blob/main/3_Hackathon_NMR_Challenge_RKKY.ipynb). 
- The solution for model's evaluation of the Gaussian data [gauss_mat_info_eval.txt](https://github.com/aviiacharya/Machine-Learning-Models-for-Predicting-Quantum-Spin-Interactions-in-NMR-Simulations/blob/main/gauss_mat_info_eval.txt) and  RKKY data [RKKY_mat_info_eval.txt](https://github.com/aviiacharya/Machine-Learning-Models-for-Predicting-Quantum-Spin-Interactions-in-NMR-Simulations/blob/main/RKKY_mat_info_eval.txt).
- Respective models are [gauss.h5](https://github.com/aviiacharya/Machine-Learning-Models-for-Predicting-Quantum-Spin-Interactions-in-NMR-Simulations/blob/main/gauss.h5) and [RKKY.h5](https://github.com/aviiacharya/Machine-Learning-Models-for-Predicting-Quantum-Spin-Interactions-in-NMR-Simulations/blob/main/RKKY.h5).
