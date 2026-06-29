---
permalink: /research/
title: "Research"
author_profile: true
---


### Research Topics

My research develops artificial intelligence (AI) methods for understanding and predicting environmental systems, with a particular focus on physics-informed differentiable modeling. By integrating machine learning with physical process models, I develop AI systems that are more accurate, interpretable, and physically consistent for applications including flood forecasting, hydrologic prediction, hydrodynamics, water quality, and snow hydrology. In addition, I conduct research on computational fluid dynamics and sediment transport, developing numerical methods for simulating complex hydraulic flows and scour processes.

* [Differentiable (Physics-Informed AI) Hydrologic Modeling](#differentiable-hydrologic-modeling)
  * [Differentiable Modeling for Extreme Flood Prediction](#differentiable-modeling-for-extreme-flood-prediction)
  * [Differentiable National-Scale Hydrologic Modeling](#differentiable-national-scale-hydrologic-modeling)
  * [Differentiable Global Hydrologic Modeling](#differentiable-global-hydrologic-modeling)
  * [Adjoint-Based Differentiable Modeling for Large-Scale Implicit Hydrologic Models](#adjoint-based-differentiable-modeling-for-large-scale-implicit-hydrologic-models)
  * [Data Assimilation for Differentiable Hydrologic Modeling](#data-assimilation-for-differentiable-hydrologic-modeling)
  * [Hydrology-Informed Forcing Fusion with Differentiable Modeling](#hydrology-informed-forcing-fusion-with-differentiable-modeling)

* [AI for Water Quality and Snow](#ai-for-water-quality-and-snow)
  * [AI for Suspended Sediment Prediction](#ai-for-suspended-sediment-prediction)
  * [AI for Snow Water Equivalent Prediction](#ai-for-snow-water-equivalent-prediction)

* [AI for Flood Inundation](#ai-for-flood-inundation)
  * [Neural Network Surrogates for Shallow Water Equations](#neural-network-surrogates-for-shallow-water-equations)
  * [Bathymetry Inversion Using Deep Learning](#bathymetry-inversion-using-deep-learning)
  * [Differentiable Shallow Water Modeling for Knowledge Discovery (Parameter Inversion)](#differentiable-shallow-water-modeling-for-knowledge-discovery)

* [Computational Fluid Dynamics and Sediment Transport](#computational-fluid-dynamics-and-sediment-transport)
  * [Diffusion-Based Sand Slide and Scour Modeling](#diffusion-based-sand-slide-and-scour-modeling)
  * [Immersed Boundary Methods for Complex Hydraulic Structures](#immersed-boundary-methods-for-complex-hydraulic-structures)
  * [Scour Around Underwater Unexploded Ordnances (UXOs)](#scour-around-underwater-unexploded-ordnances-uxos)

---

## Differentiable (Physics-Informed AI) Hydrologic Modeling

### Differentiable Modeling for Extreme Flood Prediction

Extreme floods are becoming more frequent under climate change, yet purely data-driven models often struggle to predict events beyond their training record. I developed differentiable hydrologic models that embed physical conservation laws into neural networks, enabling robust prediction of unseen flood extremes while improving interpretability and climate sensitivity analysis.

**Representative publications**

* WRR 2026 – Physics-informed differentiable hydrologic models for capturing unseen extreme events
* Nature Communications 2025 – Distinct hydrologic response patterns and trends worldwide revealed by physics-embedded learning

---

### Differentiable National-Scale Hydrologic Modeling

High-resolution continental water prediction is computationally expensive and difficult to calibrate using traditional methods. I developed multiscale differentiable hydrologic models that efficiently learn model parameters across thousands of watersheds while preserving physical consistency, enabling accurate national-scale streamflow prediction and water resource assessment.

**Representative publications**

* WRR 2025 – High-resolution national-scale water modeling is enhanced by multiscale differentiable physics-informed machine learning

---

### Differentiable Global Hydrologic Modeling

Global hydrologic prediction requires models that generalize across diverse climates and physiographic conditions. My recent work extends differentiable hydrologic modeling to the global scale, enabling improved representation of hydrologic processes, climate sensitivities, and regional water availability worldwide.

**Representative publications**

* Nature Communications 2025
* HESS 2025 – How many models do we need to simulate hydrologic processes across large geographical domains?

---

### Data Assimilation for Differentiable Hydrologic Modeling

Differentiable models naturally enable gradient-based data assimilation by treating model states and forcings as optimization variables. My research explores efficient assimilation of hydrologic observations and meteorological forcings to improve real-time forecasting and uncertainty quantification.

**Representative publications**

* Journal of Hydrology 2025 – Comparing hydrologic state and forcing assimilation
* Journal of Hydrometeorology 2024 – Data integration for snow water equivalent prediction

---

### Hydrology-Informed Forcing Fusion

Meteorological forcing uncertainty is a major source of hydrologic prediction error. I developed interpretable differentiable frameworks that fuse multiple forcing datasets using hydrologic constraints, improving streamflow simulations while providing insight into forcing uncertainty.

**Representative publications**

* Journal of Hydrology 2025 – Interpretable forcing fusion
* HESS 2025 – Ensembling differentiable and data-driven models

---

## AI for Water Quality and Snow

### AI for Suspended Sediment Prediction

I developed large-scale deep learning models to estimate suspended sediment concentration across the conterminous United States. This work evaluated both the strengths and limitations of deep learning for water quality prediction and identified conditions where physically informed approaches are needed.

**Representative publication**

* Journal of Hydrology 2024

---

### AI for Snow Water Equivalent Prediction

Snow observations are sparse in mountainous regions, limiting hydrologic forecasting. I developed LSTM-based data integration methods that combine multiple observational datasets to improve snow water equivalent estimation while diagnosing model error sources.

**Representative publication**

* Journal of Hydrometeorology 2024

---

## AI for Flood Inundation

### Neural Network Surrogates for Shallow Water Equations

High-fidelity hydrodynamic simulations are computationally demanding for real-time flood prediction. I developed neural network surrogate models that emulate shallow water equation solvers with orders-of-magnitude faster computation while maintaining high prediction accuracy.

**Representative publication**

* Journal of Hydraulic Engineering 2023

---

### Bathymetry Inversion Using Deep Learning

River bathymetry is difficult to measure directly. I developed differentiable surrogate-based inversion methods that infer riverbed topography efficiently from hydraulic observations, significantly reducing computational cost compared with conventional optimization approaches.

**Representative publication**

* Water Resources Research 2024

---

### Differentiable Shallow Water Modeling for Knowledge Discovery (Parameter Inversion)

Beyond prediction, differentiable shallow water models enable direct learning of unknown physical parameters such as spatially varying Manning's roughness. This framework combines numerical solvers and neural networks for scientific discovery while maintaining physical consistency.

**Representative publication**

* Water Resources Research 2025

---

## Computational Fluid Dynamics and Sediment Transport

### Diffusion-Based Sand Slide Modeling

I developed a physically based sand slide formulation that improves numerical stability and realism in scour simulations by representing gravitational sediment transport over steep slopes.

**Representative publication**

* Journal of Hydraulic Engineering 2020

---

### Immersed Boundary Methods for Complex Hydraulic Structures

I developed improved immersed boundary methods for simulating complex hydraulic flows and local scour around engineering structures. These methods substantially reduce mesh generation effort while maintaining simulation accuracy.

**Representative publications**

* Water 2020
* Coastal Engineering 2022

---

### Scour Around Underwater Unexploded Ordnances (UXOs)

I combined laboratory experiments and three-dimensional numerical simulations to investigate scour development around underwater unexploded ordnances. The work provides guidance for hazard assessment and offshore engineering applications.

**Representative publication**

* Ocean Engineering 2022
