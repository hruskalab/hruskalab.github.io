---
layout: page
title: Reorganization energy
description: from explicit solvation
img: assets/img/reorg-hist.PNG
importance: 2
category: work
---

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/reorg-hist.PNG" title="histogram" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/outer-sphere.PNG" title="outer sphere contribution" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The solvent at room temperature is not static. Chemical changes to the center molecule lead to a reorganization of the solvent, measured as reorganization energy. Previously the computational estimation of reorganization energy was done only for a limited number of systems, but with high-throughput simulation with <a href="https://github.com/Liu-group/AutoSolvate">Autosolvate software</a> described [here](../3_project) this could be done for 100+ molecules. The reorganization energy can be split into the contribution by the center molecule and the contribution by the solvent. The fraction caused by solvent (outer-sphere) shown above differs for individual molecules.
<div class="caption">
    [Hruska et al., Bridging the experiment-calculation divide: Machine learning corrections to redox potential calculations in implicit and explicit solvent models, 2022]
</div>
[Previous](../1_project)  [Next](../3_project)