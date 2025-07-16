# Project Structure Guide

This repository is organized into several directories to separate the raw research notebooks from the documentation and results.

## Core Directories

-   **/notebooks**: Contains all the Jupyter notebooks, organized by research theme.
-   **/docs**: Contains all project documentation, including this guide.
-   **/examples**: (Empty) Intended for example scripts or usage cases.
-   **/results**: (Empty) Intended for storing output data, plots, or other simulation results.

## Notebook Organization

The research notebooks are categorized into the following subdirectories within `/notebooks`:

### `1_phase_analysis/`
Notebooks focused on analyzing the phase response of the structure to geometric changes. This was critical for understanding the fundamental physics before attempting full optimization.
-   `e1_phase_analysis.ipynb`
-   `ypos_phase_analysis.ipynb`

### `2_optimization_studies/`
This directory contains the core optimization work, progressing from simple single-period problems to complex, multi-period, non-periodic structures.
-   `single_period_optimization.ipynb`
-   `multi_parameter_optimization.ipynb`
-   `non_periodic_optimization.ipynb`

### `3_non_periodic_structures/`
This section explores the design of non-periodic (aperiodic) structures, where the periodicity changes dynamically. It also tests the generation of complex, non-sinusoidal waveforms.
-   `sawtooth_adjoint_simulation.ipynb`
-   `sawtooth_no_adjoint_simulation.ipynb`
-   `sinusoid_superposition.ipynb`

### `4_field_analysis/`
These notebooks focus on analyzing and generating specific target field shapes, such as sawtooth and superposition waveforms, and include a fundamental study of how field strength relates to electron velocity.
-   `e1_sawtooth_waveform.ipynb`
-   `e1_superposition_waveform.ipynb`
-   `e1_vs_periodicity.ipynb`

### `5_final_plots/`
Contains the notebook used to generate the final aggregate plots for the thesis.
-   `final_plots.ipynb` 