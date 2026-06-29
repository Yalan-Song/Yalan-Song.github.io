---
permalink: /research/
title: "Research"
author_profile: true
---


### Research Topics

My research develops artificial intelligence (AI) methods for understanding and predicting environmental systems, with a particular focus on physics-informed differentiable modeling. By integrating machine learning with physical process models, I develop AI systems that are more accurate, interpretable, and physically consistent for applications including flood forecasting, hydrologic prediction, hydrodynamics, water quality, and snow hydrology. I also conduct research on computational fluid dynamics and sediment transport, developing classic numerical solvers for simulating complex hydraulic flows and scour processes.

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

Extreme floods are becoming more frequent under climate change, yet purely data-driven AI models often struggle to predict events beyond their training domain. I develop physics-informed differentiable hydrologic models that seamlessly integrate physical process equations with neural networks, enabling more robust prediction of unseen flood extremes while improving physical interpretability and generalizability.

An improved differentiable HBV method that can surpass LSTM in predicting unseen extreme events with 50-year or 100-year return periods by around 10%
![extreme](/images/extreme.png)

**Representative publications**

Song, Y., Sawadekar, K., Frame, J.M., Pan, M., Clark, M.P., Knoben, W.J., Wood, A.W., Lawson, K.E., Patel, T. and Shen, C., 2026. Physics-informed, Differentiable hydrologic models for capturing unseen extreme events. Water Resources Research, 62(2), p.e2025WR040414. [https://doi.org/10.1029/2025WR040414](https://doi.org/10.1029/2025WR040414) 

---

### Differentiable National-Scale Hydrologic Modeling

High-resolution national water prediction is computationally expensive and difficult to calibrate using traditional methods. I developed multiscale differentiable hydrologic models that efficiently learn model parameters across approximately 180,000 subbasins while preserving physical consistency, enabling accurate national-scale streamflow prediction and water resource assessment. The resulting model outperformed the National Water Model (NWM) v3.0 at more than 4,000 stream gauges while providing a seamless, high-resolution streamflow dataset over the national river network. The model can generate a continuous 40-year retrospective simulation of the continental United States in approximately one GPU hour, demonstrating its exceptional computational efficiency for large-scale operational and climate applications. A 40-year high-resolution streamflow dataset over the MERIT Hydro river network (~180,000 reaches with a median reach length of 7 km) is publicly available at [Zenodo](https://doi.org/10.5281/zenodo.13774373).

![dhbv2-national](/images/dhbv2-national.png)

**Representative publications**

Song, Y., Bindas, T., Shen, C., Ji, H., Knoben, W. J. M., Lonzarich, L., et al., 2025. High-resolution national-scale water modeling is enhanced by multiscale differentiable physics-informed machine learning. Water Resources Research, 61, e2024WR038928. https://doi.org/10.1029/2024WR038928

---

### Differentiable Global Hydrologic Modeling

Global hydrologic prediction requires models that generalize across diverse climates and physiographic conditions. We extend differentiable hydrologic modeling to the global scale, enabling improved representation of hydrologic processes, climate sensitivities, and regional water availability worldwide. The resulting framework achieves a step change in predictive accuracy and efficiency compared with existing global hydrologic models. A 40-year high-resolution streamflow dataset over the MERIT Hydro river network (~3,000,000 reaches with a median reach length of 7 km) is publicly available at [Zenodo](https://doi.org/10.5281/zenodo.17042358).

![dhbv2-global](/images/dhbv2-global.png)

**Representative publications**

Ji, H., Song, Y., Bindas, T., Shen, C., Yang, Y., Pan, M., Liu, J., Rahmani, F., Abbas, A., Beck, H. and Lawson, K., 2025. Distinct hydrologic response patterns and trends worldwide revealed by physics-embedded learning. Nature Communications, 16(1), p.9169. [https://www.nature.com/articles/s41467-025-64367-1](https://www.nature.com/articles/s41467-025-64367-1)

---
### Adjoint-Based Differentiable Modeling for Large-Scale Implicit Hydrologic Models
Large-scale hydrologic models often rely on implicit numerical schemes, making gradient computation prohibitively expensive for differentiable modeling. I developed an adjoint-based differentiable framework that efficiently computes gradients for implicit solvers, enabling scalable end-to-end training of physics-informed AI models without sacrificing numerical stability or accuracy.

![adjoint](/images/adjoint.png)

**Representative publications**

Song, Y., Knoben, W.J., Clark, M.P., Feng, D., Lawson, K., Sawadekar, K.$^*$ and Shen, C., 2024. When ancient numerical demons meet physics-informed machine learning: adjoint-based gradients for implicit differentiable modeling. Hydrology and Earth System Sciences, 28(13), pp.3051-3077, [https://doi.org/10.5194/hess-28-3051-2024](https://doi.org/10.5194/hess-28-3051-2024) 

---

### Data Assimilation for Differentiable Hydrologic Modeling

Differentiable models naturally enable gradient-based variational data assimilation by treating model states and meteorological forcings as optimization variables. My research develops efficient variational data assimilation methods that integrate near-real-time hydrologic observations to substantially improve streamflow forecasting accuracy in physics-informed AI models.

![DA](/images/DA.png)

**Representative publications**

Jamaat, A.,Song, Y., (corresponding author), Rahmani, F., Liu, J., Lawson, K. and Shen, C., 2025. Update hydrological states or meteorological forcings? Comparing data assimilation methods for differentiable hydrologic models. Journal of Hydrology. [https://doi.org/10.1016/j.jhydrol.2025.134137](https://doi.org/10.1016/j.jhydrol.2025.134137)

---

### Hydrology-Informed Forcing Fusion with Differentiable Modeling

Meteorological forcing uncertainty is a major source of hydrologic prediction error. I developed an interpretable differentiable framework that uses neural networks to fuse multiple meteorological forcing datasets under hydrologic constraints, improving streamflow simulations while providing insight into forcing uncertainty. The resulting high-quality fused precipitation dataset also enhances the performance of other AI-based hydrologic models.

![fusion](/images/fusion.png)

**Representative publications**

Sawadekar, K., Song, Y. (corresponding author), Pan, M., Beck, H., McCrary, R., Ullrich, P., Lawson, K. and Shen, C., 2025. Improving differentiable hydrologic modeling with interpretable forcing fusion. Journal of Hydrology, p.133320. [https://doi.org/10.1016/j.jhydrol.2025.133320](https://doi.org/10.1016/j.jhydrol.2025.133320)

---

## AI for Water Quality and Snow

### AI for Suspended Sediment Prediction

I developed a large-scale deep learning model based on Long Short-Term Memory (LSTM) networks to estimate suspended sediment concentrations across the conterminous United States. This work systematically evaluated the strengths and limitations of deep learning for large-scale water quality prediction, identifying where AI performs well and where additional constraints are needed to improve robustness and generalizability.

![ssc](/images/ssc.png)

**Representative publication**

Song, Y., Chaemchuen, P., Rahmani, F., Zhi, W., Li, L., Liu, X., Boyer, E., Bindas, T., Lawson, K. and Shen, C., 2024. Deep learning insights into suspended sediment concentrations across the conterminous United States: Strengths and limitations. Journal of Hydrology, p.131573, [https://doi.org/10.1016/j.jhydrol.2024.131573](https://doi.org/10.1016/j.jhydrol.2024.131573)

---

### AI for Snow Water Equivalent Prediction

Snow observations are sparse in mountainous regions, limiting hydrologic forecasting. I developed LSTM-based data integration methods that combine multiple observational datasets to improve snow water equivalent estimation while diagnosing model error sources.

![snow](/images/snow.png)

**Representative publication**

Song, Y., Tsai, W.P., Gluck, J., Rhoades, A., Zarzycki, C., McCrary, R., Lawson, K. and Shen, C., 2024. LSTM-based data integration to improve snow water equivalent prediction and diagnose error sources. Journal of Hydrometeorology, 25(1), pp.223-237, [https://doi.org/10.1175/JHM-D-22-0220.1](https://doi.org/10.1175/JHM-D-22-0220.1)

---

## AI for Flood Inundation

### Neural Network Surrogates for Shallow Water Equations

High-fidelity hydrodynamic simulations are computationally demanding for real-time flood prediction and engineering design. I developed neural network surrogate models that emulate shallow water equation solvers with orders-of-magnitude faster computation while maintaining high prediction accuracy.

![surrogate](/images/surrogate.png)

**Representative publication**

Song, Y. , Shen, C. and Liu, X., 2023. A surrogate model for shallow water equations solvers with deep learning. Journal of Hydraulic Engineering, 149(11), p.04023045, [https://doi.org/10.1061/JHEND8.HYENG-13190](https://doi.org/10.1061/JHEND8.HYENG-13190).

---

### Bathymetry Inversion Using Deep Learning

River bathymetry is difficult to measure directly. We developed differentiable surrogate-based inversion methods that infer riverbed topography efficiently from hydraulic observations, significantly reducing computational cost compared with conventional optimization approaches.

![bathymetry](/images/bathymetry.png)

**Representative publication**

Liu, X., Song, Y. and Shen, C., 2024. Bathymetry inversion using a deep-learning-based surrogate for shallow water equations solvers. Water Resources Research, 60(3), p.e2023WR035890. [https://doi.org/10.1029/2023WR035890](https://doi.org/10.1029/2023WR035890)

---

### Differentiable Shallow Water Modeling for Knowledge Discovery (Parameter Inversion)

Beyond prediction, differentiable shallow water models enable direct learning of unknown physical parameters, such as spatially varying Manning’s roughness, from flow observations. We developed a framework that directly couples neural networks with shallow water equation solvers, allowing the model to infer hidden hydraulic properties while preserving the governing physics of river flow. This approach turns hydrodynamic modeling into a tool for scientific discovery with AI, helping reveal spatial patterns in flow resistance that are difficult to measure directly.

<video controls autoplay muted loop playsinline width="100%">
  <source src="/images/manningn_github.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


Spatial distribution of Manning's n in a real river channel learned by a neural network within a differentiable shallow water model (USWEs).
![Manningn](/images/Manningn.png)

**Representative publication**

Liu, X. and Song, Y. (corresponding author), 2025. Scientific machine learning of flow resistance using universal shallow water equations with differentiable programming. Water Resources Research, 61(9), e2025WR040265. [https://doi.org/10.1029/2025WR040265](https://doi.org/10.1029/2025WR040265)

---

## Computational Fluid Dynamics and Sediment Transport

### Diffusion-Based Sand Slide and Scour Modeling

I developed a physically based sand slide formulation that improves numerical stability and realism in scour simulations by representing gravitational sediment transport over steep slopes.

<video controls autoplay muted loop playsinline width="100%">
  <source src="/images/scour_cylinder_web.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Representative publication**

Song, Y., Xu, Y., and Liu, X. (2020). Physically Based Sand Slide Method in Scour Models Based on Slope-Limited Diffusion. Journal of Hydraulic Engineering, 146(11), 04020074, [https://doi.org/10.1061/(ASCE)HY.1943-7900.0001814](https://doi.org/10.1061/(ASCE)HY.1943-7900.0001814).

---

### Immersed Boundary Methods for Complex Hydraulic Structures

Predicting local scour around bridges, piers, and other hydraulic structures remains challenging because conventional mesh deformation or body-fitted mesh methods become unstable or prohibitively expensive for structures with complex geometries. As the riverbed evolves during scour, these methods require repeated mesh deformation or remeshing, which often fails for real-world bridges with intricate structural components. I developed an immersed boundary method that embeds complex structures directly into structured computational grids, eliminating the need for body-fitted meshes while accurately resolving flow–structure interactions. This approach substantially reduces computational cost and makes high-fidelity three-dimensional scour modeling practical for complex hydraulic engineering applications.

<video controls autoplay muted loop playsinline width="100%">
  <source src="/images/scour_github.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Representative publications**

Song, Y., Xu, Y., Ismail, H. and Liu, X., 2022. Scour modeling based on immersed boundary method: A pathway to practical use of three-dimensional scour models. Coastal Engineering, 171, p.104037, [https://doi.org/10.1016/j.coastaleng.2021.104037](https://doi.org/10.1016/j.coastaleng.2021.104037).

---

### Scour Around Underwater Unexploded Ordnances (UXOs)

I combined laboratory experiments and three-dimensional numerical simulations to investigate scour development around underwater unexploded ordnances. The work provides guidance for hazard assessment and offshore engineering applications.

<video controls autoplay muted loop playsinline width="100%">
  <source src="/images/scour_uxos_web.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

**Representative publication**

Song, Y., Darzikolaei, S.A.M. and Liu, X., 2022. Scour around underwater unexploded ordnances (UXOs): An experimental and computational investigation. Ocean Engineering, 262, p.112146, [https://doi.org/10.1016/j.oceaneng.2022.112146](https://doi.org/10.1016/j.oceaneng.2022.112146).
