# Inverse Design of Non-Periodic Dual-Pillar Structures for Dielectric Laser Acceleration
> A Thesis Research Project

---

## Documentation & Presentations

- **[Full Thesis PDF](docs/master_thesis.pdf)** - Complete research document with detailed methodology and results
- **[Thesis Presentation](docs/master_thesis_presentation.pptx)** - PowerPoint presentation summarizing key findings

---

## Overview

This repository contains the full body of research and code from my master's thesis on the inverse design of photonic structures for dielectric laser acceleration (DLA). The project focuses on designing and optimizing periodic and non-periodic dual-pillar silicon structures to maximize the energy gain of an electron beam.

The core of this work is the development and application of a sophisticated computational pipeline that combines **Finite-Difference Time-Domain (FDTD) simulations** with advanced, gradient-based optimization algorithms. By leveraging the **adjoint method**, this research efficiently calculates the electromagnetic field gradients necessary for optimizing structures with a large number of geometric parameters, making it possible to design complex, high-performance particle accelerators on a chip.

## Key Features & Technical Achievements

-   **Advanced Optimization Algorithms**: Implementation of a custom **ADAM optimizer** combined with a **basin-hopping** strategy for robust global optimization of non-convex, high-dimensional electromagnetic problems.

-   **Complex Waveform Generation**: Successfully designed structures capable of producing arbitrary, non-sinusoidal accelerating fields, including **sawtooth waveforms** and **multi-harmonic superpositions**. This demonstrates the versatility of the inverse design framework.

-   **Dynamic & Aperiodic Design**: Developed methods to optimize non-periodic ("chirped") structures where the periodicity changes dynamically with the electron's energy. This is a critical step towards creating realistic, high-gradient accelerator sections.

-   **Comprehensive Design-Space Mapping**: Systematically mapped the design space to establish an empirical, sigmoid-based relationship between electron velocity (β) and the achievable accelerating field strength (E1), providing crucial design guidelines for future DLA research.

## Core Methodologies

-   **Adjoint Method**: Used to efficiently calculate the gradient of the objective function (i.e., the accelerating field) with respect to all geometric parameters of the structure from just two simulations, drastically reducing computational cost.
-   **FDTD Simulations**: All electromagnetic field calculations were performed using Lumerical FDTD Solutions, integrated into a Python-based control script via the `lumapi` library.
-   **Custom ADAM Optimizer**: An implementation of the ADAM algorithm to perform gradient-based parameter updates with momentum and adaptive learning rates.
-   **Constraint & Weighting System**: A sophisticated system of constraints and weights was developed to guide the optimization, ensuring physically manufacturable designs and improving convergence by focusing on the most promising regions of the design space.

## Repository Structure

The project is organized into several key directories. For a detailed breakdown of the notebooks, please see the **[Project Structure Guide](docs/PROJECT_STRUCTURE.md)**.

-   `notebooks/`: Contains all the Jupyter notebooks, categorized by research theme.
-   `docs/`: Contains all project documentation, including the installation guide.
-   `examples/`: Intended for example scripts or simplified usage cases.
-   `results/`: Intended for storing output data, plots, or other simulation results.

## Getting Started

To explore this research, please refer to the **[Installation Guide](docs/INSTALLATION.md)** for setup instructions.

It is recommended to start with the notebooks in `notebooks/1_phase_analysis` to understand the fundamental concepts of phase sensitivity before moving to the more complex optimization studies in the other folders.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details. 