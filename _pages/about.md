---
permalink: /
title: "Exploring the science of water in a changing world"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Hi! I'm Yalan Song, a Research Assistant Professor in Water Resources Engineering at The Pennsylvania State University, working with Prof. [Chaopeng Shen](https://water.engr.psu.edu/shen/). I earned my Ph.D. in Civil Engineering, with a minor in Computational Science, from Penn State under the supervision of Prof. [Xiaofeng Liu](https://water.engr.psu.edu/liu/). I also hold an M.S. in Ocean Engineering from Shanghai Jiao Tong University and a B.S. in Ocean Engineering from Tianjin University.

My research focuses on large-scale hydrologic modeling, climate impacts on water resources, machine learning, environmental fluid dynamics, and sediment transport. Through my research, I aim to advance our understanding of the water cycle and develop next-generation hydrologic prediction systems with AI to support water resource management, climate adaptation, and hazard mitigation in a changing world. Here is my [CV](https://Yalan-Song.github.io/cv).

Selected Research
======

Differentiable Hydrologic Modeling (AI+physical principles) for Extreme Events
------
This work demonstrates that differentiable hydrologic models, which integrate hydrologic principles with neural networks, can provide more reliable predictions of extreme and unseen flood events than purely data-driven deep learning models (e.g., LSTMs) while maintaining physical interpretability and spatial generalizability, as well as producing good estimates of untrained internal hydrologic variables.

Song, Y., Sawadekar, K., Frame, J.M., Pan, M., Clark, M.P., Knoben, W.J., Wood, A.W., Lawson, K.E., Patel, T. and Shen, C., 2026. Physics-informed, Differentiable hydrologic models for capturing unseen extreme events. Water Resources Research, 62(2), p.e2025WR040414. [https://doi.org/10.1029/2025WR040414](https://doi.org/10.1029/2025WR040414) 

An improved differentiable HBV method that can surpass LSTM in predicting unseen extreme events with 50-year or 100-year return periods by around 10%
![extreme](/images/extreme.png)

AI for Continental and Global Water Prediction
------
I developed δHBV2.0, a high-resolution differentiable hydrologic model that integrates physical principles with neural networks for continental- and global-scale water prediction. By explicitly representing sub-basin heterogeneity, δHBV2.0 enables seamless streamflow simulation across approximately 180,000 MERIT unit basins across CONUS and can simulate 40 years of streamflow in just one GPU hour. Compared to the National Water Model 3.0 and existing global hydrologic models, δHBV2.0 represents a step change in large-scale, high-resolution hydrologic simulation capabilities. National and global hydrologic [datasets](https://Yalan-Song.github.io/datasets) from δHBV2.0 are publicly available.

Song, Y., Bindas, T., Shen, C., Ji, H., Knoben, W. J. M., Lonzarich, L., et al., 2025. High-resolution national-scale water modeling is enhanced by multiscale differentiable physics-informed machine learning. Water Resources Research, 61, e2024WR038928. [https://doi.org/10.1029/2024WR038928](https://doi.org/10.1029/2024WR038928)

Ji, H., Song, Y., Bindas, T., Shen, C., Yang, Y., Pan, M., Liu, J., Rahmani, F., Abbas, A., Beck, H. and Lawson, K., 2025. Distinct hydrologic response patterns and trends worldwide revealed by physics-embedded learning. Nature Communications, 16(1), p.9169. [https://www.nature.com/articles/s41467-025-64367-1](https://www.nature.com/articles/s41467-025-64367-1)

Comparisons of δHBV2.0 with NWM3.0 and GWMs/
![δHBV2](/images/δHBV2.png)

AI for Bathymetry Inversion and Scientific Learning in River Hydrodynamics
------
This work is a collaboration with Prof. Xiaofeng Liu exploring how AI can advance river hydrodynamic modeling. We first developed neural network-based surrogate models to accelerate river hydrodynamic simulations and applied them to the challenging problem of bathymetry inversion. To overcome the limitations of purely data-driven approaches (surrogates), which require large training datasets and often generalize poorly beyond the training domain, we then developed a differentiable hybrid framework that directly couples neural networks with numerical solvers (shallow water equations), called USWEs. This approach enables efficient and physically consistent inversion of hydraulic parameters, demonstrating how AI can help rather than replace classical numerical modeling for scientific discovery.

Liu, X., Song, Y. and Shen, C., 2024. Bathymetry inversion using a deep-learning-based surrogate for shallow water equations solvers. Water Resources Research, 60(3), p.e2023WR035890. [https://doi.org/10.1029/2023WR035890](https://doi.org/10.1029/2023WR035890)

Liu, X. and Song, Y. (corresponding author), 2025. Scientific machine learning of flow resistance using universal shallow water equations with differentiable programming. Water Resources Research, 61(9), e2025WR040265. [https://doi.org/10.1029/2025WR040265](https://doi.org/10.1029/2025WR040265)

<video controls autoplay muted loop playsinline width="100%">
  <source src="/images/manningn_github.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


Spatial distribution of Manning's n in a real river channel learned by a neural network within a differentiable hydrodynamic model (USWEs).
![Manningn](/images/Manningn.png)

Environmental fluid dynamics and sediment transport
------
During my Ph.D. research, I developed a high-fidelity three-dimensional (3D) hydrodynamic--sediment model to address a long-standing challenge in the field: accurately simulating 3D scour around complex hydraulic structures. By incorporating an immersed boundary method and an adapted wall function into a 3D scour model, I resolved numerical instability issues present in previous approaches and achieved the first successful simulation and validation of 3D scour around structures with complex foundations using unstructured meshes.

Song, Y., Xu, Y., Ismail, H. and Liu, X., 2022. Scour modeling based on immersed boundary method: A pathway to practical use of three-dimensional scour models. Coastal Engineering, 171, p.104037, [https://doi.org/10.1016/j.coastaleng.2021.104037](https://doi.org/10.1016/j.coastaleng.2021.104037).

Song, Y., Darzikolaei, S.A.M. and Liu, X., 2022. Scour around underwater unexploded ordnances (UXOs): An experimental and computational investigation. Ocean Engineering, 262, p.112146, [https://doi.org/10.1016/j.oceaneng.2022.112146](https://doi.org/10.1016/j.oceaneng.2022.112146).

<video controls autoplay muted loop playsinline width="100%">
  <source src="/images/scour_github.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

Explore more of my research on differentiable modeling, AI for water quality and snow, river hydrodynamics, computational fluid dynamics, and sediment transport on my [research page](https://Yalan-Song.github.io/research)
------
