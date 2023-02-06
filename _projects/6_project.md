---
layout: page
title: Sampling of rare events 
description: for proteins
img: assets/img/folding.PNG
importance: 2
category: work
---
<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/schema1.png" title="adaptive sampling steps" class="img-fluid rounded z-depth-1" %}
    </div>

</div>
For larger molecules like proteins, the sampling of all conformations that the molecule reaches is challenging. To sample this ensemble efficiently, adaptive sampling stores the already sampled conformations and iteratively adds data points at the optimal positions. Here, machine learning of the latent space of protein dynamics helps. The open-source software <a href="https://github.com/ClementiGroup/ExTASY/">ExTASY</a> used to achieve adaptive sampling for 70+ residue proteins is described [here](../8_project). 


<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/folding.PNG" title="folding conformations" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/adaptive-explore.PNG" title="adaptive explore" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

To validate that adaptive sampling reaches the correct ensemble of conformations, adaptive sampling (black diagonal lines) is compared with plain molecular dynamics (colored background). Adaptive sampling (red) reaches the folded state (vertical lines) faster than plain molecular dynamics (blue). Note that the x-axis is logarithmic, indicating a significant speed up. 
<div class="caption">[Hruska et al., Extensible and scalable adaptive sampling on supercomputers., 2020].
</div>


